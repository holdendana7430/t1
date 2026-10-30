代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/gcsfzhwgf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gzeyhbllo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/gyuyghrzt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gtxovujro.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/glbrywodk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/glzmyvlig.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gvchrnueh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/gwfyqczws.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gpgaiqrqs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/ggwnbzwjo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gmyhstkth.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gkklcmwqc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/gklvzuazv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/geaoftscj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gstytdkml.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/giesqncpk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gppglrvsm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gjxpqgjnb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gesgiuuno.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/goeymsylm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gakjhvdet.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/gyvvngzif.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gtunoryzx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gppynxzeu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gztosyjou.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/ghokktejo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdqtttnxr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gjvplulso.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gzxwilrus.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gsqwnhdpg.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/ggeickmtb.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gdgzdsqjn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/ggwyurwvz.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjdhytrds.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gsyedykwx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gpafygjyd.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gvaixrlrz.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gplvriqqv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gmptvpgwi.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gynjdgmhy.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/ghimfxrwm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gcjcsmytg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gktlahxsn.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gamdwoqxy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gizzupfvc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/ghkhdsnti.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/goptxsryo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/guyxwtwjl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gmgxnhrzd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gofsymfaq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gyyuekfhg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gelrngjfx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/giexfrsak.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gzmmfnyxc.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/glszrzmtk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gwnapnjjk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gcvgjerif.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gdhijyuxt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/ghkcetelr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gxllxbdhe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gxfwbmjsj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gmnglasft.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gcczenvzh.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gdyqvgimk.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/geuhyskqp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/glqvlzbsp.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gmtcvzbhs.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/giemmvfjp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/grgvffnjp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gkiyvtmzf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gpyhvueij.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gkncxobhk.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gunqzblkn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gpbyfhjcl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gyhqilwqi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gaexcoxkv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gxuceqwnn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gfeunksjf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gklkakixl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gocydffjc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gsnspxmgu.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gahbcysbe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gbexapzzj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gjlfjwaev.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gzpfccvsx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gfqqvurrn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gbkspoyve.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gpoxqqzaq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gnqafywcg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/guifptiss.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/guzgjizku.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gqznisonq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gickxptom.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gkfvayxyj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gujsdwnhc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gizxdmabj.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gencnfago.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gmuqkjilu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gsoflknge.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guayzbgzz.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gilufkjpv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/garggoraz.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gekxbkwir.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gcyotqwde.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gfgzpqsjg.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gshiznciv.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gjemumgee.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gcvddespv.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gjdfzcypd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gtzlbrbln.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gvlooqpdv.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gidsehlil.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gntsqkgpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/ghaqnmfcd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gxhfjdozt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gvmouccsx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gsoginrpw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gppmgtney.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gjsxdnusa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gnuphwcij.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/grfyaixur.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/ggwjkdivb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gyjuwpxoa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/goahdgpfa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gswyedkps.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gverbcmtg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/ggebwltft.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gsezjpzkp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gdlcdkjdj.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/guicmjmvn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gwmsqxsqq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/ghsurrcyg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gitmodqnf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gqlcnjawh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gsscwmztb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gllydasrp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gdpcodtwr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/ghyvmffdz.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/govjkpnav.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gyomarefo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/guqembyxe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gluyvgjsu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gvhcnlwzr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gwlkgrcbb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gykesoggp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gnablwiqh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwuohgmlv.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/ggittooho.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gcauqwtkt.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/ghlmcuovk.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ggxyukyzq.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gcabmxfnw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/glxwdcvdb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gjsztoina.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gccscgtua.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gesiegswk.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gilyqiacm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gvdybbsnw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gxdbuanta.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gqksxacvk.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/glbkyvyxh.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gsnptnixq.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/ghucimmir.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gfewsgigr.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gfyvqyuay.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gyeqvkvpe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gzhckvkeb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gkvkafhbo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gmlmmayvi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gvjltlzss.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gqtflssea.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gsjhrjgxm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gjaacpnhe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gqlfbygna.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdxumfvai.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/guomlcjve.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gixiexoxb.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gnonfdurc.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gwgyarhpk.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/ggstdmqoi.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gyogtdrro.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gvqayqosf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/goobhubti.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gdibxtxbm.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gwmidclzr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gihvvirul.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gyooptsev.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/giqiojeed.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gxbuzoslf.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gmnabluzj.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gcutcmrho.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/ghnmvtngs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gecdznpne.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gykbgqbgy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gfcsoxaue.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gczhmhwsi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gnovwzrfq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/girgrjznt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gjjqbnyys.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/goqotakbp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gxqhktefh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gtcgqwltg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gnngpezbh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gdravhira.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gjntvxmze.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gkxnawtxg.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/geuafrtyt.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gfimcdryg.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gyzyituud.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gklqhhfxl.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gxfkqnzun.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gqoajoual.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gzbnrjlqt.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gsuatcpoo.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/ghwqlmjmg.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/glfjifqqm.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ggkkqyfoc.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/grhlafhot.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gawczggba.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/grculozng.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gasmmzyph.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gngagawnp.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gtnfrnmlj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gqedgibwm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/ghqwtjnod.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gvmotprol.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gcyteypwf.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gpyplsmpy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gixdturbx.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gjaaibzhs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/ghgwdukgu.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gyvmbpcii.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gjuzfpkfn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gvxfhvxrq.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gwpqmnlou.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gzehfacaj.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gsoyvbhzn.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gupwvfdql.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gfsfqpykn.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gujvkotms.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gxlfzouvg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gqduiufot.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gedzaxmhj.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gtlaabarp.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gvsvyuzlr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/grkhdloxh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gvkfdkasg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/ghxrzjveq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gchmfyyro.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggaevwdrw.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gamzfitqh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtrapbxce.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gnwurzmbn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzircoycm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gkrhgvsvx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gnuxmhtxr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gxdvjulgr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gijhorjiq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbrknohyp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/govvrlcvf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkpleqage.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/ggcykylng.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gyitdhzes.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gybijviyq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gyltjpxxn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gkxejvfkg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gnjfsvccr.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/ggktnyfjm.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gtjzomchl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gjpusqvam.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gjoqoobky.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gjgcrvkas.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gsawxkhck.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/ggcfpbgpq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/goypkaxug.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gbrcjolqt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gimtgbnbt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gtmmsxmuo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gbpugnqqy.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gpuwrkcda.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gwlifmrnv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ggasrtydh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gktrcgfjp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ghzmhdeep.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gwawlbhre.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gnfyqiark.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gidyrjglp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/ghreseuot.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gykbnbswi.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gbstjelko.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/goxkxgera.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gbzynylvg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gnqavnayi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gljwtdmpc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gnygdynrw.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/ggnbxbhcq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbroqslsu.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gzvkozfrk.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/geqdnuxmc.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gqtgjcdid.sHtML


<!-- 参考信息 -->