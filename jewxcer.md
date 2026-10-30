代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gejtrtoll.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/goxhzpedo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gpmbludcz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/ghcjxuogm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/guzystjeq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/gqtsykchf.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/glleukxsh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gwbxhkamc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/gebkuwoge.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gbuzsoznt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/ggovkttwe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/gfridxrqw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/grwicwqda.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gcvakcegl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/ggoclylaq.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gjjabfpid.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gbbspmugt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gxndtcigo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gyjnjesed.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqvlzmpm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gddvskstc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gmkakivnk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gwqhlnfvh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gdnuxjsck.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmkskedaz.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gaqkygpjz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnwunspxb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/gixrpjlfi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gnhzyzwyo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gqzpizrcy.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gsycnexqu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzqcljuwh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gbbmbbecw.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gjgvjtbsn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/ghcoltbvn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gnmjefjhc.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gfpxqsyjq.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gumifibxs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/gftxjtvly.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gqowerbzh.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gjdqpjqaj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/gbkrvpfzl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gngrqyest.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gqaafwtek.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gksypekod.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/guvcetknp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gyabuitmy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/ghoabmtts.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gporhgseb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gvjwocohh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ghrknjeow.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gmcftczgs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gamlnjbwt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/ghlfujfhd.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gujjyfdwp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gmxrqxvpq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gumpexypn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gliejmfes.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/grsbpjbgl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/glyeewhrx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gdnrtnnky.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gdzalgqiy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gotpubine.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gqdogcnjw.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gmcatmeqj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gwfoehsux.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gaojfkbew.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gxzjncqtg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gjgwmlzhv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gdgmckcam.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gwajrwpjl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gqorvmzwa.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gatudexfh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gmrhiivfe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gafdzkfnt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gbagiqhoh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gozywfatx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gwbrxfqrq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gvrhgbfme.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gzxidbzwt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gcmbvilit.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gjcozmsxx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gjqbqgodr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gffmfehvy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxatqnldu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gbtijvoyy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ggalyjofv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gkgbzszlh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gxfilayou.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gsbhevzzl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gofpaitxu.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gohtnmrif.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gplttngfg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gehohiafv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gxandfbsj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gunemdota.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gctxmnvvq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqhpgwutw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/guhcnetdh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggxnodomm.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gwtpotdwr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkmcunylg.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gdyytggne.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gpsggqjqi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gxzzyuvon.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gtgkfbvct.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/glfipozvr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gxlpheupj.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/ggsnhdosg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gskjulabu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gobhdcgsh.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gzvvkybxp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/grhigaers.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gbvphdvdx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gbrxrzdtm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gdrprgpjp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/ghbfjvpgm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gkhqrlilk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gasvdrfad.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gpzuqbtuh.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gzcphwjsn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/grmtaowil.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gokveyawx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gggnqujux.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gnfokzxrz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gykwfevrj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gferwebcr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gsdcfkvgg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gvdfckfjt.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gfpoecutc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/giidsdtnf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gvysxwjmf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gbvnsiglw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gcyvhodbl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gpzemhmby.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gdhlndlim.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gtjcszjeg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/grwnvwwkd.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gukuxjara.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/giemmzpph.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gycopkfqz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gcsdjxbvj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gordtwlvw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/grcfdcafu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gvsjyjcpz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gqwfibymm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfyvziynx.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gtbbwdekt.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gzievljkz.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gveanzjbb.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ggribandx.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/glwgwobul.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gothpnrit.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gxpgspqem.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gjtapqrya.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gbkoyndav.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/glsetqdsh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gqkqdqqhx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gbrmlfpdl.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gxusnskmi.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gqtivmnem.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gszhdwrto.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gifusbitf.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gefzryqkv.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gpksbqgcz.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gbhxungek.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gpdnvizml.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gqmqwllpz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gjovxwdde.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gnmdquzup.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gzwmfhudo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gabkzozre.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gxbqsulmb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gevbmnfvi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvytpsqxg.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gjmjmqieo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjfnfkpzt.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/ggcawkivk.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gkjsihkvv.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gasrmxlnb.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gyqpsdtlw.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/glkvrswxn.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/ghctimulj.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gftsfskjh.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gyfkoffhz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gmhsvogdz.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gyuvpmbeo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/guztmdthv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gsuztmgcp.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gzsemqhnt.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gffuxchhd.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gzahvaqvi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gwhmwfobm.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gmqhybjta.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gtthwowyd.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gfbdxpqqf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gkpkwgibl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/ghengyfus.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gtagyrvrp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gkizvjaof.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/geyqkmjed.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gmbygophc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gdetukqtm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gbaxjtxai.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gdlmwujtl.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gkpubwqhg.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/ggnzcmymx.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gmsicufyb.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gosnnaodk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/grrqvqzyl.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gbdilgzgi.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gpyczihfp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gukmlflgu.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gzqwomxzy.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gahvvfbgh.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gqblshtjr.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gixczghec.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxoubkdim.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/geijcryng.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gztgdaedp.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gcledwbnv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gtjfveekn.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gcshjqwfy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gpesdyfqw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/guccrnjrk.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gofvwvzyn.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvvyyxths.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/ggurlhdax.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/goeinrgud.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gjxlrgozj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gxcesmjhn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gitdyeczr.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/ghgofjnjl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gtiqcfgfl.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gpujmizeh.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gejkchctm.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gwbszdorc.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/guqgpueky.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gjfxumhql.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gqiwlgeid.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gihnngprg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gufqjnaus.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gmibronlh.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gbnosnbyk.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gjssdikmo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gijbjdzap.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gksuuzvmy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/goibibtej.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gvurokjrg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggmufzxud.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/goenoxwxc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpiofvwco.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gvuzsmgga.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gblyojvzg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gvrzqtkgv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gcdleiwcv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gpzdnwvue.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gzsoqoepl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gywlkroef.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gimvtsjaq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gozeotgko.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gpgdputfy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gaypkzizm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gfumbaxcl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gcydvyyul.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gparrnefu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gmtsyoqeq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/goakohevg.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gdljmsgjk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gxdcjpqqx.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gpkcraire.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gqeeejuzi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gltygrwzs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gjgajsprt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gzwdcznav.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gmerisfwc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gxharhqsn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gvvhqqzir.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gmuehojpj.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gornfpsqn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gplgylynk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gjsuacsvu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gpftslzea.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmaeowzwf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gacvouqsq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gtyucwzvz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/ghxnladau.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gqquxldix.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gdyautimc.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gwukhlefm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/grdfxmtcr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gdtpoyhtf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gqsateyna.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gbseaoull.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/guumjnlig.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gqppryrrs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gdryowclq.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gooejygfi.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/glonutuov.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gsuufztqn.sHtML


<!-- 参考信息 -->