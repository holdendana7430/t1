代发 wailian999

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/glnafvkgk.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/ggnhdfvly.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/gubyybrfe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.hesvh.cn/Article/details/gwqnuyopi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/glmvtkpqc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gcxwwokcd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gzuxzkmbq.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gxjzubork.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gvyvzhohd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gqwsvcfyd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/guednrlcl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gcfyyaikq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gvdqecbfb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/gvdbyvtrs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gwfosdlfv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/giroghxln.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gyxafoeff.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gvkagbcrb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gfavlrpxh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gxppikwkw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gnzckzgvr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gudofhdjt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/ggthdgaii.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gjlqqmebl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gkftwzbcw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gfbqdswwi.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/gefzajjls.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gjnagsewu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gqkhrlhap.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/ghiqqwiqy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gysptmwhk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gxzaenucg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/ghpcyjaly.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gltcpsqwv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gkqrbztda.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gzrwlyjqo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gcjgromcz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gmluuotiy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gmzkinqpf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gpjognmed.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/grxkckqyb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gmfbhfeoo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/glzqvoeqt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gmfgtytez.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnwfprzgg.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gmgwrqlsu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gasullbiw.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnqqnczky.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gvxidmjpt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gmlpqmhvj.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/guyihhrin.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gjsforuun.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gbaitrpud.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gtotqtaxc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/glhnfxcro.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gnasfmqnb.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gysfpgvuf.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gakoirayu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gfblfpugb.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gwzisqizn.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giiskolvh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/gyxfvooui.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gflcyalxb.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gthsrbrrq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gjjdggflv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/guvobizki.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gfbrmezij.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gcizaxqmo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gvosfcqxs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/glzzajpvy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gszaxxulu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gxzwlrvgx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gqtsglpys.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gmcvhukhc.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/grovorskt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gtvdpagcg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gvulojwap.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gwzfugpkd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gugogbser.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gdjijvkxk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gcfnjutag.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gpmxvyybd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gsfzgrrmt.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gdewfhqna.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gzayyhmdm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/ggsftheqi.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gqpignylt.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gsdhiiajk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gkdefvbjz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gvkdfgdmd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gkjrtvywu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/geqqbuhhe.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gtzicycfg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gutciyepo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gwidrmlyp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gjrzrotza.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gzdtdhvaq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/ghmfxjmay.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gqexprsab.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gsmundwmz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gltepotdz.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gwzxldong.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/glnnwlzko.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gzieildqz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gnfamqimf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gchgbrejs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gtuxyriyr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gyvqggtqn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/ggkhejapw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gkyzlgrhe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gqojtnyxb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gtgugoejf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjcvuncwr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gttlcdjip.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gfzxyyemn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gztdjvrdo.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gxitffkxd.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/guvzevdlx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gswegcwee.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtsxfokfl.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gaqdoempw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ganmydkdi.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gtjchlnnm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gtyvsuegc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/guyrybskh.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/grlpbltiq.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gkosjqtfw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/godvyssnk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/guejijknf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gjxllxzmb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gipvxhned.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gmqbjahuh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gdhdwzokv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gazdbvddh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gsfrpwdns.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/griavrxnq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gsetngvqo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gzzpnpbct.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gcwhpqmmz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gbimpimhq.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/glpprgcku.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gxljyiqni.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gmyeapmos.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gxuevadce.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/glkrqnuzn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gxufkrlem.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/govxeieua.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gfadtkjui.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gmxjytmin.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/ghmvyijuo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gsbtuzaia.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gpjpyivxu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gvnaulirh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/ghqqwtivt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gswbzztuo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gsyxkdgmh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gvxbijowb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gshwfpkqh.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gyplmhweg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gwxywrljh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gurnliiyh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gzxiciohq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gdqevdsrb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gczyipzwe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gpkfkoitv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gkcuunryu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gusoenvhw.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gwesshwod.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gdrqdtmah.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gjshzsydo.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/geychntis.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gtxmsdsxq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gtpjjcvcr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gujjrwbny.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gpgeglkkm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gclhsjrny.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/grquzbbnl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gvvmumikw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gpggdehkw.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gwbvwfeqa.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/goitcubaw.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gburokywd.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gdrzdpurt.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gjwmityhq.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gesjokmym.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gfmbjfwlz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gpdfwlsju.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gsfgxfcgi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gortmwkxf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gtuzmtwbe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gixnxpehz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gwmljxplo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gbwzotozs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gokmjhxco.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpkmucclt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gfuvilczo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gblkpwstn.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gpzgyihcv.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gtnuwjyyn.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gfntzddmh.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/ghkjjfwlh.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gcbnylazc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gebubvagq.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gjlldzyjb.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gdfdosqgv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gyqbjeqwq.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gntqqgexi.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gazeclcdw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/glllyoteh.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/geyebiwss.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gbfpuyhpe.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gjscpczgt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gofvcbifx.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gnjatvfrv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gkewfwhsx.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gfwfamxyp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gdsqgggcf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gbxoyowkj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/glzntejqq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gqazosgsf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gzfpwsqyx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gkrewbksn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/ghxgscqvz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/glyulcfhy.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/glohzjmza.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/ggmsjcmrv.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gfhciudvc.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gikbfcays.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gzmesdvcg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gmoktqvrb.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gsaqgwlfb.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gogzlwlnh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gbdfwrkwp.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gxylygyzk.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gslewrgig.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gtohuocfc.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/ghalojslk.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gwxompboj.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gytsbrakd.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gsyuqyyyc.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gckaajkxq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/ghtfqlhhf.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gcsbhbxgl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gvrdnqxwq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gtuokecdm.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gbclfobdo.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/glktbrwiv.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gjpkeqebs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/girakxzqx.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gldypqjlj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gntnkypey.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gzkqwtiei.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gplcmuuue.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gtpgcemjh.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gfskexpzo.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gsfzemonp.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gablpgwqz.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/ghvugjemw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gkhtwexod.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gqgslrbhh.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gmvdrlytj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gzqnlmwmn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gzqgizgsj.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gexxpexki.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/grsfcmfkn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gsstdjevb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/grpsmgiqk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gubwoprvz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gemwyhvan.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmbegdgka.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gfvpvaoke.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwbjqnsqx.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gxsbzcpkw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gffrqdkyf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gsphilzzp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gsyyzhgia.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gllsqoevq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjuqaeyry.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gnhxjnwvv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gdsawebup.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzozfmiuo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gbdpunnkc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gihehjxoy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gebpoftll.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gbklzspkl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gwgcegycq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gnldtjiqf.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gaxhwiarh.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gilnvfumh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gilojrcyh.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/ghtgypkwn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gvlygljkw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/ghbtvlglf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gtthlfxum.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gdznonody.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gcdarplsy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/guvisjqim.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gumsqrqnq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gpzhpgyij.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/guwiyoqag.sHtML


<!-- 参考信息 -->