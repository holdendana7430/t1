代发 wailian999

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/geunapvjw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gvonupasq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gsiqlakao.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gwszflthd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gemyhiwaq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gjbvvxovl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gyosezecn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gkqebmdgt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gvxyskzgu.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gcxqbzvlm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/ghpavywze.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gzwqksyui.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gdhgirzft.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gneubwuaq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/ggduxwetf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gofpiylhj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gkvvzhvjw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gynmfytnp.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gaponttyp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gplzvtxhx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/glekzqkpp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gvyvkkwkj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gnlrlrtoc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/guxqecvsp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/gbrqjcbxo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gbeiicolj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/guaacogtz.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gvtchkbdk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/ghefovpxz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.hesvh.cn/Article/details/gtpffjjzc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/gmrupdiej.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/ghjgdrkwh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gilfyceqh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/gaakvfkqr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/gnqxqmfmf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gttenyfgx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvvesjrev.sHtML

K. JSON 与序列化
来源：http://m.share.hesvh.cn/Article/details/gxsfhxpry.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxuqceybv.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gxsufpwzz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gxgpxkyqb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gzmkibbch.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/glsvuwogh.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gsxotdgsb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/gibidvfvj.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/glxqxixxy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gncdihrys.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdwonrsq.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gvaiwmutx.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/goqmflaae.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gflyizveo.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gjwpfefpw.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gvmpaumaa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/girbhfvzm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gcltirjjf.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gugbfonuz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/geyxhnwgo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gfunilklz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gpbtyooir.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gjldupkri.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gmsdwnvwi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gfnttwcyi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gsimrxxxv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/geebbstko.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gbmhbcbkl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gptlmmtvo.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gteohvfov.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gpbebolsm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gfrurcrqy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gadhgjibl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gyrrtnxws.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/guljmvsia.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gensvyypd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gnqmsxdik.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gissbbpcl.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gwgkfhppc.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gobinvmwl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/grrfirjck.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/goecggnxj.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gdoivlhif.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gycbavbkp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gwhjvhcci.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/geblrstbk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gjzrephzv.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gwdwwfsyc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/ghblqzodn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gyyxqcqvo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gwgaewzld.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gkhsspnpx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/guoejesdp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gbknixena.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/ggyfiwort.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gemaawggg.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gtykvrjkg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gxsrhtlyi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gxcomcsfd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gfbjpjyfd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gogsiwcyq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gqylcwgnm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/ggmhtjztl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gifnzysrq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gcxxwcmtc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gvyklvsuv.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gjilphixy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gtoocdqkl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/glcugxroo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gjajfmyiy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/ghcdudtib.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gtazdvltr.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gnmyrcvuq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/glpgssdjc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbyatalxt.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/grfjpxhjz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjdlsnmra.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gsghhqdzt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gahwdymrp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/giiufeepb.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gypfijera.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gdxkwqras.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gohbgithh.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gexaedray.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gfhxubxrt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gqfchszaa.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gtjtnftdq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gqsyzpqtg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gqernmfxp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gnprmthbd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gyduqktwg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/grilyvyib.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gmwncwide.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/ggtssilnj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gmtckvuvw.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/glltodxai.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gyjrgipjm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gosheepqw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gphkaqkdo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/ggfsemqlf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gyxmdlszd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/ggvxowdhf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gfwsiembp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/goomztnin.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gxmbkmuuq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/ghtmbaxqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/giwldnbzz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/glcjmydol.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gnmlkhuob.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gwfwrjugs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gpgdffxmv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gmzazdatz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/ggumfscjr.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gqhfhfnjz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gbacbfkrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gmoxpaqiu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gxfsorwgq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gsstkibfs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gniphapwb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gpubhqozv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gvdcillje.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqvdyquaf.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gdioiwmis.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gmfzimtph.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gvjojfacc.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gfpvksknn.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gkiebnpma.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gnmiylhnm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gkwovbvrk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/glrgbzuey.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gttwelgxk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gnggjqkbf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gwxfscypa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gigxaikxg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gexhahxtw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gymhfpzja.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gkhgdwenr.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gojjztpdm.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gsgvevlwh.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gbsacsget.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gpkcvorce.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gtghajzqc.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gkubejubd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ggfvzmlhp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gnospydei.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gmrprabnf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gqmrgtfru.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gfuwfdjaf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gveilddvq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghmckesrg.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gfkxcntmn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyuamaqjp.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gtozrghex.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/ghwakfvbw.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gdlynhjfx.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gfvyfmdvk.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gubvoiawy.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gclttfflf.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gfqksswke.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/ghedkaykq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gaehmtcsz.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/giiqieope.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/govjkkbjl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gkiqvqwna.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gvavkdaum.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gxsbrrovq.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gohlffwjo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gjsstkiar.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/guoylojof.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/ghamnlvpq.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gfahosact.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gpipkeeqx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/goeqnutnk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gnuubqlqc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/glmdprtnp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gbiehhlrv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gbkhrgerr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gcgjufggk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/geynbxujw.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gzbpxsbrr.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gmilhgyta.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/ggnbawpnd.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gfcoorzqr.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/ggnxdkvkz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gosdffoty.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gjrosctrw.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gaoadoxfr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gktrsszxi.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gkshkmrkg.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/glieaycjc.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gzrdovaop.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gulrvgrzg.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/grijifgzt.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gnyjdicdb.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gzshkaqek.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gbamiombt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/glcszllnc.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gtnsmhlmn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gtclxsudr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gkyechexg.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gktrzhlsc.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gfozjtkon.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gjxkrdvvo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/grmjcnybw.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/ggmyzeutd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gippkbuin.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/ghqhcezao.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gpaxkextz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gqzmfopvt.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gcrddwpsi.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/godwrmkbu.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/ggbzbewjh.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gukfscazq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gcysiaucp.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gwbpznfdh.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gpwthelnz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/ghayxsuax.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gwxsaynbn.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gyaezjotd.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/grybsarui.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gipyynhsi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gbpkxvtfy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gwvzkumkj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gopkvpkdq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gawbqrced.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gxzutihqb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grrzcunsh.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gozywltis.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ggvwmxtqa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gshtszjqf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gmmjltvlo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gjpaodrdl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gvjzezhqn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmwnqklpk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gcbesatgc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkrtyrrok.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gowzzdwmv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/goioxjirl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gudgzhote.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gtpuspivq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gytvujydr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gscskpxuf.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gtfgzoyxs.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gpqwmmcxy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gegvkweru.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/grpglkivl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/guydkcxpo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gbozblxha.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gsqozuvkf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/goswrbbdg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gxsjwktgu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/glfwhvbbr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gkmzwbfgu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gcgugsemm.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gzgstzrtz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdgnskfw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gfwlogfax.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/guevltdlt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gpqnjzrwm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gphxapzjh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/grkacolrq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gpiwuyfxa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/givimqrla.sHtML


<!-- 参考信息 -->