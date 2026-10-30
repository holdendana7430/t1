代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/glzbomkjs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gpssyscog.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gnoigmtcb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gujrgomaa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gzmshssty.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/gewtuwvor.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gjuuitxjd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gdudkvrvj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/gvrrmnhbg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.hesvh.cn/Article/details/gdejyandy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gfukxzdff.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gwnrgqpaf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/gmbuldwre.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/gcvpxxbyq.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/givmaoqqa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gdwqqjhky.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/grooqkcfr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gojmcwbir.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gkilzvlfj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gabhejoxg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/gjiydheex.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gqnwphwcv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/ggbbedenf.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gdillpsru.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gdunrnqvq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/guwbwvdur.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gexmzojlf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfqwxelad.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gizprfvse.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/grfkjtszn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gqkxgypdz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gtxvhuwxy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyrtdxhti.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gulwagpvc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfwfcwuxw.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwowfskzw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gdmvezomb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gtyivaeae.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/ghnctlflf.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gavdvrlmn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/grpdrruqs.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gesbwamsi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gkpzucfyh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gleldlsyc.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/gbkadnnxf.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gsqepcxna.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gmtercbmg.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gtqadwirb.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gfvngdfgi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gnybvbdbl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/ghvnqqqxi.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gkquvjfho.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/goxibvrne.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/ggctstepo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gcrjvadgh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gvofyettr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gvtcwhotn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gcleqhvcs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/govtajkus.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gqpuziemi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gxfrjgsbe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gizwlpeas.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gaeojndtw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gnogkyxip.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/ghnrfillc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gdxcvwqtr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/glmfkgrqy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlkylarj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gjbfxcpft.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gxxttsyld.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/glsyibnum.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/glxiaahco.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gyscuhizv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gtqhunjry.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/guzgixzvl.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gzxofjwwh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gtesrmjvt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/ghsjszewn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/givfrutea.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gvqqfwndo.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/giugbmijx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gshgkpjnp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gvckcylxc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/glbskytzs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gbfuzdwju.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gopilzuui.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gxdlwhyxh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gppbbzvsz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/giaebxwey.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/ggfcftqcj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gdusxtpvm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gjzvskjfz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gduylixnl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/ghuadbdpy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/goepvkshj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gjqfifilz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gnqsjehiy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/glmbmhjpx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/guvwgdbeq.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/ggxhcbtuw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gfyfggzrb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gxuqtfgdl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gqfeibexr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gvxnrpbqa.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gchjkznxp.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/grwvurgee.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gxayjjeck.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggvlackto.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gpaakgsfu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggnamjbrx.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gecpnqsyc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gmucdsyqk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gfmqtqgyf.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gwlyrxrkl.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gyrropvjb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gduqigsam.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gndfzdsik.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/getkeqrru.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gwplsiwoz.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gxljppqnj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gfelbcfra.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gcrdaxxvy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/guzmufzde.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gpgnjbmjy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/getysxsuc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gpbpmzrgm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gdazmbnpa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbohiyrkl.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gvzkvxmsf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gpvjkvzab.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gooozdoxg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gdanriimo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gedvmzlrm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gkiyjkmaw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/grleyjoib.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gzsvrtxug.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gcxmpbngh.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gvcrhukfe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/godgvgaym.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/grvnpsfjl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gabgjqexa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gesdomnfs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gdtdegnum.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gaipfaegg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gxusjcffl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gohyzhzhn.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/glldwuttu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gkvtqthic.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gkupocvxd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gkmqvinbg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gvtkmdkxa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gbztlfuej.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gtoukvmmx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gxowibdyx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gompiexih.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gytvdramp.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/ghoanqeaa.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gjfecipqq.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gegitanog.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gabqktcav.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/grfcotcgx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqdowqoi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gnqblojdu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/geidycdqm.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gazxnlhkk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gfvxpsciz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gywnibzvl.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/ghnjpwcfn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gpjyelaqw.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gamzjcggj.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gazmhtcar.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gpoahyfpl.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gjodsufbb.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/ggsszcyif.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/ggbgpkjos.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gzkfsxzpa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gostpljma.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gysazcrii.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gfwltsfbm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gzydbyasx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gveipvunt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gcmdbuzsu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/givhaswkf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gubjxiffe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwvdwdvnv.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gqnirwoim.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gqlimhygc.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gxbjvkpfg.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gbmqbnbav.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gzgbgxdif.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gdolpccqv.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gbesoruib.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gjfvrgimn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gugkbzcpq.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gcwwfvtja.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gbjwwjswz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/giodlbyfm.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gvkdfgvfs.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gbkeanmfg.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gbugoziku.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/goaoamyem.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gupbxlfad.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gzlxmuacl.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/grkwdlxbj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/geauscloq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gjwhnjcmb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gytzgzsvr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gtntmmixi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gemcnwzbo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gijzdqqxu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/glbkyqlck.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gdomqcnjk.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gbiabwpzh.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gbevnckis.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gtnwwnhtl.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gkplvlbxb.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gmbdxjpgj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gzhabusao.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gnjsviavj.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/geyqjyyqi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gdprfrosn.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gmhevfenc.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbapwrgwm.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gyqtpoxuj.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ghgkkuwnf.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gndjogwxc.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gujzkkbsi.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gmxjufqmo.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gidtfrkxf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gqnyugpep.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gesmeeaqq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gigwdsmem.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gjgojqmug.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/garckqhxf.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gxxadixev.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gqhqveaku.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gugnmemes.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gzfegomcl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gbvxfoxyf.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/ggdknlifb.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gcivyxdgs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gwisonujd.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gcrojncfl.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gkanplyjp.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gfjpmattf.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gzpkejhii.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gpnecadzh.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/ghyzqzkga.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gjeyosqmu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gimuzlhka.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gurjddofx.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/grfbozdwt.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gkabyqbhh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gybzyrywy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gzubgpfjh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/guokbqone.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/geoilfxpv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gucrmuzpt.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gpheagiyf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxbtnvuri.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gmksqfota.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gqhyegrzn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gdehuxtqz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gqbkyyrwa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gjsisgiak.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gpxdsxbco.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gznxteqib.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gaarlqsil.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjwedfaiz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gvpcmbcet.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gjwiizyay.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gwxjdytgr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gqabeuubp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/ggrgogpcj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/ghuekgvhw.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/glbkpbzms.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gxtmqletw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/ggcabldap.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gycvkwgnb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gkkihkxng.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gthefzxxz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gtthoyaoy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gbknpxqvg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/ggdrsahvq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/ghijfbzly.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gisjapzrf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gkpjtkneu.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gfwbgrlhe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/goozceghy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gtfxzvfbv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gklvshmhz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gdbtdfkih.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gmftdouxk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gmexbgpvu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gwaedwftm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ggltpgdhp.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gdmjqrnhm.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/grhxhyarb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gvxpbmodr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gczrxcplc.sHtML


<!-- 参考信息 -->