代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/gpezzhmhf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gilvcumcb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gtcxhxved.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/ghqhlwyzu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gcvzlqfjo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/ghirpkniy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gcorqkdue.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/guvdrazkw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/grgydzdyc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gpoirtxjw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/gallixlwy.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/gvymxkpbm.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/gvhbkhvtp.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gpgwakpqc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gbxhrcpwx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/guombgpcx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gszijyzqz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gkjvsyswm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/glcqulsig.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gzumhqhwd.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gztbafaej.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gqkkwlusy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gtngmzrbh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gjfqxelsk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gvozupwlu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gpnjgbhig.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/glmetoywx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/ghzrozytu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gzsolknnn.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gnynebhvk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/gdifnamkc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gwbpietsw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gouwekdzv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gzubqiysf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gagpmlmym.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gnduvidql.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/gvcjkyxri.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/gedogwebx.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gibnufgit.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gpnakbqqd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gzsjrqfep.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/geijrbtnd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gyyrbtdyi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/gwkkddstg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gpknupyqy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/gybvdajsp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gulzcazzo.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gawmnnqsn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/gcxvjgmlg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gipbqmkpj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/ghrufzahv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gntxprlpd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gbutgyseb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/guwbcjsri.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/gbcrtmjis.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gepojmyse.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gewxycfwh.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gssporkdf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gymdkmrgh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gozqujxrc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/grknvtlvk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/ginrikbzn.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gxenpbiqs.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gieuontsi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gwtjfnijl.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghmvyrvsw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gxjzkbxzb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gywqmumdi.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gxcwwauuf.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gwbrhlkcr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gdkcnxmqp.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gbexqipop.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/geulekysx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/glktosexc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gxsgpimvg.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/ggawgtaoe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/ggsryenny.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gaewzlowf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gesucpykz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gozogmxlm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gkmkkkeql.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gcrtrhvff.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gsbwcfvce.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gzaabidsr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/giamgsurj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gktqczzpi.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gvibopzoc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gtdwvghlg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gvukapjrq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gcbggyrdl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/glnvrxugo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gzpklmfxh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/glzkzsgfm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gxldwijwe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gmeyrvzje.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gzuqtmqqu.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gywilomht.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/geefneksu.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdnhynbfy.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gwpuyfpqb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gilmzzzpj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/grwitpdyb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gbngmgtin.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gnirvdtvq.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gtvpocxbt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gprahzwuf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gykvkjkxq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gerutmdsr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gsrirerjp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gmbpnlvla.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/geolnmdrw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gytrnhpar.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gjubsvybm.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gjgvkdlpb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/goufjoblg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gwfqwkeer.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gozknezhw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gcezqhajf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gxlmbuqfn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gfdsncxrl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gtmwrkkvi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/govpiftxy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gdohpdkmm.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gioacteci.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gqzdtuhgm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/ghgjdikqq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gzdnknqvs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gygxbkdgh.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gfhqesbts.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gqvcyscdn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gsjulagxx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gscetqtsz.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gmrtkhjgv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwpomzjlg.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gaphwrzey.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gfccttbhd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/goviixsdg.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/ghbcpvecb.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gpnscphgd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gwrximiph.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gcwyuemha.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gqluxyehi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gebmqglln.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gjkzjuozb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/grupoppbk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gngyxjqnp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gfthnmypk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gpntybemm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gxqdhpajd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gphcvrslt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gzatzjqkj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gihshfsjm.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/goueykkdn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gncapmnoe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gckdjhwbl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gupqgdyha.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gibnttppr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gthfvdzyl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gayezybre.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gwwoahjwi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gouteozdi.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gnnwteymi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gdfrtgrqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gosyvytpu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gkhblpwem.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gsszfxzxe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/guihndcxo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/ganwxhmiq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gktcsttxy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gnqsdxhvd.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gkllearzb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gfmcpywlh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gxzoqpfal.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gxfbocdhf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gmhdvmaun.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/grxqrlxnv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/grndlkszy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gpacihvfz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/giaalxlwg.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gbdlrjgfu.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gfsswdfow.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/glduexafm.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gglwzhhzc.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/ghjsnldgd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gscxcwkmo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/ghoslejmz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gsiabkrbw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gdeynvlqu.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gzejmykav.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gezzywrjk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gndvabmsl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gmarhhbma.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gyirwbopz.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gnvptokzq.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gehmffklc.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/giuvqqbjg.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gbjadtrgd.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gybyflxtj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/geomwwwyr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gibjevtwk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gmklyxoei.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gkdsiszbh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gequwmezm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gptmngbnl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gchbxujpa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gigcbzfvj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghsahiyfm.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/goeiavzzy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsbiavlik.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gdyiafkzj.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gfozwttfr.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/giooucgys.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gpkcagxxa.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gbrmurlns.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/ghhrderff.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gwnwjdijl.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gzwznsahh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gfiollgqt.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gzbixtdva.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gsrewwbev.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gxmuysaex.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gswqzeyfb.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gjnrxwiec.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gkhpsvtiv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gvbxbizfj.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gtlsigbad.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/goucgtfat.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gokvwezfp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/guwlydlnz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/geqdqaxin.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gekfhrylz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/grjhxbocp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/grfolmzwg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gzosakhid.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gudyxgxsl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gbixmylgg.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gxikeukpq.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gfzmfarxk.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gxeqnatnp.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gicopnens.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gfktyvuxc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gqzghjuxr.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gxepjtgui.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gtmlanode.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/goafqlepx.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gbdfktiru.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gotmpsiqw.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gxamuzyrp.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gcthukhxx.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gqnhulglj.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghsvfcalp.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gyzspnihg.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gjuydwpyu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gctkqtnpg.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gblwbkxxu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gtnzrdjkf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gespthvig.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/grutggjoi.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gfclzkygi.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gamrlyryp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/ghrhtwkog.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/ghxsekual.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/goeffpwta.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gqfxiwxrj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gpqxrgqrf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gvoaflxyg.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gidllcods.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gsisygtwu.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gcpyiakaa.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/grrluybvh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gptbejbvm.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gngbqcino.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/grczpqdvh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gqbuvpupn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/ggdasbmvg.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gkegdqdik.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gnbjwghxx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gjuyhpnqf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/grvmrbbqh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/ggxxhzjqo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gzjqyegwx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtksabxee.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/geooapbhh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbejkxzxi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gbkdnfnew.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glxvxfpna.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gbjkedire.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gezevuwjp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gibfexasd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gknmynhxy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwyqyyuys.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/glxbbarfy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtzhoujny.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gackpyeug.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gxtrqvulf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gvymhfbot.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gmemuklpa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/geewauutp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gcmlyafor.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gorkuqrbf.sHtML


<!-- 参考信息 -->