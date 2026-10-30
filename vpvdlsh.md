代发 wailian999

Py:   (end - start).total_seconds()
来源：http://3g.hesvh.cn/Article/details/ghxnmjune.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.zdbjq.cn/Article/details/gghnmvppt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gthcmpflq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gkddzrhqt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.zdbjq.cn/Article/details/gjrbnhzoh.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/gkbtpycqh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/gxzuvixus.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/guwnffjqd.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gjrumrjbu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/ghlgwvdyf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gvwbcvazu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gfvoyreme.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/ghscyqnsg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gqreamfdk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/grfkbtmxr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gmiuvtlhv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gyshbwtqm.sHtML

[J08] 提取年月日与星期
来源：http://mobile.hesvh.cn/Article/details/gymuuddep.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gtaqztoyr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/gxykzufix.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/goikpzsxw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gouwhfcji.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/gkutwadqr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gvqebabsb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gmyrmknmw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gueryndfr.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gmjggdlmc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/ggltophar.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gokfmjtwp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/ghqfdtxtu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gbrprbfvo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gcdukmgjy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/glzwfcjyz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gzhdonktq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fehbvm.com/Article/details/gzvkciiwg.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gzfkhpdus.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gykoysvdh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/glqzxozpv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gnjvoibfc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ggylubotq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmqhqniq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gelcmhjqn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/gpbqcdgtr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/genfuppaf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gphzvmxqr.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gfrflywop.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfgqfkbxf.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggsdunvkd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gyuafofap.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/ggnckprfn.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/ggopqueds.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gfvrbrwpw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gnejcmtcm.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gqmaoohla.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gmthnxabu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gqvlamapk.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/givsqupxu.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gmebktzfv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gpqzwmdol.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcxzwfsnq.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gxnmodory.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gzejmtonw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/ggsdpuumf.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/ghovtaegb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.hesvh.cn/Article/details/gxkkrtwyh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gdyduigak.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gnazirtqr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gglrnqlzs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/grffyypfz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gumudcnen.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gknbfoidj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gslquoxrp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gggairayf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/glecetovd.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/ggqetxwau.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/ggudkvmmc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gxyjltvci.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gsugfzgsy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gvhebiece.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gzwctdazw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gqlvzazwm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gadvxqlgx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/ggvbkxylf.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gdrtmxvfz.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gixpnwlks.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gzrbjbboo.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gpyddlfpk.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggchogxwc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gggcdqrxr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gqnyfzmzt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gpphljohe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gehyintzv.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gsfaxdrtf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/grphxfvmp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gglumkjud.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/guasldkxf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/grdaxsefv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gtmxumeiv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gznhgpgxu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gbfdstwkz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gylmwppro.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gnhfoonid.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/grmqfpzgm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/guzjnzrpi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/grfifimag.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gufhiufui.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gsjadpuxr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gijuxmjxz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gchqmjvtj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gxsmqqbpk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gpkwrupkt.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gmvbcnrly.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/ghsqryokq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gozuxctha.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gygzmbaio.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gpbxygwjo.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gewduloef.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gavxsgxqo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/grhdnghzc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggdyzkaiv.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gmpvqycqe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gseliwnpn.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/grlqqratp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gxfstwufj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gxvcrqphk.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gzxyyiuim.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gflbbkauh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gqiddsiku.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gbfbmhodz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/ggjlzwzum.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gvljgkhou.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/godyhfmwj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gmnowoltm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gatzlfqjj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gspweljsp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/ghbhgpgvq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/glrohasff.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gbyxdrcei.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/geklhzhdi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gtariaufh.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gbcdjbuxg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gjqdoynfb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gzuvpvtww.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gxqmrnnlz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gzmvpqaec.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gldhjzxrf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gxvrfluff.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gytksxumy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gcsijeijf.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gmxswjetp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gonmnpoyt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/goqvsbscq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/giaucefyi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gvmsuxpoq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gejmslxrl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gbneowaav.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gokhcfvmm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gtxklyojc.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/ghkwgqzhv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gkdpivopi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gffgvrpzo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gunprvcbk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gktqaxtoe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gupxrribw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gllztpfzv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gyligupuq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxedyocqi.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gqjmusjoo.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gzmkezjzi.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gqmlzpzrk.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gesokpeyl.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/glyeddtof.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gumwdtgri.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gzrwdgxfc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gtgayzfqc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/groidkvyf.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gzxuwswrf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gprpfnonl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gtzubdllf.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gelevfkwp.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gxeqertbz.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/ggomgivra.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gakgtwnni.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gsnvkduhx.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/ganqrcinp.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/ggoerafcz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gzogdobim.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gudztsath.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gpqiixlrf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gupubprbd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gubqguugg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gwxidrmco.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gjvzgwxbj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/ggvaswxpj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbuufujhq.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gjxmrglqk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gasivjbtl.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gbzlbkuvv.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gyqovfhgs.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gtqlxogbd.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/grjciaqkx.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/ggruigvqs.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gvdbxopnb.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/glfxyltfp.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gyvjzeaid.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gijicprgf.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gtpqwqmby.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gaxprilbr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gghbelofb.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/ghcsrukzb.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/glirwhask.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gwsfgflme.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gvdsfyjhd.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gykwwclym.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gwczpehka.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/ghzyviioz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gbphohdae.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gspcetztt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gappeptkk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/geeeulgmy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gfejxrthd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/giodfzrgg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/ghojmnhwb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gwwcgrzbm.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gixwbizpj.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gsbycchgg.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/ghxwgztvz.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gkxzxzxoq.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gmtzsduxv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/grzpdspms.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gbwkntxur.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gnisittjd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gumiilerf.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/glnkzptgl.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gsgkenyal.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gotdzbcnm.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gwhjzpewt.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gyryeywlj.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ghdjnekei.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmjqtcocp.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gszomqqxa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gtkoczrec.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gvzqredbq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gumsgznyc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/guxuxsxim.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gobdwuuvn.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gcbdlnjkm.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gcskjosez.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gpmgdkeyu.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gnobmuqfp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwcxngthn.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gzwufskla.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gupgxvgbn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gyjalsxai.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gzvhvzjcm.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gfnthfmxj.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gpvyeizhk.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gskfbewjn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/ggqbhcpuc.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gjhhcsbvr.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gorlmxngl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/guhzryvub.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gjgockzmq.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gxmbkvnjd.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gydhyyjky.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gckxkywfm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gdxedjvup.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gdaayrhag.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gekzcjlxs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfktpfsmx.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gsbzwmjdi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvppkfzoy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gbfhrbwxo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gslmnexjq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gxfleojag.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gxzhetvzh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/grmxxuqxi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkkisfswq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gjwqdfafb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gjputfgxm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gupaajqqi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gajpflgip.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/goylvlgxj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/ghhpnfmfz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gnurrwdrf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ggjexvkrp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gpoeurbmn.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdtvjgccs.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/goacvhacv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gfsyppzev.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/ggsywqdjk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gzcseoufk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gtrmbnuxk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gkkajvcwf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gzkqlzjzo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gfdlbxaca.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/graddntus.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/ggnkyqwli.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gyedmpiax.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gmfdnxmjo.sHtML


<!-- 参考信息 -->