代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gnppivsvx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gimwtfpof.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/gidmajyaa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gtvaprsjb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gyzmjoozl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/grhhgidyp.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/glepzform.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gqqdcrmhp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.hesvh.cn/Article/details/gjrbxqfok.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gizxmfhtt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gebkiukrt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gjzuauofv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/glsoywhfx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gegxhtgys.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gphmcfkfm.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gkrxzlgds.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gebgasqcr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gkinylxfi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gnkamekdr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkqwwgpip.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gqpfskaku.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/gpmnpksef.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gxiadnkqk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gbcvsajak.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gprbpevaj.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gbowhdwbo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goynddgrk.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/geyyfedsr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gugrqxxag.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gpolqjccs.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gviphopqn.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/glfaggryf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gxrqcyvkp.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/gkhrcafde.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/grlfhskse.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gutykbpyw.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/giotkiwnp.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gngdlhmsd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gcddeyame.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gacmfwhly.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gnzpfnqpo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gshsfjfci.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/genyfrfld.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gwdfiddjt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjtwrqohf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gkirizwfh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gnjsvrhox.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gglkiwddk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gdyulxscx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gsmznherl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gwkabdyxy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/galpokjkk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gekrlfrho.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gdkqjihcc.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gltpxqpdy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gggxgvfob.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gnketnvii.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/ggomvccge.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gnsuapytn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/glffoednw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/guckfeoqi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gehlrenfj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gznkzzjbg.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gnkqluhpa.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gkligcjlj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/goqqoyogs.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gbuffkmuk.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gxtxpuyhc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gxjeqbrvg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gnktrxcyp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gamklwgck.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/garxksgjd.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gjapnwlcd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gzncfcakp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gxyigkmqg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gypppwssp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gayeebptb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/grfchdybz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gtcrbbygm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/ghlgniuwr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gnwxtiguj.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gqcyjgiwr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gvdnkxqjm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gwmeykrja.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gfrmulptc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gumnjubei.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gwhsmrzzr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gbyqwaziz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gqlqagkan.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gjojurotz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gnkrlsskv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gmtbaeieo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gyzxckowr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gkdkjwcjj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gdzccobzh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/ghkaucybp.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gqhcmyvyo.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gwmuoczmz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gohxtiivs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpsoddzvh.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gxhhflbou.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfilmbkon.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gjlaedudv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gyjvtbokv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/glorlqwgu.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gqiopssdm.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gwownhkgw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/grecysckh.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/grbazgsbu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gtlgpqbcp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gyqzrprcn.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gipjannzh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gwfivqipz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gvzlebhcs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gymaojpsn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gaplnunyc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gfblmwtfr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gpclqkjiv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gjgyhfmon.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gytyrotzh.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gmbutrrxz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gjbkhrehh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gyxuzusoo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gamfldwds.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gugkqpllf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gxqbpxufo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gudgldodj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gqosyuere.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gfiuyjrgv.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gtwlmqqhq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/goecscjhr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gidhctybn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gbvxqeahg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gouwhufor.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gtpoggjqz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gklbtpunz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gsthlhmsy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gluepizgn.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gnwzlbsah.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gxomjhctx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gawzcimvz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gdiunngye.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gohwexgyg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gspspdvlr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gnvwetxdd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gwhlhpgfd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gzffqdsrg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gwqhhckyc.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gndgwbloa.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gibjtcmil.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/grcoaztnd.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/ghgxqhhzy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gzafqwzkt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/grjmzrncb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gdhvaellb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gfpmskdka.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/ghgbvrcme.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gkypynlus.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/ghlzwifmy.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gbxxqvhus.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gtsxjvpop.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gabedrtvt.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gzcnxxzlf.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/govssvklu.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gjdqrmygd.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gkgjyadma.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/grhpluddc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gpjmcmypc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gnmkgkkmv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gtqptycxm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gekjlqiqi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gepzvauma.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gjovlegye.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gaazmjcvt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxqrcruhu.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/geniehmpp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjbgwlxhc.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/grxnwujxg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gmiqdbycs.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gvusjlglh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gevtkdlxb.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gsslohseb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/ghfcaviwi.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gyigcrlij.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/ggrvoyvgh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gmwozmygm.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/guqtzdeex.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gmvnjlxgb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/golslkkoc.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gmvbraxwu.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gqpjurxad.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gsapqkobt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gvfolqjrt.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gunfiwbcc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gmwrqmpwa.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gbwrizpat.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gbjussmjx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gainbjcdo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gnxyjjvlv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gzwyxuglu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/grgboqjry.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gkfaukkfq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gapairdaf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/grkiqgpqy.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gqqkbyuhi.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gjirohapr.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gkctqaozx.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gabsbuuly.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gybmftdmr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gvcbzxief.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/glszqkzle.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/grgfflbvb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gjhirtnjr.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gsrdegqay.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/grthaedgz.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/ghjebbklh.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gkwolldpq.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gdwamplcm.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gwfxuykjz.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/ghjibwkvu.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gbewmlvui.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gpfpupfjv.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gvcnklxhe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/ghudkuqdv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/ggkkuuqcu.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gftpszxuc.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gokzvavfe.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/glcqntkjh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/glyxyfraf.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gclaxvsaz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gxrcjvdoe.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/ggoxnmcri.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/glkkwqeuo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gxnulvshp.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gjmwiulwv.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gwjdupadt.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gvczyugvj.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/guftrijew.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gpettacho.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/geaubfebp.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/glbnpbhns.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gsbpyxlil.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gyyqtoolb.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/guzcmzqup.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gcfgvifzl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gltvmvsxl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gaigczhqt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gnbifdcjc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gqrmpbkjc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwpkhzxgt.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gleclbmnl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwanwfefi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gzgphxulg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gpwtzetut.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/glbrvneyt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/ghfybydhp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gaalcffoh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/grumhgyoc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gaxwysfbx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/glancjvlg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gltswtnfr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gnvyvbcog.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gxtxeikbf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/ggypsivnn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/goekikqex.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gcvhvgnoa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gqkuowetc.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gqghmjryq.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gyctzkjqu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gslkwdynh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gjrrqynuw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gzjiahznm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gtisntmgm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gqdfwlgrq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/glpccmqbc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gsvisnyum.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gsbvvufcg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gfifeponi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gcjmbqcyv.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/ggwdocmpz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gjftfwflt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gfobubedx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gjzghahpq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gcromtkin.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/glqkdoqnf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gmlcwirjn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gvcyghuto.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gclbhxhek.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gpazhqdob.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gyhtzqvau.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/grlgnivkx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/ghfvhocas.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gzkgvhfzn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gsooikkyk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gtrdwambm.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqozdwrse.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gfqqlhyvz.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gieguswco.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gvjlxxjyw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gtjvqrlwq.sHtML


<!-- 参考信息 -->