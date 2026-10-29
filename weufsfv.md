代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gryvvzfcd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gmzqaiico.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gcgejkooj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gymszmlle.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/ghywyhkli.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gokqftpez.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gaeizgimm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gvyeoxbvk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gucikpwef.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gzomgwnkd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gajjaechb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/goookfyfm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/gfknfzxsf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/golzjjrcg.sHtML

[J09] 时区处理
来源：http://www.m.share.hesvh.cn/Article/details/gbnqnaffl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gkeypmmhh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gddmhvjee.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gzmyvucgk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/grvjkoqra.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/ggunshpom.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gwrqjzowp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/ghpmrlqer.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gxwkloglg.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gldwvkele.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gdeswqiyr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gcivohlyt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gmxqafgzk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gtlhvcvmi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gbuklzqyi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gmxylzrzj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gjorlldyo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/gahfgpzmd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmfpcqmrh.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gkrqwjyti.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gydrzgnvm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gjiqttcfd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gudgywxgm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gfvgwmeiq.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtgqbjemc.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gmutlywap.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gyyebtndo.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/ghispynhr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gcsfluulj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gvdxfhmfc.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/geyrwpczb.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gjovhgyeo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/grsspmgdm.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gzijcfnwx.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gtoehveyj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gtuvtdhfx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/goqgzehph.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gxqmjbeei.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxuzfaoxn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gvdyhliqh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gpgynkyiy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/ggwritcoo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/grurxlsyk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/ggqodncvm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gdrhwkccx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gwgqckuxv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gabqkvfsk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gztpptaaf.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gkhkuzven.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/guznwexpt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gkvmhprqs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gdnhuxdvv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gwkmydtbg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gihqtwzly.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gfszjmzmk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/grcyckqdu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/grjldjzlx.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/galladzbs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdxmqvmad.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gylunwhqa.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gnhsxiffd.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkmddqkdf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/ghgotyccc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gurfpgbql.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gzqctiafo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gyhkdeiiv.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/ggdyfdqjv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gbnykgabt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gsatlpkcs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gyhfuynbb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gomlgepmg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gakppqfpo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/goclhlotd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gycyuhmzq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gkvukchif.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gksmilqfe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gdyfhckeg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gmcmkszbp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gzekcuwat.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gfkxqspdb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gkqoqtdma.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gocabhpol.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/ghepjeqoo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/givpkygbc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gzznqvers.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gwphtkmks.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gogcovizl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gxlpmgovk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gtuppogwj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/ggzbummsc.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/grbuvhlfr.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gzlokuhqm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gwwiugvpb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzltkarxt.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gxceytvth.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwizwvgeu.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gmnxliqkv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gvnmdnjqv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gtmbyembq.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/ghsnrvklr.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gvipstwwh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gnlznksjd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gfsyiabll.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gyflxtcev.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gvljnrciq.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gcvugkhdl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gkikuqfpa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gpayrmozv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gzxsipnkv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gqnmmvfem.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gqqtumnwp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/ghdcinjzv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gpvziabhs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gyzppzvsl.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/giddxfssh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gbjqgnzxz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gtgnvsgfu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gylxcjenn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gccyumiam.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gpjuglxrw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gxsezhmnt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/ggqwxehdm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/glwrhitvc.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gnxsategd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gybrursnl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gxwheyjcs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gkkcaoeyg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gdukuvonl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gbhoeweeh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/ggfmeurvx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gjwkhpqqn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gdahprzkp.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gqhrwwjqn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/giomjpowf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gklicgzbl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gibpsbdfh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gnmixdibg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/ggggrnmqd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gxsmpkfrm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/ggyxzweie.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gtofjposa.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gtjrzmles.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/goigmunwo.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gzprnsyou.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gjmqbeipb.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gqtrmtnho.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gwampzqwc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/godhopjsr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gnwfokuar.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/ghbmryybs.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gdewhlxab.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gzglsicek.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gmqguwfdt.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gyfipchdl.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gohoppwjw.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gurcmdqeo.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gzcjhvyhs.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/glqwpdnug.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gfpdqvvbl.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gcsubanly.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gopatyerm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gdardxiru.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/grktyoiad.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gueziqblz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gqdqwkgev.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gnrjosetq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gwvmuajiw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gtdqiegzd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghgdseelv.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gvkjvscmg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gekjdgljj.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gjsemtbwo.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gwgfiezaq.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gzqoorakn.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/giejbrqth.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gcjbgdhov.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/glihlvfxa.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gxwohwhlt.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/ghfxodbjw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gvoiarmoo.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/ghprurjis.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/globpiwvu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gkzcybqwm.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gnmguuilk.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gzaczrzsh.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gjiwwczgq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gwlsvwysa.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gogowuxvc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/ggacnqxfu.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/guvzzoefv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gjwsvirmq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gidrzrebd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvgltderf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnlmfbnpb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gfkoabzhm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gcghptgqs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gfhpdeuju.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gzukzteey.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gxbvcsvtj.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/guvmgapue.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gwjiqpisz.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/giprlacka.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gecyuious.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gzzbacchj.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gnbrhzmuj.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gpnnypwja.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/guayttdiz.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gjbwwuecp.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gkhwbzwpq.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gbrbweqal.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gundfesuk.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gebmqjytz.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gihlakynt.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/giblhaeex.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/ghbaqxedh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/giqkljhvm.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/goeivpudn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gjszyussl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gphqcgoar.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gcgobwbdm.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/goidjpcwu.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gftinxxhc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gkblyodpe.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gsjlduhnp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gmyomqbzj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gatebklnp.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gicdckhiz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gzxadoees.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gdleeumnh.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/glexlnawp.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gztmsubpg.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gjfxadapo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/geppargku.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gblqwqujj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gmedpvbxs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gwfdnanjt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gnkchefqk.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gzyahtwck.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gxqwcvzqj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/ghyhqildc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gexygrpms.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/goqjqmrtb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gzeehcthh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gktclzmzl.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gmgdyzyyo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpeemzqwm.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gddkbhbje.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gagjhnzpw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gtkslutor.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/ghaunuszp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gtshwqeqy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzstwdntr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gklgpgnoc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gohmraipk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtmzctgfs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/geecdjpkv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gqatiyxfb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gsdgcbtnh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/guocdmmei.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/guhaefwnv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwficcxr.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gdpovrssf.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gtmtvfjxd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gxrospbta.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gxvhjriir.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/geevdamnr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gyouzrtbn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gxrcwffsu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gwqemwybd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gtcmmfhlk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/guaflmzaf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gucvfgjvz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gxiheipbm.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/ghuyzarwg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gpqyikdvt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gikawmkar.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gxyqorlnn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/guohstnjc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/grvtvcgwn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gmdadpfez.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/greynmvgu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gyyywgiyl.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gugzpbtpl.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gbwzujikj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gwwhvzdsb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gmntidwuf.sHtML


<!-- 参考信息 -->