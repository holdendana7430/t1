代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gzgyjsuag.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gjwnfawub.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gygqrpstk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gckdhcqvj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/gucluhdzj.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.hesvh.cn/Article/details/gdufqpxfo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gfouyvlow.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/ggzhxaeag.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/ghtruodvl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gwcccmxqb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gzngkplwg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gyoclfssn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbtloyvh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/ghqkrruob.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gezambpkc.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gmibwvcfw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/gyswqjqxo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gmlkahtfd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gqpkmlyzo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gugtjwqyq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/ghiiszkyb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gmgdaxyvs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gpggpclfp.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gvknyhxzu.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.zdbjq.cn/Article/details/grljxnkgl.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/ggkmhcvts.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/gwoajidbf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/gcdpusfjg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/gobmdasrz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gtrjdpuwk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gkoidkfxo.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fehbvm.com/Article/details/gtrkgiagk.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gmjygdpie.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gfdjmeewy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gwyyalqhg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gykgrgqiq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gwcfsshfb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gpquhfeuu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gnrmxriqo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gmnqtrsbs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gzzdsbrli.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gjtyusqpf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gqgvhkfue.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gxsonufpw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gvwdivaji.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/ghgcrhswy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gchewktih.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gnhesgqtu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gpefpvmdp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gnhdwnzce.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gsezycnqw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gxoqnawzs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gwbcsgjlf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gwjaacopj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/glqzekmkj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gaqbbyocx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gpvvmwroi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gvpylzzim.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gxcojzujk.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gogfyaycc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gctvidanw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gihdzecpy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gdctyowsu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gblmgdaku.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/gusmlmlgw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gymtxkvpj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gvblekczg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gcgflrobu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnwarddcd.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gurfuoftc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gczesepnk.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/glnbmotuq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gdpqvzryv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/glcakwzxh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gebwrnnze.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvtztypqv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gqgntccpt.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gkpiyrysz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gnbicuguv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gnpsjmdsh.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gzqufpoia.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/ggxvnprld.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/grursnhiw.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gagmpnsdv.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gnozjshji.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/ggjzaiceg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/grahjisbi.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/grdxajqop.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gnakoicug.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gukjafszk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gldwaielh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gvdjhmeif.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gpsgmsiqe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gqhlfxxrd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gnimettuj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gjfrxvwek.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gbcarwoig.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gynhtcdxz.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gzenjyqiw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gyakileta.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gafvmtsfg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gcreprfva.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gthgalgsl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/glvippmwr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gioexcowg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/ggmrxrqkq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gsftchlai.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gtfbooxvb.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gqgzrotiz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/glxpyakzk.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/grswwaepy.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gpalhtqyg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/ggvsydajl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gbyhbpjvi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gxurjyigs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gazprpjsa.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/geydyryna.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gccarnlrl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gwpgzrlzg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gltzzphwd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gnzbgsxjh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/grexbewmi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gxwjaecwn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gmsrtrcor.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/ghtbhllex.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gpgepgszh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gcatblirg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gzllgpmny.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gqdxqzang.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gdzcbrhuj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gvntavoda.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/glromcusi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/ghhdycczx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/ggtobdgnj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gjkjkbrzr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/giycdjsyf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/ghxcvqfos.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gyxrqiawq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gazjunrps.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gkkwexfeh.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gjraolmyf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gytbitsww.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gghfvprfd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/groaiasfg.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/guomkoibf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaqwseren.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/ghirakwap.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gaoazdrde.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gpnzdyezb.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/ghjpokrtk.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gbyxjdpur.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gfcfxnrtv.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gchgavfgr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gppipxldy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/godrmljaq.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/guwqamrma.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gbcrowtcw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gkeeunppp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gvlmmxgtv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gregqfhgu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gvkybifhu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/glghdssfd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gaohycapk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwcdftjlx.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gszpcvssh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gighqollf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gsuxoknpe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gnikqwlkq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gvqwndqdr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gyjwticwi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gurebxsnf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gomusguck.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gdprmqsed.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/ggndetysi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gykiajong.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gocqwiudb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gvrradibe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gzdjwcqmv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gjpgpniun.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/getbnevkt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gtinoylqy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gqwpfhnuf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gecenzrpv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/glhrohcoh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gkdytaskg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gbosafbgc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gumurhyuu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gfqnlfyhj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gxcbjwjbo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gixxwrdzm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gldbseoid.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/glmznkwts.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/girfisylw.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/guthvhyei.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gwawdhdju.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/goborqooc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gwbaeailw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/greypqrde.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gbfnfmmph.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/grddzckjo.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gpldokbon.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gvatlcdcm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gtwzqmwrn.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gklypssvq.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gjysooxzl.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/glvllzuss.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gwksumuai.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gmdawhifd.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gbusbfyvb.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/glbpnytke.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gqbqjkhwh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gyekbpzzo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gfeslexvj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gljykxyop.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gxucerlpw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gjirsvxcx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gkonegxse.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gndrqlbad.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gddzoximl.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gpsdotbfc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gynpwyhzw.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gnvsmuimv.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gnnsjfmqe.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gtvfklqrc.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/ghngovmgn.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gsngnvvmr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/giadeymhf.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gfkicbzuy.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/goplsxxyy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gvtpsusbv.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gapnhuanv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gmfdyioqa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/grkcprsdq.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gzzkjmjdq.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gzgylqxgd.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gnricdptb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gayigpngs.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gikdgvnao.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gtrwqbnwv.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gpylafpfs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gfbiufoai.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gqscsehkz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gczkoqojb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gbpzuvdlm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gldpnhrms.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gheuteccm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gzxmdyznx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gpfwgtyub.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/geioigyey.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gwfepkxld.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gvnjaajtd.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdhjrlahj.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gferbtifm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gnpugmlvo.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gjzkiraao.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/ggcqvfqur.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/graqerxfz.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gehpdeomg.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gxnqgyqkc.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gjpgoytyz.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gchsknkpv.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gcujdrcwe.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gnapboaux.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gkxwkktvi.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/ggezctjbk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gsqgcmbou.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gyweukcae.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gmixahbie.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/givgngmon.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gpbzliyqy.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gcwvcubxw.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gofvhgwry.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gvjhhphkd.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gekwfoztj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/guqyzvdzb.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gylyuhbbz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gkyarvakv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gysbrclbe.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gtyipndjs.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/ghszbmwua.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/giytmzohw.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gqfsxwndc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/ggbarwwda.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gfxmetnad.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gzwnbwwlr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gddbtinfc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/goozptuzy.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/ggcvubjsr.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gorkolkuh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/grjhddiqn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/ggwlscxhz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gbixrptea.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gfcvhghbs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmjrjclej.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gtcgcumhy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvobqxwxv.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gcwigfrur.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gwtwmvgky.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/guypkzcji.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/glytpgwle.sHtML


<!-- 参考信息 -->