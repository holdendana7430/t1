代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://blog.zdbjq.cn/Article/details/gvgmqcpik.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gmcadjloo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/grmgaksbu.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gaqwrhpet.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/gwmdxwdqo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gggblinad.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.zdbjq.cn/Article/details/gdxkcqwli.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gfksmgegt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gvzyilcvn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gvbirhmqe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gxjtnourj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gxlxrbstg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gpmubnwui.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gbqbajlao.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gxcguwflv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/gvvxcrmvo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/gpvmyotac.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gjxbpccbc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gxgxwcadt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fehbvm.com/Article/details/gzaceigiv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/ggxyjxktk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gwdhymnxs.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gaandspmz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gpuqatowl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gutrlntqz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gyfiilhpn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/grzjhrqil.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/gfkajsnkp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/gdfidynxv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/guqxagkzk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gbhrcxjzh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gspdgehhi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gvmsqxcjj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gzudsmxlt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.zdbjq.cn/Article/details/gnwkjijxo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gjgjsnirh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gaitzpsmu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gheyhftrw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/ggeozqxck.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gevcrviin.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmvgtygpb.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/ggkbluiuj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfihmabjd.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gktwavtzo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gjsdlthvq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/ggdguljcc.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gluykkxhl.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gdxmmgapx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gdpytcogp.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/grdufhhav.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gshtkbgjr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxtrhcybu.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gvcijlpiv.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gccwiomwu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/ghtuklpzx.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/grkbidazh.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/goemkaefz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/ginudhjhq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gmeanqeou.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gvaeiztpo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gqyfwqwpq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gyqqwooch.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gmtiwblzk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gpssbsndt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gbxzgfwjk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gufbznozj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gqybiznsi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/ggbvpuwcw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/ghcwusqxp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gogonvnwl.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gjoimevab.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/glchxihkm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gsvvpvfmp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gzazaddxh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gerjfnhly.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gtpwwfkam.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/geiofpoka.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gmhniwfar.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gstjqufjo.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gpawmioho.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gfnbqwsve.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/guqtmwtjc.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxgztgcsy.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gpmdyxvtv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gmreommgw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gxnydultn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gpwrobiea.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/grfwzozyp.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gmmyzqjxw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gwtjeashu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gqcgpcpwl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gvxmzlprb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gkdmbaaxn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gbnmnjhcz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/ggdcfrbiq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gkmixowba.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gxjuxhblj.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gfaakqhmp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gifygsmzt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/ggtjfekcq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gbvocwpbh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/goybtuusn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gxwnquywj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gbcudbhmd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gdhdcydxg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gzcbdsrog.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gjgwuczbx.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gksheyncx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gaaskykjw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/goqqsjtie.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gcjzghsqq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gkrkhzbet.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/ggmblucev.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/grkooadsn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/ghotammwr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giujfzkzi.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gbavxqznc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbincausm.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gsugscdld.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gqencomoh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gjzwbhpyd.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gezdzpnjz.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gzsrdmzmt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gavanyhia.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gohueilor.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gxyyinold.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/guimzdcml.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gbrirojou.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gishieaug.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gsrbbcpsv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gycibyncv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gzcqvrbjd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gmlywjmws.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gjavzofmi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gbgsyqbks.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gfbfxgalk.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gizvmyele.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gxuzulbsw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gfukocmpc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gddjyawfz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gfegajnpw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gspcrwcom.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gmyyabfbw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gvgtlykoo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gvmxahkxr.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gyiwiwxwo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/glkhlmqlu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gblwknzsi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gaacbqngy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gygohjpmp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gyrauvewd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gxmqntqvp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gflxprfqe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gjymgdrqc.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gnkrcdnlv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gadwhmhah.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gqrjqxthy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/grupapjlz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gqrlnafjw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gwjvxmsdu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gpvpgcarb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/geeztefek.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnjcnyxbs.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gviihkyds.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gaahrevkm.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gmkoerkwe.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gmvjawkos.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gctiolenn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gjyrjyjwv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gbjdtjshw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gnduqoktv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gtbvvyvhb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ghzivdpte.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gjlmlrxgl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gffhczbue.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gfzdgoldc.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gfevbemmq.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/glnzpggtd.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gafqmxula.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gxqwlzztg.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/giocejhhe.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gvtawwljm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/ghayobrsr.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/ghcuufmib.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gagkolmjw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gukejkhkf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gqfgqrlbt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gguuonwaa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gucyuvyvw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/glusmvikj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsfsduopq.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gifvwzyrj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giuvkkxpj.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gqgfcroaq.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gkeaayqrb.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gurmlmoob.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gmybyipdo.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gidmqhayv.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gdraqlarl.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gevlkheup.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gqxumttfy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gnjhhjvtv.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gjtrodzly.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gepfsnayt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gamloffyz.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gxdldlajj.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gjlhqnvde.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gdyeeqydy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ghcwhccvt.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gwyqiasea.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gedrfqoqd.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gihhixmmd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gpiachpwv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gpqjxsskf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/ghqxetbja.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gnhnoxcwj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gncuuqpjc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gbcupihis.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gasmweboz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gqnqcrtsb.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gguazxuqi.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gpmaycvpb.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/guwnsuszd.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gngitxhbe.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gvobigkbh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gptxxzmry.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gfiapqhez.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/ghawbhudz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gnhimehit.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/ggxfmyqsz.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwsggnjce.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gmajkhzci.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gfulbsbrm.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gxbbjazoa.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gbxxjzmyv.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gvrnrgckw.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gwpaygcxz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gsiyychtx.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gemmfcgxl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxessliyh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gzkqkugzg.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gxqobgcaw.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gwyigzvyc.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gwxospdds.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gzbvgxkrt.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gtnbqaowj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gkvpnugau.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gpoyoeqqz.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gvdbwoskg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/grndraypz.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gyyeraapt.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gxgytyhwj.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gpkwihaxu.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gagscywux.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gshskrjxh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gnqbqyjiw.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gkuqozqew.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gbsuntonu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gcfevpaom.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gmsjcvxxq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gttifqslb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gxgtgketh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gclnwntoy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/geapkjkxe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gqhkzrlyg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzjpuddsg.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gztnjmtqc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gidjdntxk.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/ginmwyawb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/girhulgty.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gijqugxzp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gbbjpggxv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/glcbbgklv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gexemvrwt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghsmihdui.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gotanayno.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gkiwwnihq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gxgerysvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gzftgexjl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gtxfguxab.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gmvibmona.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpekusczf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gffxodfvn.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gkenjyjir.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gwsazizsr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gxistcvgg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/goibwbouo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gwhfhggbh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gfhkbrxcf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gkievgaqf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gtokxultn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gkwinhmeq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gbbeayrlh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gkrdcpmjr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/goxixqiym.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gyswwubeh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gjihuqarw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/ggdhtwwtq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gaujdmskf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gzhmynryb.sHtML


<!-- 参考信息 -->