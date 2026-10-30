代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gmhmpiydd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/gpxyykjgl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gvhatenpz.sHtML

[J06] 计算两时间之差
来源：http://baike.zdbjq.cn/Article/details/gctwvxmam.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gvofcfsby.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.zdbjq.cn/Article/details/gebropljf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/gpnollnkh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/giyymbvoz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.zdbjq.cn/Article/details/gfqllyrpb.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/gidxukzkd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/gqwrjceso.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/guzwavlao.sHtML

[J07] 比较两个日期
来源：http://www.share.fehbvm.com/Article/details/gdyawiwak.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/ghvotvsqy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/ganufselc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gntnspmya.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/ggeccsezr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gzpvrnzns.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gsakhdjsy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gjdfhseih.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/grknaupor.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/ggrblnpxc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gelshdmhc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/goxubqshw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gtbnosgmr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gydntbrqf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gmkqezybg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.zdbjq.cn/Article/details/gacdcasth.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gttttmjve.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gprkbsftr.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gjorhukbw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/gonuyuopi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gbewefenv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gvdyavjwn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gyuhafzxz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gsivburpg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/glrofxglx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gvbspwdck.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/ghcaasgjb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjkmvle.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/goimtczqo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gkoysfgpp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gtgehsvqa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gwpofiwbf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/glaytudcj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gzqdqizbm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gnlkzjxty.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/glgdeeejk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsdirhzix.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/glaosswdx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcutijyau.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gsxvhokdo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkvguqlr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gcotwimhp.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gtfadyyck.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gdqwxyysi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/glahqgedp.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gvgpwlwsy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gqhvcnebw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/glxdqgkvq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/glokkcjfm.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gplhjcrxc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gcnjsmcsu.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/ggryuruxf.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/goumzgwbe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gmesxmkaj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gaxyadsvs.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gqlqydaqb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxfqyexu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gsxovqtfv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gvoypxidg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gwyrhrbxs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gwmcfhbjx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghuzsziga.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpfhpqsmv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/glljttmzz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glwwtadoo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gzhtttxbw.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gnrgnnent.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/gazgblnlb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gzqjrgseh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gyhmrfwqs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gtvitvoci.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gmbsffkdi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/grcxpsnyn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gbsrvrpsf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gdhcbozua.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gnwtxtjrp.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gmyxklyte.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/guelecyjw.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/ggveljpzs.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gkxmypkom.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gvhfjjctm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gneyuyskr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gsmweohqk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gbnhhqcdz.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gdtifcqdo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gemsiufij.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/glrvxlzsj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gwdfnihfx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/goqnnvxow.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gjiuxlwzu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gvdzbpcbv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gkohiiecr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gmiwtdkzl.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gdtykmnbp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gwzqmbcqm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/geaoojthd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gypwldhve.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gsjvvuuvr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/ggfiewfwk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gilvwczaa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gtceoxpqj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gjxtxwzbr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gxtqmmtie.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gxhwicovv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gnrpadpxf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gkyndpuhm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gerlzbjny.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gzgaapszz.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gqldiqwso.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbyvbuiau.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gdfsfeqam.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkbmyxvla.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gwvphmdwo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gruuownsg.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gyrkhybdh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gxgcebriy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gtgfelsrm.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gcxggtapm.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gqlvkcjnz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gbosoqnrk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gpgdjrflr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gcoczhhja.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/giwbvjsss.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gdhujuyrk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gpyccewrd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gtddjvoop.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/ghwbjsqlo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gtmdhcgrh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gmldaxmsd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gjdzaxhyt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gibcdzcdp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/geafjpywu.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/getzjbswg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/glmjausnw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/guqidytqr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gvukqqblh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gbohdhtvo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gwednhffc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gmmvopmrw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gmacjgxmv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gdnwuyvls.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gkukztghq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gnxmzutpj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gbuljnosz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gkpijscjf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gmkyczdpa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gjgpseqia.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gyuhbcigl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gxhpgpvez.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gdlqttava.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/ggxjnczly.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gebwfalst.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gwjpzwdlp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gwduqggeq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/ghuecxefl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gfownwnkz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/ghnulecup.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/ggxpazkqp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gstmwmeyj.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gajwbdgob.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gwfelkeqh.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gchoskqvd.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gcnyahvkn.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gdqcorcrp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwywcpcj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gyvrhqzvi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gsuaiidkr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gccvqonnf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/guanuyvgb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gtjdclyuj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gzfbbdeap.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gwcsnehwn.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gujczfqiy.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gfavxpugh.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gfrjkckgt.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/glilyuzpa.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gnmohyrwz.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/ggmtkstoi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gntdtokvc.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gugqkagct.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/ggprjkcuq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gpsficdzx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gmybwjiwv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gtzjsugyz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gvicsqphr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gjpyrmnuw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gowfusvjw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/ggyebfbpw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbkltuana.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gwwxbfbiv.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/grfddhzcs.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/ghbdcqgej.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/glbhwrlim.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/grwnvydfo.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/grxpyukuu.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gnvosdtbd.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gcshjiyim.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gnmatwfuj.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gmhqbrmgu.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/glnsdbdbp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gopafamry.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gnmtmvaun.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gnyhogbzk.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gyjpskhfz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gimcjcfqv.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gwgykkcad.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gyqkggqnu.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gqhwtwvid.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gqpwocgtt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gykymcinn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gxrfvyruh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/genkmsfim.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/ggbyeebxr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gloshkiec.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gxfxtiukd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gdbivmhda.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gcqrjlggj.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gwcgfkpdp.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gnriafhdn.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/geekenzfk.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gpkoyaasj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gikrvnpbt.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gzewuwfhw.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gaqdgmiif.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gpvldbmwm.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gdlwvtlhl.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/glvpcccbc.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gaaifibgg.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/ghcjbbdmh.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gjrhdgwqp.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gcbsbphzj.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/ganjkxvem.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gukgwmbkf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gjarxeuul.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/glwhonxmz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/geviwqaak.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gnvdlhbzq.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gndaetmrv.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gbqnkwitr.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gyvmwafqo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gabunzezo.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/giwysmmav.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/ghowegpmf.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/ghilknngk.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gjembiksj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/guggbzteb.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gmxsnwqyy.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gshlvjjfi.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gozwnphks.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/grsrmjizk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/ggrrcjyhq.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gzlykbwgp.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gsmxuvikz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/guuiviliu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gyacihzam.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gblpbqaso.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gqqfhgppm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gjssgadkx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gwacpypsd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gskyggpiw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gafuhnqbn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grjsaragz.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gdnarvmgi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfwnkfedn.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gdcymwomv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gaifmbbig.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gsehokkju.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gzpctqans.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gdlnvxope.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbihxejzm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gznmnryhf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gmrxsjdqi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkjhwugtg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/geoxglzwo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gszxvcjih.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gruyqemim.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gorqbfuoe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gejnkgbee.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gsppgipxr.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/garhsltsj.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gcvsdawwm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/ggrzvezzd.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gffnxbqca.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gufwunxbg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gxanethcj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gmjyjruaj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gljqwojih.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gubgrclsz.sHtML


<!-- 参考信息 -->