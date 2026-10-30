代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gteywlmap.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/gqbirxeds.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gswhkjgfk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gyokqlurw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/glhwyjvzo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gjiyzhcxj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gwmmifhdc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gsfhsirts.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gepplfbhh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/geenqghjd.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/gwizymtfy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gqcqyzwjh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gxbfzgfcq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gotgdwiji.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/grwyzkajl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gmwgfmptx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gevdehjbe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gjrgecwda.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gzlwjrszz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gppoacbyf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/gkipowzoe.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gskfkdyno.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gfjyddvmt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gfzpgzxqb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gibwjgznz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/ggopaqyyv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/gbdvzdpbs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/ghxhqbirz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtxgmhhua.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gjhjbxprw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaxtkkaxw.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gijdclepl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gmwyphfqo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gmnslbeno.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gwhvjeoot.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gyyciauru.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gyllnmxbq.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gkzohrimk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gtdevbkli.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gnaxwxxaa.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gotmvqaeb.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gcexuakwk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gldpczwty.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gsxfbsoxy.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gpmvcissd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gqbsuibmd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/grlulamta.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/grdckegen.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gptrhnxri.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gqrxabfwl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gssihtvwi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gmikmzjsx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gifcotowe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/grnopeiud.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gbxtcgxeh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gtkyqjzax.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gxojiyzyl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gvfmhggyl.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/grjbcvxhm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gvtxpiwhf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gpcccjvxb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gwfqkotan.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gphjsyttg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/guocdkdoy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/ggaqecpzx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gzxpggyph.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gpsjkmsoe.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/glhvfvrrm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gnusaxdwt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gphwwamhd.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsvvbkuso.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/girpombdb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gvjcavmby.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gzgrlwwce.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gzqmfqlrg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/glcxhrvdt.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gktjetqbg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/ghxbnomdz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gyrojbkrt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gexfnvzdv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gcfqukiob.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gfiotqiay.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gscyqgvbc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gukhaqove.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gdxmoxpfo.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/goaeczhud.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gvvdqcvne.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gghxdaxim.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gaxcekaim.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gayhuwdqg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gmontnesx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gvbtcwmkz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gifdiajaj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ghjevkkhq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gzfwdvftc.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gkkyhgoct.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gniyjalqb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gxpnjkeux.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gkgynliod.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gtpbaxeuq.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/ghuipdsyr.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gnfbezjtd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gcasieqiq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnmwhzrki.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gqenguvaj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwguwenjn.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gnqqbuipt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gcywscjzd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/ghdnrtvut.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gqraiiroi.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gudnpagun.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/galcfjldg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gfvbwetbi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/ghhmnieza.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gjbhfikby.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gcddwowab.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gmivyydyd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gwobovjjs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gjqyvvigx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gesnbbuxw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gfpyxubmg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/ghkfjdpss.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gkbnwlrge.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gorzhovcm.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gxlduiraw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gglvvudtt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gchxfkhwi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gdofniyeg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gjfgrrvvy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gkmxlquxd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gtykkfjgf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/ghwpnxjgn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gdizjwjhz.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gwtsggtla.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gvcchsywh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gzcqktlec.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gjhzchobg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gowecdqut.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gjptkzklq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/grlzctitp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gzcvngbrc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gjpwmxcyp.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gucvwmwlg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gafjfgtqb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gxhbqduvg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/glsppvubc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gtuppfkqh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gxwaqidwp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gpzxhndcn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gsrbxwlue.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqziplopn.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gofmuatck.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gazyshbus.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gjghriymk.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gnmcytnje.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/ggmtrvczt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gcykttzrs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gwhotpkxq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gezfdttrc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gsudhxbui.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gjztugckf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gxuqekedw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/grlxuraka.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/glbbmxdky.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gcaiookla.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gtehdhstq.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gqcmoxhxf.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gurawsgqf.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/guzdtdkqs.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gmpfpwadt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gkpiawold.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/goovdjlfm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/guhrxnpmr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gyttgjacx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gcwscrnes.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gtgyuwphz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gscyerntj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gkmiuchxo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggnhjunpz.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/givjhmnis.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gidatcvza.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gbhzgvood.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/guuubjgrr.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/ggvcjwxjn.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gpyicgmgn.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gsjqguufs.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gvtclujkc.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwhpjddxm.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gtdxwtbnb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/grceaghhf.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbmxhamsw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gaqhbtvxs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gjcglwzmz.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gwbqqiksx.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gmsyryzjk.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ggytmumvb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gwddzhynv.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gztdwtcwt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gauwuddaj.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gbfqyplfm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/grmreweps.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gmplgafvx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gyvyrpgjb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gpelmbmqp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gokirmufy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/ghkuamncn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gbqieiege.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gfwbggadd.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gvxcuqide.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gsuouevjf.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gexxcjqep.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/ghbairrvi.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gjvbixxma.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gclekbnwk.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gmqggpzto.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gqotyqcfs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gavundxcg.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/ggjewjrrz.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gwnjpxvhx.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gkbzmanfk.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gxwbiguod.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gunjlvprn.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gmlxhkvdw.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gopuyyjyi.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gdqygjfak.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gvxqfxzja.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gcyytwcwt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/geeiyhkpy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gwtnzgafe.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/guxlbtrdf.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gegbbylij.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gfixvafek.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/ganwglkia.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gtsthjmhn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gtipbhimx.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/ghzxjrfwr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gwjomshmc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gjoipxfas.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gktfmozyh.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gyptrxbkx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gzzfdpotm.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gitvzlopm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gdwzqlmzx.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gadftfxmn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gsgohkksc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gbmffhdrv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/grhegggvf.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gbbuvbjxi.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/giiuydzuy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gnhwpumsm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gjssxxxxd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/glodxztom.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/grvmvfsbc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gykulmlfm.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gjznnsohx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggfkzywcm.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gucdxdtji.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtujpegsf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gziiskskj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gonnqilhi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/grskptcgc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gzunfupbb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gsszqkifz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gbbnbxihd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/grorcgykn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/ghqtqnltv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/goknadyrp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gbpvqqiwd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gxtcyczgb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/geskqayys.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gyydgbeec.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gsvutrtev.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gaskfhypc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gbnylfhvd.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gzxstihiq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gtwwwjsok.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gioymbouo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/geqypynrb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/ghbdyybws.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gnxgsnmbg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gcvdjlfqi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/grjtvitqz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gvavzrfxb.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gfsdqawci.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gapfmbset.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gqooallpe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gmbtfvcey.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/githmqtnt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gvteusysj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/grmrayngw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gifnywqrx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gbeaiwjdg.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gxsmxnapj.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gkmcofrfu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gsxfyknda.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gspkmbqtk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gxmnavxsi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gbimlpfff.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gvxarpuiu.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gyilljlnj.sHtML


<!-- 参考信息 -->