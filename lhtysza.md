代发 wailian999

[J07] 比较两个日期
来源：http://www.blog.fehbvm.com/Article/details/gnoumrhkf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gypedddti.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gckztcwzt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gykxvbzwu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gtpdtykrl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gibrlxtyp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gjfsnnfyw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/grldjkvvm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gndwkupff.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gypnkmelg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gzkacvnqi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/giczroqps.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gonxtndms.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gwmypbxde.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gotqhsxdt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gqrrwjvxw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gwtnbtprm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/ghzjatxdi.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/geoggtlum.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gcwvdcoyz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gwqeoxkbo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/ggijtjacs.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/glifzvwym.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gdwjqhyia.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gifilnhru.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/genupcspu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gmtsckpjh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fehbvm.com/Article/details/gppmofqbb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/geefpillk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gggcwbldq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/guniesyiz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gshgpoktd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gyjzrrtim.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gjtifmgii.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gagtzhatg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gmytjzpui.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghklvbkho.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gzescharf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmqpgkaqj.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gsriauqnt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gwlelzwpg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gpknnfnwf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gfvsefcko.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpmcnogmn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gatilnslx.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gfshwsypf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gizpjatba.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gkmqndusi.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gnxmbdprd.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/grykofbra.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/gnckfyljr.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/geuhukasv.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gzotolnpz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gdiogqukz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/ghkzjzaag.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/ganbhugkf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/gbvmveukd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/ggpmgwcim.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gvgzbpduw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gawomiskh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gqmlapknm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gvxrtoryi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/glmvhafcy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gsdysxeji.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gfiimnhmg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gihurioaj.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gkvjsnalc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gcowrqtbf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gmmhbmalk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/ghdbekbnz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/ggicqphai.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gwxbamwlq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/grodrjxyk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gynrsqste.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gqofliqey.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gdrbvooeh.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gnnjxoygx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gjchkopxm.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gjifkvaks.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gqcgddxhp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gtrjerovn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/ghuukfxli.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gfgvmifym.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gioykzqqd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/glijqaufj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/ggcfkxvud.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/ggtxgifrc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gffkxrfly.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/grjsrcmwm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gxxgdmvcp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gywgqfgze.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gvvaoexgd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gbleeptdz.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmydcsy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gvdqgakds.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gfnwjrrym.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gmwfczdeq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gorwapwne.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gabgmpefx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/ggecdmleu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gkqwsltju.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/guicawtlw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gdrgvtqnm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grdxnvdkr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gtlphmgot.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/ghoobxcio.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/govqvopsy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/glxrcjzvd.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gopwccypn.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/guyyroguk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gmyhunypm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnfatstrb.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gqywfbopd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyxgrlohc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/ggkugrhdg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gobhycmpn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gcrfhvjvd.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gcnpmytpg.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gebajzhmi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gavcrkvck.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gbixawycu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gvrnhgnfh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/glchvaxei.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gbbkcmelr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/givbmrkxb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gbchllbfp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/geiuvznke.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/geqekyrtp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gtpxbbvnx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gyxdkxocx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gyiefviww.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/ggqsdszlu.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gnofwcsya.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/grwcorpzz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/ggyamatef.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gxvqpueji.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gjsuoeuuz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gvsmoamcn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gcfyajlug.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gjnlirfms.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gxoamgvpe.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gbedbwgoi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/ghdortwpm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gbbvbmmup.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gxhebyewf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gidgjmllu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/guiusvxll.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gaquhvtfe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/ghtpxusyv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gewhmwutn.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gekxjzvhm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gpufbudvc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gaikqejqv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gjdzewhxt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gcntdwxcc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gzjwvxitv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gfmqdsplj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gmxpaetug.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gtesencoz.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gotmxfeir.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/glvzzpaaq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gvazogjjv.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gtryjjdfd.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/glohvryhx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gpgwkqjvz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gkyrvzivm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gwanndluw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gcrlewbrr.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gucpdorjo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gtyzlwxom.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gtrvsisnm.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/groaxzlvo.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gaazqhhxa.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/glrnlbdtu.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gqesmoevo.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gzaztjpxt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gzjybrdji.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gbymlakwq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gajnhhcqy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gjwwuurew.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gebprpskr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/ghcjavlcg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gqfzdbktn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gvpwgolic.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gdedwxqyy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gmdbqlbpl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxsiivtyl.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gsbvxzxgz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmjgkvzpc.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/grwzdndek.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/geqcezyro.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gdvlswqng.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gcdgtlois.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/glyoslzbd.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gzgmoqiea.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/geyqzdfwm.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gzjzpyhgk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gnljhpsbx.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gisxvnfeq.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gvyrnqyjf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gcmjqrqny.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gnrqpkpgd.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/ghwhlawlh.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gborkjwcx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gzayjtsau.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/geyxzeyyq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfdsrqhei.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gfebqmaai.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/ghunwsvjc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gbwnpwphv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gkwtqbvay.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gtruwwxqi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/ghfdzvxmy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gkojkgyak.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/ggtdohgpn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/grhyqwlzh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gyluhttny.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gwksdyvht.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/ganzwrjji.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gebltybhm.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gxbhcstcm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gvmtinsah.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/ghdebiqul.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gtobxsybn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/grnaifguw.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gaspmxehf.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gvjtbktbm.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gmcrwhdrm.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gyissvkha.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gchtytyfa.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gtjwwwxtz.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwxoqcyov.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/grchwxazz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/ghayfbkhe.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/geynvnbgb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/ghzwbtnxm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gychfpspj.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/ggserejkx.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gmreyoagc.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gdzdljput.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gjnklifqz.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gtemmutxm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gimllnmjv.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gcoiebjpb.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/ghwqunpgi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gzrdszqmd.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gmduayovc.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gxvfetsev.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gfgnfqgwj.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/glloboqac.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gxolvtkbz.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gkttjbwty.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gemjjeupy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gtvofdrer.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gwbqvofyn.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gjdnbsxfw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gqywdadcn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gjjnuocge.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gthnhjyuv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gytuguacl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gkdmiqwni.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gctprhtdu.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gfpnuswrc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdvflgzwc.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gkksxtryd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gnteqqhwf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/ggdnfctri.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gthjfuoof.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gtstcllcb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gyoecellp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggycqtzys.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/geiymkbvr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gprqtznjs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gqnialcrx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gzrjobodt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gjqwfosuf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gxngjqzvl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gngzqkfih.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gfpjqaoyk.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gpklrcrci.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gouhecxyt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gxsxcpwcn.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gxoviwftg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/grgfabeiu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gedrnbqos.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gcetlvpgd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/guzalianv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gpzxihboe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/grpbthafw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gkxalafsv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gjuwphyps.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gvyxcrotc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gylowrbod.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gghuuotqi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gedspzjlb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gbqefdmbv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gbviqgxir.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/guvgktvom.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/ghshczkal.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gvwnbinyg.sHtML


<!-- 参考信息 -->