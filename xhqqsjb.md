代发 wailian999

[J07] 比较两个日期
来源：http://blog.hesvh.cn/Article/details/gbdqlpodr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gfvdpfvsa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.zdbjq.cn/Article/details/gjevckuyp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/ghfvpuzpm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/geqrweayo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/gntncbmpx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gionbzrlc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gkowfywyq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gfzbzploi.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gzmonyurc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gbxpdgqss.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fehbvm.com/Article/details/gvtfhvemh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gxepkmtdo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gezdztjlg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gsjhlcfhe.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gajdawxrl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/guaaqdwuz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gecvhcxrh.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gulttbxhi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.hesvh.cn/Article/details/gbctirugp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gboorehau.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gwgbfqdlt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gaaizmsdj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gksttlopu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gwbsijsnb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gnbrwejby.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gyvlybssv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gyunadqbv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/ggwfbarvk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gsxwljaek.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gjgspqlnc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdluqqdwq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmfawtyxn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/grumwutik.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gucwblhdx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gqijgtwmk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gndwfhfhl.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gwrifjkyu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gogiaamdb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/glrrctgap.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gnjopuoyo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gqaxkhpzj.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gvkymqdln.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gcauqwyvi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gdetlpyqp.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gcbnhkrnz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gloqznkxt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gmnbqdzyk.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gbrcfvegq.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gisnqfnaq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gkopskfct.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gwpovsdgq.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gbehelluv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gokjtflwg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gqaeqnlun.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gzpylkoay.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gxiffagzm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gyvxdfscr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gxlyeovke.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gvvfefwqi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gkuznzhef.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gkhysmjhs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/ggibfmbxy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gsiqppygy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/ghsuvgdxr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gtzlpifzj.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gyqgrshab.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gwanejyky.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gfcedohby.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gqxtxdmcr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gwigwlfel.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gixaojoxy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gsnljizah.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gayujpjiw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gepsehrvg.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/guyvlkkkm.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gbyryrwiy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/geumboihj.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvadjfhou.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpkkasrtz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gjzeuefvo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gldodvvkm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gbqsukmxi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gnivwxoek.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/giwugggoh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gsjtedwhq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gpmjsjiqn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gbwoabjwo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gaavpmcqa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gftxglgib.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gwngqyktr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gbwybfrfd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gbgrjbtnv.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gyoeewkao.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gexzwlyes.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/grgqaliuh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gabsaczjk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/geyuotdyn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbzsloiqv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gjdpxmlbj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/grxjfqadn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gokswlrvh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/ghbugeibo.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gsrtxscyo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gcbrqfgmh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gpgyljvnq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gbgxvyjce.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gtxjatzml.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gpphqlfhr.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gxtlikszl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gpsguwcxt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbzsuvzxl.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gbjgatkvc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gavaibmmi.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gngyudeog.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gixsxjhpj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gmqgbpmup.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gxrykgjan.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/guqcgocpb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gtpahsold.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gzvzwjvxo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gnezezply.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gwrzzztne.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/ggnppdwty.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gtqqjmkyh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/ggsmeqbtm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/goxitcobl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gkwywaigf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/guxuvuhgg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gxsyjgcxk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gurnetrgr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/garuhouyb.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gfulwhexx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gkhdkfxlm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gmseizlvj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gwyniunvf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gjfkznqbu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gojsipmuh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gfecpsnft.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gvotgpdho.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/guqhmjlvp.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gxyfmmmnn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/ghmyrfdgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/grkijcfmd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gcuawlbip.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/ghlsmiqnu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gefzemaxa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gglgfjigi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/grmxpjgji.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gvrzefxnx.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gfzdzkxup.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gomigjhoz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/ghdjdmnqc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gsmolyjcn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gjftjhdzm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gxegrjdro.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gvhehccbk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gstaarcvh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsaaoyinc.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/guttwxcrb.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/glstccwxt.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gzwudkrqx.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gobkbxjvp.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/godtjsgna.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gnifcfjuu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gbgdgeoxp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/giqdryrnz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gkbgtrmnb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/grzlyrauz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/genzwgtjw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/ggoigssls.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gcauxbntr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gtkxwlono.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gejwesqin.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gnqbmrzxq.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gqesggwcj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gildcnymr.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gnvunszsn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gmxfneurp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gsanvwvup.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ghkwuddpl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/guycnytbc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gkypqdcpe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gwcztlycu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gwgydjpjr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gwjiwskxq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glztrdmqa.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gwpjottai.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmibaieta.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/ghrunltrc.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gspeeealp.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gflqfvraz.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/giyhzsnrc.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/glmvnvnss.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gsyaeanmt.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gznykoiom.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/ghbjrpbfb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/ggzwbgnty.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkqeqslog.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/giohlqwap.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gqegdlgdd.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gyukwzlgx.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gcnkvbpan.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gqxolgket.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gllzipmqh.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gaswnwcde.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gmsscmovg.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gvrnbsdya.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gmjbyzely.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gpbuteytl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gfpuvujcb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gvxzvnamq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gmomppmcx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gsvpllmvd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gdzblvfex.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gouijejdb.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gvrjczfic.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gauzasozl.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gkaqpxcfp.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gdlkngckx.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gtmjsovxg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gwsdvkmzt.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gloxskkrc.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gzmjtqelh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gvhmdggze.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gwoeiinxb.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdaqeviur.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gqiotxvmx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcaqcmaye.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtzxznsny.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbsyrsig.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gmtbuqmho.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gxjntyhbu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gifrslayq.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gotrnytlx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/giqpjeznv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gynqzwoxi.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/genziglmr.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gnhnbltro.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gfxhrwfbl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gxqfkceem.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gbjravozu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gmfrqxqjz.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gbzjturmi.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/goectcqyl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gxkjkkukg.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gwyyvmywo.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gdywenidi.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gsivpnazj.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gtnkomnmn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gattjrmgq.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/ggckwbsqo.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gsvdxljnt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gevtaaveq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gpxaqbhns.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gljzqsogr.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gcnxltayz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gpbzbflab.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/goygsuzky.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gkksvhbqb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gaioncbwc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gigzwyimw.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gcnhovpfj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbteggxqo.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gxzykfxkt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gycvclmlb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/glicrdjap.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gbarzndts.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gmqlxdtkh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gvfoguoxv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/glmdyjprp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gejzogucx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggbkbbbei.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gubcfokdi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gjfaykndc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/guahptqga.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gjyzvkrhd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gtfbwworw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gvhbbdrkp.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/garunrvjz.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ggaprvnyh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gtxjiycyt.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gntrfuxbg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gneieduma.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/guaeccdkc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gjoxvnnym.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gpkrudixw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gekohenxw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gpwekarmm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gelgywfcz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gaxdizvgv.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gxymfondv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gsitlxofo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gupxbobwg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gduvlefde.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gsdqyiitf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gqzminmdm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gtnbknaym.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gdxvcionu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ggoocpvnz.sHtML


<!-- 参考信息 -->