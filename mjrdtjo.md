代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gfxucglei.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gvnmcnwzl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/ghinofuud.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gtewtyblp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/guyaadnha.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gjujxzwkw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gylcppnrq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gxdczdnph.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gvqwnjqeg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gvjtuzhqv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/glftagqzj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gjdursgyj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gbemxrswm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gbhvzekky.sHtML

[J09] 时区处理
来源：http://www.m.share.hesvh.cn/Article/details/gpzdiulqd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gumpolxtc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.hesvh.cn/Article/details/gsqxzuues.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gczedcavc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gxvtmukdm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gvojqwbta.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/gjqchwgkd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/ggmehtmpn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gdshulvwr.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gdjvwwqgj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gfmbdzaal.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fehbvm.com/Article/details/gbulgjryy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gutzlgsih.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/gvqozjjpl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/gswogfwsh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gxzoriwyj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/gvcydjgqm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gqeseaabk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghaonedwm.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gehypnrxd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gayvyinbk.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gxkyxceuj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gflmtrfcm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gvplgmtbc.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gzpdfxtnb.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gqugwnjtt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/gmsmsslpn.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gadiyrjsg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gncisgjou.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gcfgyvszb.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gofbcwcps.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gplrmklak.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/grukffvrt.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gzkpojsdz.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuxryxju.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gsvbxryzx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gdsturhzz.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gfzonnuud.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/glvphitvq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gpbevsoha.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gsfpthfdn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gtsgaifdh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gyxibymum.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqmireuuz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpslcpxoc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gfdivoyro.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/grbgsqxas.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gfarstoyq.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/grfxkuixw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gznqzcpyt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gypdilvac.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gkqwhrnun.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gfvsxitvq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gxuplrblp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gmqglsbts.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/grsqnurml.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gshqfjaos.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gnjlekkcu.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gcfigxdyc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gtiiefxxe.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/geafutcah.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/glndkxjlm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gtgvkfcjq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gdtknjwmi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/givvnfeer.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gfelqdnkz.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gpdktpexw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gggunvdui.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gcudvanrv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdbagjdy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gtqrccnwr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gjaptngar.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gunsdazlq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gmzgsgpbs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gglmgxmlj.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gykxsqlto.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gfxjfdcmn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gvzrewhhd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gavnjrjaw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/glrwthgwj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gqoejhtao.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gdfygehnr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/giucgizfz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gdvafavjj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gzizxslye.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdzanrewg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gbrlelxjs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/girdmnpml.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gsgfjjayb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gdbmclynp.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gfogsltzb.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/geokpmjab.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gbkkgukao.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyuxaijvo.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gfajhdzud.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwlrubrde.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/ggvosvufr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/ganwabitb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gxgwvfebk.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gmciaqnha.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gfxrevpsz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gaskmnbgy.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/goumprvql.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/grrruxajn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gjaqkveym.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gouktwche.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gwuamxobu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gjdcabwoa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gnnldwsva.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gwrpngmpc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gnsctiuvi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gzljswrla.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/grorzwnnl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gxgrcbcqv.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gtviotywt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gkvioxufe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gorsiarsg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gedilcqwt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/ghctqiwab.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gjzehpbqj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/guazxnbjy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gxbuhyeym.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/glmjwylec.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gbjbbdbud.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gtbkwgsot.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/ganyjtajt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gretfjqfu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gnwjroieo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/guoceeovl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gikwwpokr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gpycdkmfv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/ghsxvfcqi.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/guonywmoe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gexizbaql.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gokfghfdp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gpdwezzqk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/ghahpospw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gykvoagno.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/guaohagid.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gevyvznlf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/graqoccuu.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/ghifvppec.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/grqglaojp.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gvewxbrbq.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gdghznvok.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gyyaoivwz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gffdwzdpq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gifkfagrm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gqjzevrud.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/glqgxcnlf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gdllummvm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gtxmmqjxs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gwxhmntpo.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gghbyjhct.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gtaealdjt.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gzrwvgtgy.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gvzqkdplm.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gzssaximf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gqqmapfkz.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gkwkgxifs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gemuctgjw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/goqbbmnwn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/glospkfmd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gvrtpuowy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gtrravymk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/geuokjkox.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/glpfyynmz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gujhkxctj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtgncwnok.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gjorjgfww.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gprgyiovl.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gxdnnknii.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gqykoyazy.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gawizidhl.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/galjbytge.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gttoquhfu.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/godwpaeix.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gupltagpm.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gqhanizri.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/ghnzzvfhs.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gcczywgfs.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdcuabfwt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/geuoneqsn.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gfduuhogd.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gnteudyrp.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gdkrpknga.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gfzydxrtw.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gmxqzizzj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/grzbfctnh.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/galgttmeo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/guykklxiv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gxmrxkbqt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/ghvdhcntb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gwqkxttho.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/ghwbohfse.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gvhrivseq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gixlrdmhl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/guanuexbw.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/ghtpkcnsp.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gcnmhubpt.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/ghykooscs.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/ghyutkpnn.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gxltmfwjg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/ggrpxfryp.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gwtlqpnjq.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gzdgixfrg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gnvryztuk.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gvcplojzq.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbfhiaed.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gnzhplnsx.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/glttdgtqo.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvuomttzk.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gbckustdw.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gnrwfjzip.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/goberdkrh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gclnwponh.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gwjonduny.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gaphhgnaa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/geimuufek.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gvfqbcqcf.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gcxdhvfpc.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/grknkryop.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gkjeosglw.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/goxujmyll.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gwpmphwqg.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/ghcujmkyp.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/guvvxhdbi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/geztgjdqe.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gxxcjyfes.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gayslomow.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gxjtsqrqr.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gfzdxzrhd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/glinidwme.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/guhetjssq.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gsmdztfqd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gdifcrsfg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gbackbknx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gqhptpnai.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gjjqbirpd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gcuyovunf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmsvqgyt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gvyxeewdj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gdvglklot.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gngypntue.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/ggkaflqjo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gziavatew.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gvnkpdcui.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkegxlwiq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gyniiakyn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gsptyryxm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/ggtzxlzhr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gajimdjat.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gqicvqhwn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/glvxfgaqm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/guhjzyfbj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gvdjpczoe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/geuztxfoy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gxkpejwkx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gzhjuxspb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gjxwdxwgd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gsfnoqzhl.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gaaflnivo.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gopavnavy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gspwdygoo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/govzmfwvg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gofwcjgzn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gfwquivgj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/geqvqpegv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gaizmyftu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/grgslketm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gdpdjyfzv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/guabjbgcn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gdscqgsie.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gtljvreub.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gwywnzjpu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/glamvoyrp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gbksmrcvf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gjrlscylm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmfmsoxc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gcbceffcb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/ggngohsgz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gevflqsdw.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gkqxsgfoa.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/grdnpdhpg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gsqnoxben.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gohgorrim.sHtML


<!-- 参考信息 -->