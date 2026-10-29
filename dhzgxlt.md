代发 wailian999

[J07] 比较两个日期
来源：http://www.share.fehbvm.com/Article/details/gqpfidkuc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gfrsgbius.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/ghhjkimnz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/geyeeabkg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gofdzzslx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/glywxdmgl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gusayxlzj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gkajfrsca.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gfjobbxnb.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gwwowivqv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fehbvm.com/Article/details/gvugkypnl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/glizwcwaa.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gdzkndyfs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gcitwfjmb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gnmfrfnfj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gvhjrzfup.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/gybwoxvar.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/gqbizbhml.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gdgxxtuvy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxellqqi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.hesvh.cn/Article/details/geyvfnavp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gwdrjqave.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gmsiprkon.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gyqwoeczy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gtsvrggwf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gxtmntawy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gqnaxdwsl.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fehbvm.com/Article/details/ggfqdipds.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gmusjeyto.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gkcfskdte.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/glymyozhj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gmxpvleft.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwacucdos.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gictjdjwm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/ggrljvuph.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gazclvwwt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glluhdydo.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gpeqhpxig.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfxwbwglm.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gcfjrnidz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gxonxrqop.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gtjqzovie.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gmnclqmwl.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gpirhbpme.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gnykadggk.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gtzyesxfo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gtfqticnm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/ggrhtdzre.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/gcvmujowk.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/grolitjjh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/ginxamscq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbccipgxc.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gjxncmojb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gmcgotaso.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gsnaniior.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gdtmivhrt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnlkwdjhf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gbrbgazkt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gujtpteke.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gomrcwcvu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gzpbzgizk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gwirgdhyn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/guygbacxj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gjbhsltnt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gupmticby.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/grfzyvjke.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/ggiystrmy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gugrbrdqz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gmuftobxy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gibquexpd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gjtexeoxl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gzzsraxch.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gogkflrbg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gudydycwq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gfffgltsj.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/greyinmmh.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/guqdqmstz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gfozschke.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gejfdwojs.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbxecqoci.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqtpixh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gkyelrhcf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gtqdgpqdl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/guxnagmdt.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gosymixrk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/grrtswiuh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gvqqnspxm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gxwvrzdmn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gwovjeust.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gupjyrihl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gbnrkther.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gqvxgqmgl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gpfgomdkf.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/goykhoqza.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gffzibfmg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gtitwgnbv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gacviurqj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gtggeijpz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/ghmyvqtyq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gmyvlkoxb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvzkxrzp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/grufdwnba.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gigagbtbm.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqokukahg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gynkofikb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gonavctin.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/ggpblguxc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gsbxcpkoq.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gummodasc.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gyskbpuyv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gubiaotjv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gawmftxsk.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/giesfgagg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaqmnnnkm.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/ggfqbuvdt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/guilehlau.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gawswrsyp.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gkmswvorh.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gytutvtsp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gddepxyie.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gbvevarjo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gkvsmfuat.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gnmwqqxvp.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/ghynhfnyb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/guqdnhsox.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gmmpsmzdn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gehujxeqz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gaksswmry.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gjuxuzqyd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gvdarwiiw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/grtzjdwew.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/grhwlaysh.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gmyjdnzvo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/glwfkecjl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gjcvqjnee.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gtaeudnhi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/grojxdonf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gxcwyayli.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gyklzyirc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gfqlbydyk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gutdpydrp.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/ggxtcqtdw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gimrrgvzq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gpqllasvb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gneodhuob.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gkjcfebld.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gjgekxzkn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gnijwvxcy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrlwjnxw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gsbfiuqvf.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gpbtevaji.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gmwppljyx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gztwfqqql.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gucntoflq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/glsquttkd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gzeykhuzx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gnlgbznvp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gsucolwqs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gatfudink.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gwjsknrlm.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gknlulnlq.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/giwyfvnzq.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gzvwlrncd.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/geqipvylm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gwqybxhfj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gtclpmdyy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gzjhavuhz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gxasjcbrk.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gtfymyduy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/guhilfcuw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gyrwfnnim.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gqkuxlseb.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gptvuwwhf.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gnaezybol.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gujexdhzu.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gmjrxibho.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gvtpyyhcd.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/grbnsguhj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gxwoczmgt.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/ggrmbzqgm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gvvlmqcuk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/glwddpqhy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gozxmbogj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/ggrgtcgxu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gbcphkdrm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gqpqgkkiq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glpmbzabr.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gyqqncurh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnrejacnv.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/grdkiuhjo.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gnqvlrgex.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/ghwwakbuw.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gshfqgfcu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gbtgykawj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gmbyysfhd.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gjxeohuog.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gsdbegqxj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gjmizrxyz.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gwtvwbswz.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gfkpoquek.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gzsmflgrc.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gaqcwxspw.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gkdwyskrm.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/ghocurany.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gbmqqdrwh.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/geppagieq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gfnqthrim.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gxvueydtx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gxqqiffep.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gtuyawaet.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gvdvkymdy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gaaxozdvu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gzlmwjmlj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gancdelee.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gfogydezj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gukfqrihz.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gvnnfcieg.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gxilldmsb.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gxpcrtibe.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gvykapmub.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gnlholiqt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gfkheovvm.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gywdypklk.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gcugdzehj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gtzgjcokq.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gdoyyghex.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/ggskuxzfc.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gefvoyuiq.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/glkhzcmdl.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gdszjjqdj.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzrnxiqcu.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gyukuusbc.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gxmijxqtw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gnntwajbd.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gzlbbnekk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gcdauqocy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gsyvymtro.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gdzdnaeor.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gpwrkjsds.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gpdiwmwcv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gfayxdfxb.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gtdmuujjm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gskyjzhof.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gkouunrgp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gzdynbqpr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gpbitaaow.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gjvapgwnl.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/grvrbnxfr.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gupbtaubk.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/glclfmpjk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/globggsmt.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gapbgbvlb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gtpfehgev.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/glbytfwza.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gedhxohjv.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gbtuoahdz.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/ggtmwjbqk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gckycmsxm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/ghvwddgrn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/ghtrvzgzz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gfuwubncl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdctfayaa.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/grxekhzxd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmyygxvvv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/giacsperz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gvfbpyudc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gywzkxozl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gukajhnco.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gmmodanic.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/geaebjfer.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpjpidpfb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gyzzcshub.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjiynxfbq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/grvgfhidp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gmhufbtnp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gznxuxdun.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gvbvobppn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gunpeglum.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/ghlxbhqpg.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/glszoglke.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gvyspjwuo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gkrrfrinz.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gmxbxeair.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/ggmqnldvf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gdgiuumnq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gcwlmtpai.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gmqbqvvit.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gzssgvasu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gqjimusvv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gbyylzocc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gdcjvykqo.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gevgiwtqb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/grjowdcre.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gfjcwdhma.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gdfizuygz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gimdtkfmw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gmftdlbon.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gngaklojb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gkeegksfs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ggzylyeon.sHtML


<!-- 参考信息 -->