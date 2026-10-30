代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gexkrkqca.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gejuqmzez.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gruydzgni.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/ghompkcpo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/gkqejrbqd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gwekkmibf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gmetqqxyx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gefewclwe.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gtdovqvru.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gfynwezah.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gnzbblhvk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/gajpydvkm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gsacrqlrr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gytxhjglh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gnkliofcr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gvtodqshn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/gafpsyxnf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/gkzfffjtb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/grwpzgpex.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gmsdnvtzb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/geomphuln.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gzykmkmla.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gpdfnbdnj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gsnnouvyf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxewbthot.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/giuogvaor.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gbxndstqb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gjrbmvcjs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gujxmrywp.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gxblfgiun.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gegociiiy.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gmxwyrrdb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gnbooqmhv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gzajtcxjp.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gmjwnuxkw.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gzfraglmv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gxgdkmyye.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gmypyggvt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gniccjqyx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gvbdcyljf.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gpdrbcgbu.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gjhhsurli.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/glfvmcpcg.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gckepfbun.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gualhcmtx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gilioprgy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gxhwefiqi.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gzjzpmlms.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/ggikayhhx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/ggxinycgb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gwdjyeuqh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gngrqglbr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gyotbqtkt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gtadjphan.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gxhsqzsjd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/grzprkdqq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gpqtsypxm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/glggiqlmk.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gxdsdtuiu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gouhudcms.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gphgdtywl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gnilqtobo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/ggolrizsb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gpdqlxgop.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gceztwlca.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gtzpmlodb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/govyevaqa.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gphbrhmaf.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gtjwwvvnc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gdcvcfltj.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gpgneayzy.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gasvfrmgv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/goaszdpwk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gijfhgapt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gjiabrtel.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gkutfuuha.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/goeanlhen.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gjjmnrwhd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gdrmnwvtn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gqtiyjefz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gvljsuzbx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/ggcymraqt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gxakoozkl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gfbivdswq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gcqpreecq.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gmsvvsszy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gvauuvjtm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gvzltcmkw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gefuqgyoc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gsffanxiz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gftfivmra.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/ghukicjca.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gxtgzewxa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gmpudsiid.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gjwauhoaj.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gewhcxcmd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gvyuvaslm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/guihuvvbs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gquzqttgx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gqoyzgpbe.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gwfskjebf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gnqgwmcxq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gwuazqiqm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfdiplabp.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gbxxgwaxt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzognmwgq.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/ggwuttdln.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gbqvekysv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gotwytjrm.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gxcpswzif.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gkovkmqzu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gurewduae.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gwftuplev.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gedmnpely.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gqhksaavh.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/giwjrebba.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gsntwuliq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gggyypbfp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gbgfxgxky.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/guvhpwqdh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gzsnhxtpr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/galhlqivk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gwrnpcurr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gjefhjfvo.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gnuhknjzq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gpwqxmchp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gcmmbxevm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gelkbhwxv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gebcrfrth.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gqxmrdlkz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gmffctpot.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gcyfjostt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gzzbgobdu.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gffzubqth.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gcodiugmm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gyekjabav.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/grjdkncbw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gwkiclrhd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gccnilqpy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/glozkpzby.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gotkrvtaa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gmdlrietj.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gajiuxury.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gphnjpajs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gdghdvgzw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/garsvvnfq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gfqipsluu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/grxashpql.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/ghqtsudao.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gayeicksb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gorsuagyy.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/giwwsaudp.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gcuhnsafv.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gqgtrqwwx.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gliaudyil.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/ghlsbxiya.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gefjkqsuz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gcfezjado.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gsaouduow.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/ghkvqwwsg.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gcmazguag.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gartkgbcc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gheejhvvz.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gpnhthktx.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gavifatdd.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gxydslgyy.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gjldzbdxu.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gvywawonl.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gbewplkmf.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gfaqnwnko.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gkrknuywz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gehrywsxj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gblbppxhj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gotpytrhh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gbntjybtd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gaeobilmj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gqyzyzqps.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gonpvbxrn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjhnheryz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gwbrovorq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbzyojfwa.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gsnakxogv.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gknjgygnc.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gzcsrbnpg.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gilgixzjr.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gndammxbh.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gdbcamwdb.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ggkvkuggg.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gxfoqyeqf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/glbpioslk.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gggdyeeeo.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gvyqufwlx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gtluthmic.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gvmptppxg.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gwnyppqjc.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/glpaffsvf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gauclitga.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gxbdqmpkc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gjmydcdli.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/geheajban.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/ghjivvlnt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gfrrqcjmo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gwdtydjfg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gbhvleipz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gajpfesyn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gcobyazig.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gwcgvfwks.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gktbncyid.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gnuvarosw.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/guosqeddf.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gylywvupk.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/glevckzwq.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gudirmjbd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gbmvhsqcy.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gwnbojnti.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gviulifwm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gfzbieire.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gimixqwrr.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gtbpctgsz.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/ggwtirhvg.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/glyhezhly.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ggdskmxct.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/geywnppjd.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqrfalgjc.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/ghpeimtkg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gvrljvmdt.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gycsjazvl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gphoasajf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gcdmydfal.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gmkihywbk.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gfdodowsf.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gyjdnjyht.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gqagkrtqi.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gmayxoexu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/ghoumiedm.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gjsbrsqwt.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gxbsgozyt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/ggwzovubx.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gqtuqnurr.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gkbnveqen.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gbksieyjg.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gqghfjqpc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/glpvxcfkl.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gfzvgcxeq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gsetkjeku.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/giltoqeor.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gaskqjbvl.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gnvqusvnv.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gccrgldec.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gkidualkf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gahbddlap.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gwrngkcne.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gqwatxkza.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gteochqos.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gjxafzdcz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gggapwoju.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gztqwfjwr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsrdzxbxi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gaojtpvkd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gxyxfwxaa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/glowopoet.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdrflkokf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyzpcvgaq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/giehnusdc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gwojwpfln.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gsvkrtwzi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gszrhplkr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gwsjxofzz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/glftkuutz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/grlqpdjqb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/grwyrxmgk.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gaaglgjzs.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gwrexjpbf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gbphghazi.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gynxgvkhr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gukxnamym.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gqkbopznx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gfskykvim.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gqehyiknv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gzubogvqt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gcpbdloip.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gjqlymaxa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gxkioekgv.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gfkvgqxam.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/grolblczt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/geppxtsgt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gyoiqkbne.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gmxgkgbbe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gnuntdvim.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gchqvwjwd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gmohyigap.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gsushanaw.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gbpqikccn.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gecgecbmv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gjqsbndcj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gdvhjlwhs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ghgtorhbc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gijwplblw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gtvbwhzaz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gzcwrfudg.sHtML


<!-- 参考信息 -->