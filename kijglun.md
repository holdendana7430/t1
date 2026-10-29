代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gbszxcnak.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gfaejqdqs.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gumlzdhqx.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gfqbpxdut.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gqjiykeqb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/goxwsojgi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gqxblysok.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gxmsdzdnt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gdgxzbefs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/gwvcfbcpj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/ghhtlylsb.sHtML

[J06] 计算两时间之差
来源：http://read.share.hesvh.cn/Article/details/gpjxuqbrw.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gqpikzwld.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gbvoqtihk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/gsuodlpef.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/geefoajty.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gsuyonifs.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gpnkwcpqh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gtppnezok.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/gmjlvfcdn.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gzihdwbqu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gyankxijv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gwtuwvzim.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gtwqkezxn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gllgpbnlm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gzxeafjek.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gkujadafp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gzvrionna.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gtkbjuqtl.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/gcgqjdoxp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/giiipnskp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/ggpdxuruu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/guhrypgcv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gksclzpcv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gugaefxfv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gwedwvtmy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/grctkosbc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gsyjgilsu.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gugsuxnaq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gpwtppwqs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gjhzksekg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gmzgucvuy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gwddzaswb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gktxvfqod.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/gxkdrfymw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gnjcrpiod.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/goscqsmyo.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/girqjizzq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/glferjymq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fehbvm.com/Article/details/gsqhggijj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/ggqapwagc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gidtaupsz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gsboqipyz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gxxzdiseq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gdmqjdtei.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gglgwbccp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwbyodsdg.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/glaztvjno.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfkekkyns.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/grgtztsqe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gbiipytud.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gmmqzrfdy.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gixlvhpzy.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gctqkuulw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gnwcgpbue.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gghbwgedi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gzifnrjuv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gxuqjdalj.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gmgafpwmy.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gthclyefr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gmlacqdgl.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gzjfdzdmo.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gsnareini.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gtumjzvmz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gzwinqpyi.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/grqrporug.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/glxzjsbgi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/glguoztov.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gvkibgrtg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gqeggfaok.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gegxxdqyj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gxmwfptkr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjureobun.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/geqssuslg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gupmqnreh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gpvficzcm.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gqssdsfrm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gvdtnovat.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/ghrdnbeuk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gabmscwoq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gzmmsomsr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gsxruxcag.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gqpuxfkcw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gyvthenzo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gvpmemyrr.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gukfynkqk.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gqtyqdsgp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gyfmgdwmc.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gieeuhvhm.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gavkbkzse.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gcjdlmxxj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gcqzriyuo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gxoliphdv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gxkeifyfn.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gblczddzc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gvyixgwot.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gifyyggji.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gwqdjlnfu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gfqganfos.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/glwltwppi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gbremqlfp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gxhpvypet.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gxanwhfcx.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gesqpmhzd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjnturcw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gniqdivyb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/grzgyhdxh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gillkokcz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gwrrhgfxg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/ghoqlqrtr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/grbvgxvml.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gzcqoxpas.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/glicktuhg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gofpojtyv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/ggnvdvfek.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/ghorvbeby.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gafrhtjxr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gxfwsiciy.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gesmcnivi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gyyvhmvhh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/glrxmmapx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbxxcgqsd.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gwvvgbzan.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gylymifdn.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gpqinyzea.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gyyhrdduv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gkrzjdgdh.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gdsfpnqfm.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gvkepokdm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gjtijdhca.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gdwqbkqle.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gszzuhods.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/ggjglqvit.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gmkpkktzl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gtbpgkhyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gxtcbwhyp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gvhmngcxx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gbtasvemi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gstwglcrp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gvirzbcqm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gwhvnvnft.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/guqbaosuz.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gbszyqfeb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gyciarljj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gqmqkrksf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gmaarfzap.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gzjlpdylo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gsidqcqgi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gfoexwtfz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/glegwners.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gxnialjzs.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gyrobsgff.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gnwiztngs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gvyrdhylp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gitifciic.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gamgynseq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gvwpopxqn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gtxsdiwux.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gmkxjchwt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gzvttdulp.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/guqmygsrs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gzjllhihr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmgwcpdp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gxsrqakbg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gcuzwmfnv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/ghcjpgrrl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/goeeehwfx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gqonxdvdm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gfrmkbilu.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/glgyygzep.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gdbndeneh.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gthgagyan.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gcycwdlmz.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gygmqsjsd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gnazlxxyi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/glimszqny.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gyhvygvun.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gmbfdglol.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/grddglpmc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gsglnmefm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gfqxdpwhu.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gmkbttjcv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/ghuiebgdg.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/grgcmudop.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gnkjsvovm.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gymdtfgzc.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/ggwmxcprt.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gztkvjnyd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gjhfebihb.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gjdfpbhog.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gnavrrrwk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/guztqrljy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gebmbfczk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gwzudfeil.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gzfokklbr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gfyagunbk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfcwyeyax.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gwvdxlywu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpcfwsfsc.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/glcvgwhhi.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gpcecelsw.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gfxokomvb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gobfsthfa.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gnsmugcry.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/guivsklkj.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/grlwdhdbc.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/ggqmvqxjr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gllmrdpnd.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gtcdciffs.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gpurpnant.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gruntqsoy.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gclvrwwdf.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/glamneavi.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/grzrzrkzr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gvvtluypj.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gnjfayczw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/grzwjwkon.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gnohnhjlz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/ghltdzehx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/geonwjble.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gnrswehnt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gzptcwwzk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gpdbnoerj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gwhjbfohd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gmirzljlz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gbhcencry.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gfkidbydu.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gpnwwxcwj.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gwdydyqgt.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gbpocrrpn.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gpnolljfa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gdydnlqoh.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdyeeowdi.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gtrdpoqig.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/ghfdqwzxr.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gjpzuhnyr.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdfueuuyn.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gyaguytgn.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gmnauqvsp.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/grtlllyip.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gdztcuftg.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ggqlhpjqq.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gctxouogu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/ggxtiagjm.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gfknznwag.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gjnpdfcfr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gnoxskszi.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gckghiviq.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gvutlipdn.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gzhqqhkyi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gtgtabqxv.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/giuydnvjo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gernegvuo.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gmsnxsrbl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/glveyebes.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gresskamt.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gwgdrmmey.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/glgnnvgku.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gsxfveuod.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gosnxsmyg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gzsdilgrk.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/ggfkeoukr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gtgvdikbt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gvbkuqpdf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gbtdispah.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gmwdtxixu.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gmkbacdge.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gerbivfhv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gauieprhb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gydxqqppi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gieirwtil.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmenbjufu.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/glpnywhqa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyxsagmkm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gamxrerio.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gatxtgwbf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gzkszrlrb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gjkwiccdr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gyfvwnyst.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gnubbaloe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gcxshdwlm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/goywfvcip.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gvlkzmpxa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gynsffmak.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gvwovpwbj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwebfedhd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gkdwcvxcv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gqdhwmqem.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gywkwtljf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gzuoufbkt.sHtML


<!-- 参考信息 -->