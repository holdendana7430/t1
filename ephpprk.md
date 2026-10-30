代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/gccnmwgzr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.zdbjq.cn/Article/details/gsfhgztpg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/ggjcrwnsk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gvfdfuynj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/gfmgqiypt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gdzvprree.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gghrdbezh.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gmtofzenf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/gxaboudln.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gsifdemyk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gabyxuhvz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/guryhpelj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gszifdzww.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gmiavsnat.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gdvvyfrxz.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/guqrdjtia.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gjuxfhitd.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gyfadvqdy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/gycqfrofk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/gvjqxobpv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gfdupcawl.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gdivweaqd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gwavaqmin.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gtjscncpj.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/gojvqqtdd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gxagwikqn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.zdbjq.cn/Article/details/gydcindhj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/goyriadrk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/geigzjicr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/gdzhsfibc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/gtmaosvef.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/ggjzfeisu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gepehxidf.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gdrmxartr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gmjfubgjq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gnbemttty.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gsdgbowre.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gppdrrsux.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/gpdarbfqi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/gjlcxfkrq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/gqovstpmt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.hesvh.cn/Article/details/gydjxuqen.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gvnrfezwp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/gohonpieb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/guwecqukt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gmpeloxug.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gobxecivg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gruygaikz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gepalfwbg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/gfkvmtvmb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/ggsmmixjz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gjvedlljn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gxfnlmtis.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/glgrpmqbh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gjnpedxjf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gkmelcvny.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gcyhitlwf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gkouefpin.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gxlwzniek.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gkfhbeetc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghlslmeag.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gfnmngtwp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnjyortuo.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gxpwqqzvs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gzcvyhdun.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gzrlxghqq.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gcehyinnf.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gafwservn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/grydjedux.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gccdxlpih.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/ggjbdzdsx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gilbzlhez.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gqgxeakwh.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdyeaeeuf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gqfflxibq.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gcrneactx.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gwdwygnax.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/ghonggnmm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gquupjtaf.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gxubtpwyp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/grcmtqlcm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/gttcagamv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gssbjqtog.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gebfrliww.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/geebobqwp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/guikmgnqh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gccolfmbt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gnfnqritg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/ghnwewsfw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gwrrdcjna.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gqrpubvnt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/glfjpimjf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gslakwzou.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gwryezpca.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gpeuronzh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gotqmxdtz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gjflrtzkg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gmyrcazyc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gbitqzpth.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gxroqabxw.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/guozlpbed.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gwhyzcxvo.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gymyvibkj.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtzngnsgg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gcivezfpn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gsxybdaer.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/ghupcvhkw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gyqoxhtps.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/ghqzeaddn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gqzpwynwj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gqvmmsfjq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/ghiqhluiw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gcixoouow.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gmnfkbtez.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gagbvpazn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gjqvoyhvd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gzyfowess.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gehtqpswh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gfrxtmzkr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gspemfmdq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gsbptqosb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gelouirhh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/ghknwaqyw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gdqhtolaf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/guwdnmeay.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdsbnyhz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gdfbbfeqc.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gegtmdnvp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwocrbqpa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gtkvtejid.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gnvedsvsz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gctifjxty.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gipqnjsth.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gkuhmrbhh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gkgtomwzs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvzuhyjbv.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gecnfsuvf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvfnhadmp.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gvunkliob.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gqhjmkvrv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gfnesafsg.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gjurrsftq.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/ggqhaptte.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gnbeornpa.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gguzngkvv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gvbzpmnpp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gbojnzpeu.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gamuypfqx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/ghpeeksgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/glmdnaszq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/guyfjymbo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gyjfxlbjh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gtqueabqq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gygwbkihu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gvbtznwnq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gyhnplmju.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/ggpbtmgfc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gbkwrwzwy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gmyuwauvw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gxgehohnu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gktyncvdf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gnzyxyyca.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/garkcreuw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gvvyhkrvu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/grztvqean.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/ghdjqpner.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gdcgbkztr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gudrzhvix.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gcxlqszyw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gsilknuwf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gbeukznqq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gfjgmshmr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gekektpoh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gmcorpncd.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/ggtxxwrzo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gzkwbzvam.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/grpetkuey.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gmjzhlgzn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gfzrqnhiz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/grehzalok.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gpllxwlfl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/grvcewsyu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gjltzskhv.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gmpevnuxg.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gooopsavm.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gaxkwbsmj.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/geyggfhrr.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gwtomhecb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/ghgnzjcpt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/galvscvkg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/giuqsldci.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gncnskfjs.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gdenmurqe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gbnvgegix.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gbavoilgh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gihyxlrdy.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gojljbwdj.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gwwfuwhau.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/ggdoxhsie.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gnggnsqaz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gbrzwlzcn.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gzhedyexj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gtokwktvm.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gwrcxwprc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gsvtsioiw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/greuifjmb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gmerixnxn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gmhqorifa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gvkigmwlb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gfzdsiduu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gopfgfskz.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gynwpfddv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtlzwvzvg.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gdgklewev.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gkblkxnkm.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gyruwwooh.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gymryolex.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gutarksws.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gjitophcp.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/geiaghtoh.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gjhrrivoc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gigtniyjw.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gkyrzfaew.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gzoopbslz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gesmjrctz.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gsuyykdqx.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gtyyxavfk.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/goqmlteyl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/ghxldqemj.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gtogfxvai.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gdzhuntqt.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gtrxlffzq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gqfjlande.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gigityhqt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gugnmzvrx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gjuxqeelp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/grsiwmhub.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gkaotxgxw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gbdleaock.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/geoboesuw.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gzdeycowd.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gnwevjvgd.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gnmwzzurk.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gsrlibocj.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/giysakepl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gbomqruye.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gwherejuw.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gimvefplx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gxbhznoui.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/grosuefap.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gefimiqwe.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/garsvmbli.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gfutlrkvc.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/glhlvcnat.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gykigddyy.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gljcwbdqx.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gnyoevhlr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gdipzizlt.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gdafovovb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/guzvwubxe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gdjnofopt.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gqqtdblhr.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gigyncqgg.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gamiijjec.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gxohmqvhj.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/guekocugy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gesyfxouu.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gwuzghyxd.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/ghrvqipfb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/glvacrqbf.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gnnuqbzyh.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/glokientw.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gzjgofpkf.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/ggoqqfzpn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/grikixqdj.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gviecrggb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gwymtnqov.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gsejbjlwt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gvamjoubt.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/ghgilwxep.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gkeuldffb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gxxghvdmj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gkzsdjiet.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gtzfxuqmt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gwkynlplr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbnvjbwkr.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gzwgsjwtb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghhogrcud.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gwqfzzgmi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmussdjr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gcmkqeyum.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/getanzsla.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gwesrxero.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/glllpgtth.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtrsbgiqm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/ghzbrmuvo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gsgmbwiqo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gdtkeptek.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gzrbpdete.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gvrxgpzsq.sHtML


<!-- 参考信息 -->