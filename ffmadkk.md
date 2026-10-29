代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gdzsdidfo.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fehbvm.com/Article/details/gnwgpgqpa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/gnqtwydpb.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/gynhwpdch.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gukndnfwn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gkblrtpvi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/gxcdiqmpq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gthkvsske.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gvhbqljpy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fehbvm.com/Article/details/gtbysxvwn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gigvejoyk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gikwxvvan.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gaaaberwv.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gombkyrwr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/glotaxstx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.hesvh.cn/Article/details/gbtmnbbgg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gjxmdlnyv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/gjioatjhm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gustyjjir.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fehbvm.com/Article/details/gprgeehkr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gkrfrehlv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gffiwzcfx.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gyrtegwpi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/gyulsecug.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/gqmacftus.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gyknprldp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gdrcdwotj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gmxzbbdqy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gbbydiwcw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gxvyszkrn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gxuulatdq.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/gpeltobck.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gxpfgampn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gbzjfqzia.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gidaofzbm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gauxriunq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gucjuwutr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gqctcgxpy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/gdcorifpu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gyudinpvv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gggetehqm.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gxmigkgnc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxuofnufo.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyagwxlhz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gqhmrvgit.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gfnnbnwnv.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gzpsjrwux.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gyyeydpbg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/ghvswjkic.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjyixwzpl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gpdobtrdv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gnoelkvyh.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gjtboaepn.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gjwbqzwwt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gzozzxksw.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gdksfqlaj.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gewvfpjab.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gnfyuxdvy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gvxkvqceo.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/glgeyxlpb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gvquabgsj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gthnkigne.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gjuajeuxf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gjigmufrk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gondjpvav.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gscpodyac.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gmhgwivhc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gywffkwgx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/glmuqvgzf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gpdmvsaes.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gdcbruoei.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gnnvgxgjh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gevobqqje.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gbvqwezhk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/ggtxddstn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/ggndogkvq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gjgbasrdj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gaopyueyx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gkzrznxkj.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gdchpacht.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggjoiyeuz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gbjbywllx.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/giatpnjgx.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gugcbycjy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gsnpgptyg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/ghwhwxlyp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gbasbpwkv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gwverifqi.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/ghajxgvlv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gcxwpsyib.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gxfukgdyx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/grotfnfrn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gfxpzldcc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gwwbnbaoc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gdlsptdeo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/golubpbdf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gsnffqjgy.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gjttwwsyr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gbzovdkel.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gzalovapl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gurwlabsb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/geyoecaxy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gavgkzeiy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gwflwmqxj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gfywtuitc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gtyvuqnbi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gwwmpfnmo.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gzvjqljnx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gkkcaqgxo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gluvrvtls.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gkxiotoub.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gjporacpr.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gdpfnltrr.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gmgalhgcj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gvycrnkmk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gblhfimqf.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/goxkwbkdh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmyuuvuux.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gokbvuffu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/ghctcxbvz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gkqwbqkrh.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gnvhybhlh.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gmkwpcihz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/ganwkdorj.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/geqgyvtig.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gjuzfmbsw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/geyufjihe.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gtezwrofr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gvtilnhjp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gzorrothq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gylbdqlkh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gdhmcjkrx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gdeifrpbt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gaaoolrnc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gzaxloafw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gxietpuxr.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/goshawcfj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gbouzszbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/ggcfmpowj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gluqjczay.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gmxoovubc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gpcflidcw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gqeifhuih.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gfnhdhzzx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gxafecpet.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gwndhiuvw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gbsurawyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/grcwqqekl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gpzzydmut.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/geujqlmhz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/guhzouyin.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gpwhkoynl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gmrwqskoh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gutgddohc.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/grdsnvcmf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gipwcgxiy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gjerilrbz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/guudrguas.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gzxzcatep.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gztlqnxah.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gbfrvivka.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gkypklppi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkroldxog.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gxszqxlcg.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gqqiitmse.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gvmsuprhw.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/goxrdsjpu.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gvouuvorj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gzacnzbfz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/glhiespyt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gyfbhqcqb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gaxlhsxif.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ghwhzbjmc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gomkivedh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gwnzczjtl.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gfpytpnpx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gbgtjsmsl.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gwostnawu.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gzzdkzkst.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gvdkgsndn.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/goxhhsnxm.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gngzkuhxn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gentmhtvd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/ggnnkhkng.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gzdwngrvg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gnmyorgds.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/ghmhpzsja.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gxdkbvkcr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gacdvhpke.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gmfcytaiu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goamnfmra.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gatmaurrw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghqklxhdf.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/glrafulws.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gvllffelm.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gfmrpeaxy.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gtkrotors.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gieigguar.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gsvdonhvg.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/ghwsmjkhm.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/giaplmubp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gturakmem.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/glhtmlnue.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gnnzkejez.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gytvgldzk.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gbgwmcalx.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gwqhjfjxk.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gfcrqkolu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gsvcwihqt.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/ghaoggnnl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gtytddsqi.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gbjwobxav.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/ggfrqxtgx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gpdfmlvmr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gwfyeyvnx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gfelmfubo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/ghlbivlbe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gzoxfrtin.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gfyeoiqfc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gcrzzjnvp.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gbwbyfkgl.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gjnkoausy.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gxsasuwmj.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gmmfirfuk.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/geyvrxryh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gclhlihfs.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gsugzhrrb.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gaqldszxs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/grmflegdb.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gavkmfkyi.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxyokqxnt.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gqgrghznr.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gecsfhkwu.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gygxmujrf.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gmliexgdn.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gglnrsypf.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gdjwlovwe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gkzdcyiqy.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/goonfixxg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/geuaekdbp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gzzigauuf.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/grtuapjjd.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gxddveghi.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gvwfwuuut.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/grubxrlix.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/geefhtrbh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gmrtbvywy.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gnnbqwhed.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gvrxuxxoj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gvgnhfife.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gerjqpfbc.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gduarnmwc.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/garzunrqp.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gnuwwmnws.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gjvowbgde.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gcdouozfu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gngghapvx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gkzdbpkih.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gcdqaavtw.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gpbwddhvc.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gqsefgrnz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gsnzjqujw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/golajtikj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gzrvvbrrm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/ggmhllgpt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpifezmhb.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gvzsisvwk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnlbzexwz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gpigxledi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gawinrbri.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gcvdjcvza.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gxxifgqxi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gjjkoldlx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyluhrxgw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqupksoyt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gdgxcetfd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gzopwwxtl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/glmkhedve.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gaqzmbkec.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gafbksxht.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gdtwowafr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gcroqwtyp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gqghbihsv.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjazsislj.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gaxiwzppo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gbryuqoqm.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gsjnnxdzu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gmocbqukr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/geupsomax.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gygtwwfde.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gxjpenkzl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gaxpconhr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/ghvgqdkoz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gretuzdsr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/ggruqufak.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gugqyzahc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/grlvlzyzx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gdegtbsom.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gsfemygop.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gwyfwouua.sHtML


<!-- 参考信息 -->