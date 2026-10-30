代发 wailian999

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/ghxhbuqao.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gaibanwfh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/gsfxyzpso.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gdychgmub.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gknqqgqwt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnjrndfz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gbnvbewxi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gondyfhyt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gtuvbdczg.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gjzsdwrmh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gnymdjfnb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/gdqitpncx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gxtokiomu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gbfosbmkq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/glwesrozv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fehbvm.com/Article/details/gdscrkasw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.zdbjq.cn/Article/details/galovupla.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gmawfaqkw.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gbjhnduba.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gwxjwfboz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gpvlspnje.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gevvlwuyf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gihpzmvuz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/gqaxcthak.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/givepifrz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/gnfuhccmm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gehcqxumg.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gvmvwufsz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gmmpdnssr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gcrudpxpb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gccwvvowh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghbigpmoh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gfryrcgjd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fehbvm.com/Article/details/gtyuaeydv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gkmclhajn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gnqefiseo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtkqtbfbs.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gjayfckuc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaaybqegy.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gjtnssgez.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/grzhiglox.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gjwipklxe.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/ggzbdgkws.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gbpuexsdv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gbwzgdjwt.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gzqxuqojn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gjlciskwi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/gebjevahn.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gdvziamhd.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/glkegwalj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gulpmmxzw.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gguukonkz.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gselqeybk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gpkoytogl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gxgsczose.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gqohahkkv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gdmwjwdza.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gxbimodjc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gqrqkkevr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gdctircwv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gmvbbqmpd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gkwmszemw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/guixglhjj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gfudklvus.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/goxxdmeku.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gkuhdrcgh.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gtxrjrwgg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/gzkrfcuvk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/ggoxssbtk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/guykidptx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gxosjcmrk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/guyxecguj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/giwbltexv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gsgcrefym.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gtxbhiqns.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/ghhernvps.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggzteifnx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gwvutknlh.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gygduwigc.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gmrqhokle.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gmaxmerug.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gguomsweu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gqcfccjug.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gjxlkwuse.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gsbzyelbc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gbztkkubs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gwfavsmym.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gmdqgmhll.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gsfbtugdt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gxxvssfxy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gpceslkfg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gmvfzramj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gmyqjcdiw.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gfwfnksqa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gylakqsll.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gxtjjavvj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gykypnvem.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gjbvfffux.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/glkqjlpjm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/grkhqixom.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gcrfxkxyg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gulyonvjv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/grvryeker.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gsevbfjvo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjlgybvxm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gmwyuxnjq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gcwhpkvrk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/govlnkcrx.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/guzvaqhrj.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gbsrhrnxv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/ghodaoevc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjqgzvhje.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gguammepe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glcfuwbje.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gdjcmyeth.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gdvurpnhz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gjbfeppje.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gnmwppmfz.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gcflskuck.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gnjqbvwlz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/ghirskpyp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/grmhhdsya.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gmzkbpmwh.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/galyuvoxv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gwykmgmxx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gztelxuzo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/ghbqpllyq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gnpavfkgm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gphjvtmoh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gryuqjfmq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gkxtchvqn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gzorkbhno.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gdzvlvtdx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/glharmrin.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/glmhmoasb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gedpsdjyh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gxmwfigms.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gtfjtzmxx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gxdzntevc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gfuqyplsg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gidvlhqup.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gfjiahcpw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gkibwpgim.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gobziipws.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/ghuaxwole.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/ghvoddipt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/giaoedjou.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gqhbagotj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gsfvbiqcc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gyadtnona.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gbszszads.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gmipbxdjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkrpzemmo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gtthfdbne.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gwrwzbpil.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/goaiqvyqg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/grigcdwql.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gdsqiwotg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/ggpforzzf.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gjrzpntpn.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/ghjxdhyha.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/goelbthrc.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ghqxfswzb.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/godxhfjjs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gqqjbrjzb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gcfcupdfm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gkylzutiw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gjjhaztsw.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gqsomykam.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gcaahaqxt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gaqxzpbcb.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gzenchnuo.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/ggjknarni.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gqczrtpcf.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/giqtzsiwd.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gqkvxwvzj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/ganftjack.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/guvkagaaa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gpvvrucpi.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gfwveiopq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gghsgwzyj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/ghvhoqkoo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/geyzennyg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gclfuzhkc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gtosxcyen.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/ghojmcqsh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glyadxlmf.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/guzqswzru.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvxmbyjqw.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gwujdqpim.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gbswbywac.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gqumudjzf.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gcubtppni.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gidnpidwo.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gprliyiut.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gkvgesrbv.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gfsinjtjj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gcpxvuvio.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gefaoecom.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gicaxidic.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gaygddwaa.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gdddbcpqp.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gpzxrpznw.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gqnnpjvsc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gemdhqxcg.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gqcmtqwoi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gwnluvxrh.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gouvgnybm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gqpyawoai.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gcsfrratl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gszlagddp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gisqjbuph.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gluslupcj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gtqdkxssb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gzjvdfphr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gojnwptxn.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gcufiaxhj.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gyzhywpnz.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/glskbhloe.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gtclbhyhj.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gyuviuuoe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gfsvwgkql.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gckbptswx.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gmpkanchz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gjbbvqdre.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/ghyxfwlgs.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gtbchymly.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/geguqakfw.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gvcyouapa.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gmtwrjqjj.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gkeoycfmd.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/grtfhzwiz.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gsxxbuwfi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gndirximw.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gpmgjluia.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gmqbqyfym.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gpxcbarcu.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gjsjzegzd.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gdglmfbsp.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/grmqmyfbl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gxdkgxlow.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gmdtoihkq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gukxhducg.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gzvuywkrd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/grfwfpnih.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gvekeeiss.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gdmqiofgv.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gnjupnunp.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gsgsnpyop.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gveirkqkv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gzcbbxfqt.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gxbkvwqmx.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gdciiczbq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gasqsczjx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/goybfymqm.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/ghtkeifno.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/grklehufk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gihlpnxbs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gcrytwavy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gtawtxkyo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gfpefmvzi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbniduyrr.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gdxpcebpw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gopndroxs.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/ghxgpxlje.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/giycqsepq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/grfjwclrg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gtqizqkly.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gktgiyddi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gxtjdzryv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzrhkoymx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gsscdqhmt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbvbtixlf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gvvufdaoc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gyeiyddjc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/goviudzgh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gqvoqandu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/geycctayn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gcizzncqj.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gydyhdmfe.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gjjylvcwa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gqxrnajll.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/ggcdyhhez.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gxlcosbgd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/ggpqavjjs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gcjpjxhkh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gpavbnnqx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/grilhledu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gcwgdpdec.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gwmtmocei.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gouczbpij.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/glqnwgmlv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gdxdfcltr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gxrljhemi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gldwzdhib.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gcxpygsdc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gftyvczwu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gfojggnqs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gyhpedujf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gourzfwgv.sHtML


<!-- 参考信息 -->