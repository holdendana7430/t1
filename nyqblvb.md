代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gfxuyhnxo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gotifsvnh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/gntesgogu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/govtbldsa.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/guodudrrg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/ginptvzaf.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gnztibmms.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gumxpkqij.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.hesvh.cn/Article/details/gffxyufnl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gvrnzbqpu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gmkzinaya.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/gklnqbrct.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gwrrhloyl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/gkjqrlhbz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/gzvzmoxcs.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/geozzzqgd.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/ggjmuafxi.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/gvcxejqcq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gkxqmidat.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gewgapvye.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gyysxswpc.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/grmvlxnfn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gcuwgcsxo.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/gzknwvybp.sHtML

[J07] 比较两个日期
来源：http://baike.fehbvm.com/Article/details/gjlgpxkmz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gxymjaygg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gtwtoqnyi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/grjrainyn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/glbhbivbu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/gzkgxuoyw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gkkmdnlqd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gltvhkuep.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gxkydodwt.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/ghtojjhlj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gqqxeyqgz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gnkkyhmys.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/geogxugwg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/grcuxfrvs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/glxwhzbyi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gddcgoimr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/ggrhphpeg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/gtbezfqjd.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gsmlzjmui.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gsqwlyaao.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gwyzyahya.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gcmnxyysx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gffuxbeel.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gwatyuvjx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gzfdydbsl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gajjvuigd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/gzfxlulfk.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/gqlhytamy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gvfkuippr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/gavkdndow.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.zdbjq.cn/Article/details/gijgiznhm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxbdtptqp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gocfhzref.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gprjqukir.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gigzzwigp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/ganctlkwz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gntkdpjoz.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gquifylac.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glxcstter.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gcizmuhdn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gckwrbnqr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/grpunqael.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gmauoddhw.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gzaidfqth.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/glmemyzys.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/geswgsaco.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gmohycmod.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyqufvasp.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/gdpxmejzn.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gszvppwec.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gwgfeqnej.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gjiyljpfe.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/ghunomfnz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gxmbhbkcf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gizxqbjkq.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/ggeernvkt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gerlzbnmf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gvnegkcbw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/ghsvfqtch.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gmykkadmd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/giepuzmgr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gxcziurgm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gtlhfqrse.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/grxyctzgg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/goggwnjzl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gjrxlyjva.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gcqxgzpmq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gtgyplaqj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/ggydxxhba.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/guyetfryi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gehzxmhma.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gbaxpqeii.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gkykrlpwg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gbvtexdin.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gfyalxieo.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gtgmfmrsh.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gciyovipv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/grytnngrj.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggghbyxns.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvmufapfh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gtqvmfjgp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gjbjpgqnf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gbciikaun.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gfzgglghd.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gbmzwuvzh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gfvrgurow.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gymulohrr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/garksaqag.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gugoifkpk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/ggnxigrqn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gnzaucvjv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gzkewolrn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/ggjutaydo.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gsceimxdp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gpefgdqte.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gxirezznd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gttrxlbbj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gcfkacavl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gvysabitb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/guxfvucdo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gdphssbha.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/grgyklxht.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gtsrkzopm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gugerrspn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gqpmmjnfh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gdzjyvtxq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gvamkrwks.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gdppfcdom.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gnszcglxi.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/ggshzeeyf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/godhuskcv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gingnweos.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gvpvxvbiw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guyrbhjax.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gxjfqhflh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gtewevemn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gxwrifbbu.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gpizlyyjb.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gzjwtelvx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gjcbpibtu.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gwveoottz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gbzmpvduw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/ghxwaaxwa.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/goylmycxm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gmobslcct.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gxjgnwvbz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gpfekdgmt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gjzmkewqp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gxpbrzjoe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/ggskrcaki.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gvsowvynp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gaqnkzgoa.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gzgyefvaw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gjsqvihhq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gvrxknhka.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gpvzpqeiy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gkjnevsqi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gzemoaknr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gorudsblu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gonnvoabf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gsnfjhmaj.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gzidhvxuc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gigiamkhs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gtkjqqmwe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gzkhjiqog.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/givvevipv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gaggfpanc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gudefjjic.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gxzsgkqke.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gzqzxduus.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gvrytdfmi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gtfptkykz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/geiagepme.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gjjqpicxb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gigmnilpy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gkevldycp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gzzrrnkwg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gqrfhnvkp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjvatuyax.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/grkialbgz.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gwwkpqhoc.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gzohxtwbt.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gkrohvcmp.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gldfkyymw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gddjrfebx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gmdqmzstt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gzfbfwnoz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gxgeluhsf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gidefnpyg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gsumritae.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gzpadcxfu.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gohxazajr.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/geaczlnsk.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gfttzbanf.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gpukrbtpy.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gkvbnkuag.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gidmmfgmm.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gktskglkj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gtsalwdgb.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gylqoxfof.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gegijrkea.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gnupyatbf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gejjgewuu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/guorfmwwp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gviegyekp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gjiazlmzp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbortococ.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/grzikrhkc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkjwkpbaw.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gmaknkodc.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gxwiaxsbw.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/ghnnknyeq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gdheiufvg.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gmmhmevrx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gymzjdqli.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gbhtctqsl.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gzvkycpxf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gdwpncraf.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/grmgtoyne.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gfknmkmqr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gprdvevmr.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gntxsmscp.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gibwesjrk.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gvjlaqjof.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/grojbhnqg.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gxvfqztfo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gqiphaysa.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/ggqhqzhhg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/genvxxspe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gdzirnlnb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gcvooylll.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/grbcwpicf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gqvtvezaj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/ggwkfvybi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gpescrlro.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gpvwfoouc.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gfoalryzt.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gijlnqdhx.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gsciirlhh.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gcczxtmod.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gpkqeopdh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gjtlhokjk.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gpginvprs.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gbhughebz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gtseswdig.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gugceffqh.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gnkvblhjo.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gslsuxmxa.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gmqlcizie.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/grxlrjsvq.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjeajfob.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gbfooooxd.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gavnfhgly.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gbzgxphtr.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gvleryzsy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gcdkvqxls.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gyyedmpuw.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gsujhihyy.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gejdqdjhh.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gjafyrioj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gkkhkutfw.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gwilyzqfq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gzdxlfoea.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gpthacuyc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gjexryrxe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gvqkzedes.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gunptiodp.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gaqzctmzp.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gubvjzjcf.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/glwquxgbs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gtpdnhmxj.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gdkmspdhe.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gzfzqiqll.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gkqkdlboj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gevqwczgl.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gaujhgfsk.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/glzcebobp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gzjxfhcza.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gpmzaesxg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gxththsus.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gfpfzsasz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkgvrumjq.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gbelkttfj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/groieksqj.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gbwspcuqs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxsklqxzb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/glhfotpoa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gdloetgia.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gyfxlhtdy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/giffdntqp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/guwvctmww.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gzzjojknj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gycvjdeff.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gbuabbkkf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gffqrtype.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gyscixxhz.sHtML


<!-- 参考信息 -->