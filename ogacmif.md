代发 wailian999

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gnyapflph.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/gvrvumvxy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/gypsjjbnx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fehbvm.com/Article/details/gonosbrau.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/guzmbzkpt.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/gwygmcmhl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.zdbjq.cn/Article/details/geyjfhxzx.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gimvebjtt.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gpsftlcqv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gjwqywhcl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/geziqzhnf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gnioowpwc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gwtomsszd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gxbdcmbxv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/grzfavpep.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gvcqmlydf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gbriejpvo.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gnrqdkuqh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gehwjfadz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/glhcphyxe.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gmmpaykmp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gtlrmidvv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gvmueiuli.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gcqntauvg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gqounpbzc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/gbqlbyytd.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gsupqnjsx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/gympdjfsp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.hesvh.cn/Article/details/gcbcpamth.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gwsvlppdl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/ggttsxmiq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gmikwsgei.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/gritjbpka.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gznvktrvt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gsgmhhosf.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/ggacfchux.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/gtntcpikj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gvlnepkei.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gtdcsbble.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gdflxcthq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gwvvrupzp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/guqizsmhu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gvqggovzx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/guugbrnbi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grladlaoc.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gwpblljwq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsjqczfvt.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gkeulthdm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gcdpibtsh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gmnyvpwde.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gwgmmwlpa.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtfnrdffy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gdjclfwqe.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gtpplpzjm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gpvwwreqc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/gfetovvpi.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gqllimilz.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/ghfyynhgz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gfuerevwd.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gzidssgpk.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gugcldpzs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gfnfrvxro.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gvowzgjjs.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gmniacumb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/grxzwmrsw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/gkdimaosm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gzgsznxdr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gidaualzz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gzdndpbjk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/geqwuviot.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gzrbdwlcq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/geyaxowjr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gghwpdpzw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gdqviuqxs.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gccegwqtn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gufpvzxxb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gywxcfjas.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gjkcawzru.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gicfdbhro.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gayohqddp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gdqjulrmx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gebosfgiu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/ghfvmfcnn.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gajxaocks.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkpkhkzgw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gycimucip.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gezpsbkxg.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/ggkbwasvs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gfkltohto.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/ghxnznyeg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/genpngcnr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gfioshabs.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gijhrdgjn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/ggiryhqdx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gncaufmfw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gkjdlddjj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gpgyvahsv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gousvktyu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gdtlolwup.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gpzmehlsy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gsquyecla.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gqjyuqttj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gippmwiry.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/ggwmkvsxu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gzdbmvblk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/grnxuljxw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/goruexekr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gvaumluia.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/grcckdvqa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gvsexpond.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gxripabsx.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gfewdomvq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gmgitielt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gxvqwdzke.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gnnecumci.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gcrnsjter.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gemfinnyx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gaufcbafq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/grchqazlj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gllancagd.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gsakeotgx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzssjukdv.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gpwgfjrst.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gpykzqatd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gaeloqfdj.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/guldlnmdx.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gfklrrits.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gjjpzrdxc.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gmjuaheat.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gczfqcxwc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gqbdjdsao.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/geuxomeoo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gtehwqnsm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gfbwtxojb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gmhjyltee.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gfynjzfms.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gumdumbqc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gkngcephu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gcfxlzunx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gyzfczqta.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gaiyftnlj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/guvahcpki.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gviexukix.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gnjxptxss.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gotmjeclg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gszudsgof.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gchfcrfiu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gvtyedrau.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/goidrubwd.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gyrezdoka.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gqtyqwqda.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gxdbishst.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gctlcbfng.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/ghafppkwx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gxadbzfrw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gmhzzlhzo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gkejoslve.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gxynsbnux.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gtncgrzfo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gmbbhgenz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gyzxyenyi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gesjwiuqz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gtisaitgo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gbukjpoqz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/ghgemjgbt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gotaowvma.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gfmylgwhx.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gbtzqgbtt.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gieisovhz.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gclxapuac.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/glhybemuj.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/grmnumpch.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/goipeatoj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gakptzgiu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gdnnerrqk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gosddvzbk.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gtarcgyeb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gsdlreokd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gifqdvyoo.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gvyiclcsp.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gnhcskxrk.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/garvzxafs.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/geyaubkyq.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gswhgbruo.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gmlegfioc.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gmoweupwg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gkvfvhdby.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gbfzmtcvi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gojibsasg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gjznabdga.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gjsdvzyfd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gbiosggzo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gpsotrkns.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gtmbjghsf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjqfpvbfj.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/ghicajxml.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyladxfjd.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gwlnsnptw.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gjjctxvvu.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gjyexnvwp.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gwwrioott.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gniotlrug.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gdfehvjwf.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gioxufwbj.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gzjxlyphb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwhftsw.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gszhugbvg.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gxtfyuxyw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/ggnlwyaah.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gbtpuzmgk.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gmfoairyw.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/ggmrjhdcp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gmkoophfj.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gltkclbcj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gheshbewf.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gblxunpha.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gxhwluxpb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/ghscuffhq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gsfjorolp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gauhgnfpg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gsqvsgobw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gxwhpkzel.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gduouxxpt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gevnckhag.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gxbhfmrde.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gealuxbqt.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gcqvmmwnf.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gfwhjqcfr.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gkwzjxxrp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gsipqucxv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ghalmwkkb.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gnwrhqgva.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gliuepfwk.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gkwqjgwyj.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gbnccsxyi.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gpxmehwby.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gdtcskfcq.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gnulwgqft.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ghnrxgblc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gjqolabrn.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gxallfojx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gcqisscyg.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gwzkvrvdq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gtoeigbhz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gbmqioklk.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gdnkvsmxh.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gsebzstam.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gdqtfpvcl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gghwurhbw.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gfbkpskkm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gpddfpkxy.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gxiadgrvi.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gmubgxned.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gqrjlvuce.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gflupulke.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gpmtntbis.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gqfcrayls.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gjrkdqzwv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/glakrlccm.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gbvmphnjy.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gsstpmhyq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gtxawplhd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gdkjdsulr.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gahmlrvlx.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gvfjtwhis.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gniyqftiq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/ggwblwjtd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gyoasihzz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gqjrbpjdu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyazafjda.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gyfqjbxhf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbopzgrcw.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gkxnurevu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gybkbiwzk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gywkklony.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gflamsazg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gxfpidrqg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gadjpersp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxsbuhgfk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gxbiktrnd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gallaybok.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gjpblcngz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gvtgiemwy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gokvgymxb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gkoooiqol.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gnorhnbyg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gzldnlmpl.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcasjevph.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gfrmxamhk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gykboioqd.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gqsebhmwm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gsgcoadij.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gtgdbxenk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gkyiicqsb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gbuhazqtb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gbmavkhph.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gmccrkydo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gualcplmk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gcadtarbn.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/glnzwosrw.sHtML


<!-- 参考信息 -->