代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gnoqxatcl.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gxsripeyn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/gzhbzksii.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/glcyrsgvn.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/ggeqtqyeg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gomkyeayc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gqvijdmpr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gmnwqugqk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/grzppnksn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/glanumrsr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gslghzvyc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gwdoqvhyo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gfpzyjlla.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gdpwsoqxo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gkziqgwbt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/goglmjmnj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gpjbgugss.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gzpbxhzqm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gpubqxfga.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gxlpyeigw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/glzavuoxs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gjhxzeziu.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/gkrvszssb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/grayirokc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/ghzjohrsy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gaquirfpr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/grzstqydk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/gexyjritp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gzyespjie.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gmvwopkuj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gbxrcqlvv.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gssnxxpoc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gcbiamzvl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gwweflvav.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/gzydrwluu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/grylklbwq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gajfnjsdm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gagrummzz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gzwsvdbqn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzjkyyctc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geskxvdti.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/guwyxxcrv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdoiqelab.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/goyvvkbro.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gleuzmric.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gtwwizxio.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gsfjusgkj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnwzknpsd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gultfyozb.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxxomrdku.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gsxcgqdky.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gqciepsha.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gjtumxyue.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gtahpxtmm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gecnolnwl.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gywupgxdi.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gmqtrkqho.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/gqaovguqc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gwhxbnsbc.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gwhbthpfl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gqyejquhu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gtgbtzibb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gzfqpmhuv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gipzajwmo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/grbshpvab.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gwvagwtbh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ggcictbli.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gdbjhmvdi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjcgumruk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/geaaobduu.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gknlsuqcc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/grcezualh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gfbjvzfma.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gznuryuma.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gyyiriifo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gkrehglqo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gbuabqefc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gaordkrxu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gccqnkrcj.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gauccgysl.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/ggfpqipxj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gdfccqhsp.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gchzgxxcm.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpazqphsc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gnqdzbpeh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gqhyqyabh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gdklyxpvm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gsxpzgwjt.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/giigqvamt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gwjaidwqp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gffdscaeu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gzdqpzznk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/ghhjgbysw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gprxlvspv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gedbdaouq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gmihbmjpn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gsqkaoqpx.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gvnwfequq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gwipljymy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gjbdchrxz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxeschesv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gcnytruxx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gvdslqiyb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gzhbzkjgh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gylqkvbsi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gcytamzys.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/giluyxjzo.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gmhlgcbgd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gmwrbzkir.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gzixbgcfc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gnxgtrsuh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gstsobvfb.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gkeihaouq.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gedvympkm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/glpqjqoop.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcfwhcoga.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gqajwlnfd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzqceyuet.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/grxisycyj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/grqumbyul.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gcvpzpqlx.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gnvgardct.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gxvyvasul.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gkhmmsyjl.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gwubqosex.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gfbpljndi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gzmkkcbxb.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gybbqueka.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gmtmgtsuk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gbzhcnamq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/ganerasso.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gvrkvjudk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gjkoiltpu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gyovhmgvt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gxxmbaumg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/govrhjtal.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gaqkjukqi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gajrnsbtw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gwjtjioaz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gjeoogvyl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gkhmwdxer.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/ganegaxwk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/ggsudhoxi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gfaidqxqn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gkpgleayc.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gvinhesro.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gvmftzytz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gxfmsbpxr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/ghzogfdku.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gqgecgptq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gwxawanuh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gcdpxpuah.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gxosjwhwy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gwwnwhidg.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gnftaqqbs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/guwzilmnt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/guhiyssnb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/ghphdjcdx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/glhpzhyus.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gdszddjtj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gzcwdrbdt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gikeevqvr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gcvhreoch.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gnlzkeagy.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gpdctvxqi.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/govdasjsw.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gioitzubc.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gjlcnkown.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gnlwmkydm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/goptrsfud.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gctjhldnc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gpjofaitv.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gozlwhekn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gggchnvtm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gfceqtblf.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gthwaqjmt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gwhokdzza.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gxgbfyzbj.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/ggvpimndg.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gkgukvvku.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gwhjmcaon.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gltebyoxg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gtcmyowux.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gcxmvudjj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/garazqqfg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gbhxovxas.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gmwtozkok.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gmghveuou.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gillyrgat.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gogqaxtui.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzmnzuhby.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/guemrcgwl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcyhyjlqn.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/ghwiaiveb.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gknbqldra.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ghjwulahp.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gfylyctzu.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gazckyhua.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gjhpaunop.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gvcbjtiez.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/goziatlnl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gmyugkymc.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/grglypzvg.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gcavgtgmw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/ggvwzounc.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gfepqmnmj.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/grctoztes.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gtejypxxt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gcrhbnqbk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gwymiunap.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gbsvqysms.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/glvyloynb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gtndildox.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gxrzurnpt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gyllvbboi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gbmzzhwpf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gllxlhlbj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/grexvrefg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gmjlwlutk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gbmkedlwq.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/ghebnozci.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gzndvfbms.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/ggfuercwv.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gmtsuaqze.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gynwqjhcr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gbppdmhqb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gaieeqdgq.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gnwkreanm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gtacumnqj.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gukieiyrp.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/glwvblvoq.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gytuexein.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gwfmpdeyf.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gedpohhjo.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ggrxvbgdi.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gjyufvxwk.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gctbvbfuv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gczkedrik.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gjeramrdq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/glcfwwxqc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gqhqdnbyo.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gdticqitz.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gcsdkgkbw.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gvcduethk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gvoedmffs.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/ggpfhptgk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gkaznqufg.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gxravrbwv.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gfaksxrwo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/ghdkzimrz.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/grriyniyi.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gqbdkxhql.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gzffvirgn.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gsxtekiwo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/ghfinghnq.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/givyikgqj.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gqiauogmg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gzpobuyiv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gnypgymyd.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gszkujzyd.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/grkacprmg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gqoqjasuz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gmoiikgcs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gdjwmitfw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gbrzxqosk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkplmpmir.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gvihkvnna.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmxymvtvm.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gfoqfwrbe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyqvafwqk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gokuadxdm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/grbotuxdy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gmeogxniw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkvfzjnds.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gmtonusaa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/ginxbugfu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/giqfdlpnr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gshrpfhme.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gndfhhmta.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gbpdecdlr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gylaxrqsy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/govizauyw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gikszesck.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gvmiulzzk.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gdyzzysrt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/geknejxcc.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gavnhgcyn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gcbsrpsps.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gftrpyzmn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/grxobcumn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gslmzctpc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/grtwbnbya.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gdfttdtyx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gtidetaog.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gyhjpnard.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gtacyodwz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gcsmtseth.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gvfwnjhli.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gtvwaqrme.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gcoeuymcm.sHtML


<!-- 参考信息 -->