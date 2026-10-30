代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fanxiaobao.xyz/Article/details/glyrgycjy.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gowlkoroh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfhavpay.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnanmheks.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbquvbeqw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gffaefyhw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gscithhrn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsqsmimp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbansgtm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhfhptsc.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxrfcham.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwjcvuju.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqxhhevm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkonvwdmo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsohrurt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/ghorvspnf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkebbsqq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fanxiaobao.xyz/Article/details/gbfwceozg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuwichhc.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldhybpsn.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fanxiaobao.xyz/Article/details/grpsrdhao.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fanxiaobao.xyz/Article/details/gcadooedo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fanxiaobao.xyz/Article/details/gofurjrhu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gmeyvyvdb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/gomrzdccb.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fanxiaobao.xyz/Article/details/gtgaoopvg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fanxiaobao.xyz/Article/details/goljejzom.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvwpwvlt.sHtML

[J07] 比较两个日期
来源：http://blog.fanxiaobao.xyz/Article/details/gdbwvhttr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gmccgxuyd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fanxiaobao.xyz/Article/details/gonxnnkir.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fanxiaobao.xyz/Article/details/gxbwpdjjw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvqgctrr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzflkdxz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofppmxyb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjflntcxn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvwumlwi.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fanxiaobao.xyz/Article/details/gybezidgf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fanxiaobao.xyz/Article/details/getkfscyi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fanxiaobao.xyz/Article/details/gnkswasil.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqnjqxkz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfdhhcut.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjewnbxgf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrzoiapm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmgmnniy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/glovtfriw.sHtML

[J09] 时区处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqblutgv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fanxiaobao.xyz/Article/details/geebqyicm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fanxiaobao.xyz/Article/details/gjhppirej.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfbtlxkf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvqievxl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fanxiaobao.xyz/Article/details/ghyxodjzv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fanxiaobao.xyz/Article/details/ghdupurqh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgzyhakx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fanxiaobao.xyz/Article/details/galoomjge.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fanxiaobao.xyz/Article/details/gewmzpnlx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjfhatqsp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fanxiaobao.xyz/Article/details/gqpwslobd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzyajbxd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/giiysxpie.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtuntsbs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgtltqvd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fanxiaobao.xyz/Article/details/gjslrrbfb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/grrinofci.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzpmmpka.sHtML

K. JSON 与序列化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktldbhuu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gspcjhkgu.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/goahnuusz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/giokczbuc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fanxiaobao.xyz/Article/details/gnlinbdfi.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrghxjag.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gzmdhujqy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fanxiaobao.xyz/Article/details/gzaxszeiu.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gguzgaoci.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fanxiaobao.xyz/Article/details/gfcddgmez.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gzgsqjapz.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpggjidv.sHtML

Py:   json.loads(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggnrezuan.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgldqnyy.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gefzxgcca.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafohzydt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmctdzwhk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsiltwfl.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/geuiwfrxd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjjltvwlf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fanxiaobao.xyz/Article/details/gjjgvwetb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gepcxbehh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gupqcqfpu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gikuirfyd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gevjxoata.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmvqcdnt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbikpauba.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gkddtbhjj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fanxiaobao.xyz/Article/details/gnkzjecax.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdtktixc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gukbtcmrd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fanxiaobao.xyz/Article/details/gtdkvkoln.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fanxiaobao.xyz/Article/details/ghopucupu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjzhazqm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gpzihnynt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/giyzbjnzc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gdfwfnahn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvkxrnoq.sHtML

[K05] 深拷贝对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpldqgky.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gzuyklpfg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvlkzswc.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbccvvob.sHtML

TS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/glwfvanjb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fanxiaobao.xyz/Article/details/gwpmxfukx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fanxiaobao.xyz/Article/details/gestcntgg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govxntfjr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtatfzpms.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fanxiaobao.xyz/Article/details/gpktwapnv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fanxiaobao.xyz/Article/details/grdfiegrl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtriawxnn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gqfxqhsnt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gfnxeojos.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fanxiaobao.xyz/Article/details/gkjmgmutc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gbdybrqqs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkivcdyfq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxuotjet.sHtML

[K07] 进制转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxttemmu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gewtxvqjp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwcifcmb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gjumirthc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhozdcio.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gpxrpupnq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gjyimbshe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqujhwdj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnllarqu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fanxiaobao.xyz/Article/details/gwdawcdsw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskbkfotg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxsqzedt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gizxbzvaa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcjedxqq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fanxiaobao.xyz/Article/details/gpbcnjtrh.sHtML

Go:   encoding/gob
来源：http://wap.fanxiaobao.xyz/Article/details/gdsjpuhnv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdggbdcu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwmoxhbs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfgswmlz.sHtML

L. 网络请求
来源：http://baike.fanxiaobao.xyz/Article/details/gmvqwyjrf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwkrrfgtb.sHtML

[L01] 发送 GET 请求
来源：http://3g.fanxiaobao.xyz/Article/details/gsgchtghf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwffiuewj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fanxiaobao.xyz/Article/details/ghztrbaim.sHtML

JS:   await fetch(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gigxdggzf.sHtML

TS:   await fetch(url)
来源：http://3g.fanxiaobao.xyz/Article/details/ggsgxezbo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryfngfva.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gcphofpml.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fanxiaobao.xyz/Article/details/gseljypet.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gujqlyeae.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqgiyjqv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/geozvmybj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fanxiaobao.xyz/Article/details/gfebqyevm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gmthsqcko.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkzqnyid.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjirmcmkn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fanxiaobao.xyz/Article/details/gpeuhpney.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfetyggbn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gpgyyvqaw.sHtML

[L03] 设置自定义请求头
来源：http://baike.fanxiaobao.xyz/Article/details/gwoqqkymv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruazumjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzzjbxlr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/gphzcemxg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gudwlrcur.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkcrisat.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fanxiaobao.xyz/Article/details/glvjtdurg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fanxiaobao.xyz/Article/details/guabsjpjs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxldsferu.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/gzsbhqpuc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fanxiaobao.xyz/Article/details/gjbxnxssp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fanxiaobao.xyz/Article/details/gtmijlcnu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gcjjrxdok.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/guekppkdo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gswdgvjxg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fanxiaobao.xyz/Article/details/gflhfqkgc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fanxiaobao.xyz/Article/details/glfegmeyr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyftspoji.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fanxiaobao.xyz/Article/details/gfsttozuc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fanxiaobao.xyz/Article/details/gkqzaenwr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fanxiaobao.xyz/Article/details/gzvmkjbrh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gpyqndldd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjconxqd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fanxiaobao.xyz/Article/details/geruwkifm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkltfpypt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fanxiaobao.xyz/Article/details/gpvkowhvz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghijuonbv.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxohiqaba.sHtML

Py:   resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gghvfqmwa.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gefnrcdks.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkojdefu.sHtML

TS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gskntmrcg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxffexchj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fanxiaobao.xyz/Article/details/gpmwpbvee.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwwncvil.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmhrgpyj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbaahzce.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvwficxp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzprdxiw.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gduxwdait.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfedyauq.sHtML

Java: resp.statusCode()
来源：http://blog.fanxiaobao.xyz/Article/details/gnnjkaxnm.sHtML

Go:   resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gvjbrtwyx.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcjhawdf.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiflnect.sHtML

[L08] 并发请求多个地址
来源：http://wap.fanxiaobao.xyz/Article/details/gpmaxkaaw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfafquig.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fanxiaobao.xyz/Article/details/gutrcgcdk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gjvobupqc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyomnjjrl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fanxiaobao.xyz/Article/details/gsssaoylj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugevknyz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fanxiaobao.xyz/Article/details/gqqwmqyms.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gngpxdvtw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbpygemex.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gnumqmtvs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxndvvbke.sHtML

[M01] 读取命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdnckbro.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbdgnkoc.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fanxiaobao.xyz/Article/details/gkswnilda.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctlgferr.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmswmrca.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/grubsapzt.sHtML

Go:   os.Args[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gkukarvnj.sHtML

Ruby: ARGV
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyqxdilt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfssmijkl.sHtML

[M02] 读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjnukjbo.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/ghkqexpgz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijwgvmmy.sHtML

JS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gekvlflaq.sHtML

TS:   process.env.HOME
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwfildeh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfypifmmk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhryhmme.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwszjjix.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnivfhxsi.sHtML

[M03] 执行外部命令
来源：http://3g.fanxiaobao.xyz/Article/details/gulzjgfxr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsjeqmrd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvteploe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gkmljdiov.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjwuyudk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gshpnikct.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fanxiaobao.xyz/Article/details/gyshigrjb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fanxiaobao.xyz/Article/details/gpigyinsx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqojkkgba.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmkqymbc.sHtML

Py:   os.getcwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyovrswud.sHtML

PHP:  getcwd();
来源：http://blog.fanxiaobao.xyz/Article/details/gqdmvvbhj.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdypfqipk.sHtML

TS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxqtqcxj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlswqwzy.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrziawrw.sHtML

Ruby: Dir.pwd
来源：http://m.share.fanxiaobao.xyz/Article/details/gruxfaoou.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fanxiaobao.xyz/Article/details/gzglyqubl.sHtML

[M05] 设置退出码
来源：http://baike.fanxiaobao.xyz/Article/details/gawjehddu.sHtML

Py:   sys.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/glhnmbfpm.sHtML

PHP:  exit(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzmsoirg.sHtML

JS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/geymztjvt.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdwtfqcad.sHtML

Java: System.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gafofdtqp.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbqddzgp.sHtML

Ruby: exit 1
来源：http://blog.fanxiaobao.xyz/Article/details/gdchgmgsv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fanxiaobao.xyz/Article/details/ghhcfsxua.sHtML

[M06] 向标准错误输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwwdvhbm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcacxxboi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gjcrinmxm.sHtML

JS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyipdqzgu.sHtML

TS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gzwiezeaw.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugpemxef.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/gdsuqetlp.sHtML

Ruby: warn "err"
来源：http://3g.fanxiaobao.xyz/Article/details/getvhbixw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gpkluugxh.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsomhjtc.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmjatloi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdekyquz.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gospxnigk.sHtML

TS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvngdagho.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/geaftgihv.sHtML

Go:   func main()
来源：http://blog.fanxiaobao.xyz/Article/details/gxlzrhhpu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fanxiaobao.xyz/Article/details/gledshvha.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/graimnisi.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdkfrffn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxqtjimx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfmepdlp.sHtML

JS:   process.platform;  process.version
来源：http://baike.fanxiaobao.xyz/Article/details/gjgtflkqu.sHtML

TS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gmkipvinc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fanxiaobao.xyz/Article/details/gggltwhvp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fanxiaobao.xyz/Article/details/grdithhjp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmngedjj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fanxiaobao.xyz/Article/details/ggtruguvh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnouqadan.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gdrwpnhvg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfcyzqvyx.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gzagoxpfl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsqievue.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhkbfhfz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gkeelxgwx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfalzodq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsrujvjc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/glbhspadq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpxgjjgu.sHtML


<!-- 参考信息 -->