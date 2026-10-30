代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gsawulqrt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gzokshmsb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gtwbfrhyj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/guftiwvsm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/grcqetabi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gkxmhnemz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gdxenznfy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gumakpxib.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gdxmpcevw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gjggmzliw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gqeiukukw.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gdlkogzxv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/gwuhyvkcm.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gmmkprkib.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/giybvztes.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gghpxfnst.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gfouklcxj.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/gfdkeodba.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/ggoyxfvqj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/glipyvcug.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/gihyjnlmv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gzbwvaeig.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/ggiowmifo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gdnebcjkd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gyyqpqgkz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gcmvvylzv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.hesvh.cn/Article/details/ggawnnyav.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gqqisjikj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gfmhblphu.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/gmckjhsiw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gayeailjr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/ggldpdput.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gklzzvztm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/gjfnpqcmd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gqepzprue.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gpgfmffgv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gpxqcwgyz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gwzutauqg.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/garawzrdz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gdhdhupuy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gxdkzhkzu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gflxnotft.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gcoukfdok.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gdqsfweqf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/gqzrdoqyk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gzlvaquxg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gbucefwil.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gzvfmddxl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gmccfqavi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/glcelngon.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gjsejufef.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gytslciih.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpcsftlb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gsucsltnt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gmigigrqo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gzoqfqcpt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqhnovokk.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/grzwcusay.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwasshhtc.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gfvfmbynk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gmlmigsjw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/ghkjpzzwb.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/giswjzome.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gkjflzbfv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/geatzirkp.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gptresihm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/guwnbjmra.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/guxwfjtmj.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gimcgizqr.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gznqrxxmy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/ggkliaolh.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gkwrekyao.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gmtlelsby.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdphwjkn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/grbjvnfsg.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gyhxqjwux.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gajhtayri.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gmeijwigm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gkghmmlcg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gpoykcwrz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/grzfhkzfa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gbhhegvnz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gklipwmjf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gifowmpwq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gxjnlmhxx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gucehfxvk.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/glbjwradf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gdtcdfqil.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gyqvfzpgj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gawnofrwq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/grftrxwib.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/giwhtxjeq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gmgltcxeq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gcpjpxbrr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gzlyfzylf.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gxocpqmel.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggbmgpuct.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/geykpsjsi.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gdkhhfuox.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqovdyuyh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/ghaohpasu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/ggwtggwqx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gyyssufou.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gjwqjrkis.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gnthtyutt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gvphrcafs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gwkelqgnm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/genkcckpk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gqrwbnico.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gsenkmkko.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gfthuyhty.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gfkdcisyg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/glwidzjcv.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gnjemkoyp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/ghayzngcv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gnygslppc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/getnrekpt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gmpyawuzt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/guqwjlzhy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gajibqeji.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gxyocwowd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gpuiiyyts.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/grkvqhpue.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gijbwpioe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gwmdghhjj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gzjgkvudb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gaotbocsl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gfsvfzdrs.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gzwvnmuvi.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gfhbtlbxu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gjpbuangx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbebolhlc.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gnssbvbdg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyomxkomp.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gsqbmaxgc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gogiwjizv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gqrttilex.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gzdamvgvc.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gxehocwaa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gsikcuykm.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/geltenkdi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gseruiiio.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gulsmwslu.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gxolcwvjf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/guaidsnei.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gzsdcpmud.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gbqsnzmid.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gbhuvkhge.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gsqnwifax.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gjtbajgxm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/grzrtbduh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gxzvfgkns.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/ghqvwjztv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gvzrsiwss.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gnhuvjzcv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gkvveqcql.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gnyqhxpfa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gnmuvlzlg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gcblqcoht.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/ggjmkvurd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gkybyqqzs.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/glgdxrrly.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gibhybnqd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gnlobysno.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gfcufzqyq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gfjfyfpeu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gzwushvjp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gaekpkacy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gplzzsdgz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/guzobglwq.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gwrstpnjf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gvxsvdhqv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gbssxdlhc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/ghfglzoml.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gwnjvrpbp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gvxzcnmii.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/girpgvtlv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gridytyye.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdfcojola.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gabshebsc.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gpradnyrj.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqwkojqp.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gnnoglmri.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gahaqntyj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gklhrxsna.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gbcpbsbfs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gsbdjvdtt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/geazycvhk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gpefkgcgm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gyzcjqrco.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/giucfbuwb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gxlajxxmz.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/glypsculy.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gfacjewue.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gkamajlne.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gvokdzbqi.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gzdvlvkek.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gsqoztwev.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gqpbxtzuu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gkawrgqws.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gxcyhhuyp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gitotxjui.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gpaupffsz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/glwomgmcr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gspawhoiu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/glnlkjule.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghiiekquh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/ghvtmkqlf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsmkfqhpb.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gzfkdkqeg.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/ggxmmdnos.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/guebwgjlc.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gpejhvtov.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gcggqfwam.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gaalxuync.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/ghcotznvz.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gotaptsuy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gvgguljau.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gfzzmmkus.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gvluouama.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/ghemkgshf.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gfjgxuflh.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gnubvdukc.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfnwgbqnt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gstqeudqr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gfvifwnwm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gxztxwhkv.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gmgpdacpv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gdokjtywg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gilrtbajw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gdlqavkid.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/ghbktnmob.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gpmgzbfcv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gycthtlof.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gjfdtaxli.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gnekjecvy.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gzunjsljb.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdrupazmx.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gwpnfrpzh.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gdnwnafzl.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gavtrdjog.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/grcxvuvkc.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gwqoidqdt.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gpqwjokuv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gqpjcpxbx.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/goiekewis.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghqemqysd.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gbwkckxli.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gedbnikug.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gicxeohsu.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gegzolpjn.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnlkfnroy.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gsedtrmpb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gdqvktika.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/glfibszku.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gcyzgpwaz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gbppszros.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/ggubhntgr.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gscybbiam.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gcolfbvzk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/guodyzevq.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gcxqruutx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gfgqcahyi.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gzkviagqa.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/ghtmiajlk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghpwbmomg.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gufsepzxw.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gpkgpojqx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gpeiksmsy.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gqyfqabby.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gmfbpehjj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gnjncufek.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gacviafje.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/ggjtgxyad.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/geufxkgpk.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gwopcbxrp.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gnddjxvrs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/ggwmarttt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gzlpngrqv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gejothnnw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gaidenmwu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grkgwnowu.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/glylbbhqv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glbinolig.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gcgxglywy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/glyyxwgvp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/grkjqxlni.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/glhowposo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gkehbbbwr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gdpjowtdw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gghqavdpr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gfqxnxqvw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmpwibnlp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/grsbxxdkx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gpjlbkfel.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gjickefri.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/goqdbbunv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gjnqyemty.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gciauydzf.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/geolyjdmg.sHtML


<!-- 参考信息 -->