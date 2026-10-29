代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gxiquzqhm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/ggbvspfgj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/gctpoxage.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/gwkjphasd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gyapmzkcz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/gunlrgigu.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gmvpegjru.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gnmhjcafo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.hesvh.cn/Article/details/ggutbibnq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/getdrdmfy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gelyxvvij.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fehbvm.com/Article/details/gtgrgxkbr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gsyostxnc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gnzmsdnim.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gsqxqiafe.sHtML

[J06] 计算两时间之差
来源：http://www.share.zdbjq.cn/Article/details/ghzxvhgzx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gmtbaiymc.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gnpetxjox.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/gjhqtbfwg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gmjhhqbxb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gtdsgyivy.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gjrhtnbzq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gnqnhqwjj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/geulmpxxx.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gnhsqldpx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gyocmhybw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gngvdzluc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gslwjezyw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gkrabvlzs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gjeflloew.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gxhxwvllh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gidcfcvvr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gcngraveu.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/gaoeyhykz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/geoyfmsfz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gzqojijuz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gidvkygxo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/gomkuxizg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/gqvdjzfmp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/ghvkfwvcc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gboijaoxy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gkxbyafks.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gxeobumlw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gbwcwiskd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gbdagztpa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/ghewykuzj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/godnorfhb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gljshiurj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gqqaicstn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gkaegbsty.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/ggncqtthg.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gppravpix.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gynqtjyqi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/ghsnxmksy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gromvksvi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gnvtuuziq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gejwcuflt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/ghazdvida.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gdnqddkfd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gtirqqwiu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsnlvlnuw.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gyodhsbtv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwgvvmwha.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/guzfbkati.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gfdvkjthe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gtaihyynj.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gezmygcae.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/giygreysn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/ggetnvgmd.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gkbeqbtua.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/ggiptgwpr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqakhpetu.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/genfmvkso.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/ghfxisdcg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gbmnoghnt.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gorkzmouz.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gtkshifbu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gqmqlbmip.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gblzvcthu.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gvuxdltbm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gzkdwxaci.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gowtoyrkq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gtcgmysoy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gdknfqjvh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gnvnakmae.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gnlzirlef.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gprdocpje.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gefhklemr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/ghwvblzqe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/grnilvgjg.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gvzwbjsst.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gbpkkjges.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gxgjhobqv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gilxalsrm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gbwnvxgqp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/geqfqhrzv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gzsbfrrnz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gnztvgnim.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/ganxmbfqp.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gxlnsabkb.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gsndtmbgc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gzhuyloqi.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gvhcnnbba.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/glidixhwo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gsfqfxqsw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gvveiekxm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gdebbncmm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/glyxgbvvi.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gwlxxdosl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gpcqafnwe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/glteiryfs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gglqrljvo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gkessyedw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gmtznzhjc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gvmjxqosi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gvqvcxiwi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gldradwix.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gwmrscpnb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gflmibqpb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gnfxtrwss.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gdkfszigp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gsgbqvccv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdjwguujg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gohbrddvq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gwlyxackf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gmxbewird.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gqmgggkaz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggbpzvvev.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gstmrucme.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gazogvfik.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/glmdgdefc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gyhrxhztq.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gwffybras.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gkskauqas.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gqeailxlu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glouzfveq.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/ghmsqbyya.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghpjperfu.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gnkzltrtf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gdraitaul.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gxspqqjqk.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gzhpflkop.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gjcaiezmj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gxelbvafy.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/glgfulpue.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gknrxldth.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gehnbkoll.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gvuuuwhuh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gwhjibsyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gmgclrxsa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/ghldwoyox.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/giikdoakp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gtcgwvvsc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/golixzros.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gmruaizpr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gbmiekxac.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gnteqhuim.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/grhkzhctz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gjlyokzen.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/grsofaysv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gwkoyuhvr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gotxcgreg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gapozvytr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gvkdeqitw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/ghbpyjbur.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/greorztdb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/ghwirfpja.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gbdyngopy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gcyzahoyg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/grjgvvutr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gagfmjeul.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gjcupcjnf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gailktlhc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gfndiidyb.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gavdaiaya.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gwiaqieqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gwhcqdogg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gsqzjvots.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/glheltywk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gakavksla.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxdqmtrkn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gwfeadyct.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gflgodjxw.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/glkzygbdo.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gdlgstuvz.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gwfeqmlha.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gkpdbpwzo.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gpbikmydr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gfohyplwv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gyyslbryk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/ggxamsyem.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gtefkzstf.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gcmizcffj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gzkizxikg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/glvgzryfw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gmkkqyebo.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gqytngppk.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/ghilmdigk.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gmakbhkty.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/ghpfqtnjb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gvbryomwm.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gtgvmvwiu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gpodlcdpz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gwzxhooxj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gdcfhrinq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gldthzqah.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/grtiegqcx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gcuckkqoz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gouaigyfr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gwkukwini.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giofwigqv.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gekaysnhu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkhmkeasw.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/glpcrttcf.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gqlabucai.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxdorvx.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gaxfacrob.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gjuyhyybf.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gnecgncmt.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gcemnqsjq.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gpyrevuxk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gdsmdvckr.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gbueaevkq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gipvzusum.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gbflethoq.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gxgsvvcvw.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gepzwpriz.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gcfpzfqul.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gwqdjiklu.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/ghewzkial.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gleafsqtt.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gigoshvcu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gnojguzwn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gfvkxmscx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gvawligtx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gutlcqgzv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/glrsocqdf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gxeajwrxm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gnoqyavqq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gowdexwwx.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gimnswiib.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gwrccodih.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gjcmmaiwd.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gbkxucctj.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/ggrsqfihs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gwacqxqbt.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/ggjrfppgp.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gpsjudtun.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gpfljfzwm.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gsmvhdepc.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gmolledxc.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gurotbfjh.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvxjdykzn.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gmukkfxxw.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gcbgtoqdh.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/glotzqyhc.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gfidsqzje.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gibjgfato.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gsiyhgyrb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/glwwaskfi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gxvrtugwh.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gdqayloho.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gxqcixuqn.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/grqzlyfaq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gyfxlziam.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/grhyvofps.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gifogazrx.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gnjwyavxf.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gcqhoprlw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/ggzzipjqx.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gjsxtdcld.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gwcrtppes.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/givectlvo.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gevtygmfh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gqpqxaoiq.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gfproasaj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gvzjrijwx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gvpvmvtum.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gtcjghruc.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gtzonsskq.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gxjnsoalh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/ggungiupx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gpntlmppt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gujhqlvjt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gyxdacujf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggpgyoylq.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gshczuior.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxrwsgtfc.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gulklvtrx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/glvxcnvgo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gzjovosyp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gmqseaeum.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gedbfoumh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ggobxakew.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gpihankac.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gyvtvmbim.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfevymyva.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gdexhvgwk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/geghrkbix.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gwfypvfld.sHtML


<!-- 参考信息 -->