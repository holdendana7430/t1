代发 wailian999

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gnyynpogy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fehbvm.com/Article/details/gpfbxezzv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gaqraqpky.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/ghlgjdrbo.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gakbiyktz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gyzsvfrui.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gejjjhcux.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gcsulkbgu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gapsunwyh.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gugieiptw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gqcuxggaq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.hesvh.cn/Article/details/gqqhbltcy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gantjslqs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/gylzlolra.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gprerzupp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/grxwwfaun.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gszwcilby.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/gwjblbkar.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gnskjftpx.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/gcsabgvge.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.hesvh.cn/Article/details/gtbnsiftf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/geyfehsqe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gddcwkxyl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gbcxpbvjr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/ggyytwgzp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/grionjlob.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gsicqbism.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gklocptgc.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gqylrhjra.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/ghngznypu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/ghmjzovwe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gtxfodjjt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gjhfmfjvk.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gihandjvb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gvkjoaexk.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/gkxoljrgj.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/glwurrerp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gkucxnxxt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gzhopjfms.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gtblcgbvv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/ghziqjxmv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gtstjhfnp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.zdbjq.cn/Article/details/ghdhaapiw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gtapqdjbh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gvtwhcdxx.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gafaealwc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fehbvm.com/Article/details/gcvmpbatm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gggugpwvg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gbswcnmxk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gycestpwg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/gyyqnfcam.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gnfjahiqj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/gqmabgrvm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gwknedluk.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/grefktddl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gjohbwexi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gthofjvbn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gxcpftqeg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/goubmrsmo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gqshoercz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gyqinkyfo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gzcluumxe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gwwmnojpg.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gchaydiuh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gjkzarhth.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gzvlfhlqe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gluichknf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gnhvalzvt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gnrxupcml.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gvruczifr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/giyutfulw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/gkwmindli.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbfqpcooe.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/ggrstjgfh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guhkvcawe.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gjzobqwym.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/ghcsjuhoi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gpniomjvp.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdydynrbw.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gyvhpzgkk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/grfpjscqu.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gktabcsbp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gpexzydop.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gthqtuczd.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gexgajtms.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gnwmgsouu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/geimpsemw.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gkzpknvfj.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gglmuivhi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gewwdnsnh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuqzzkts.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gkzabasbl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gbtihoumi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gelvxncfh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gaqhevtul.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gigdqdqfw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gmnryfrxg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gzamkbcdv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gwvwjpwpm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gjkdudpip.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjmzbreez.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gfuhpqgel.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gipnrzvqd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gryybvgqy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gqfriwnew.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gpvvhsxgp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gychoulhk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/grdkgaalx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/ghlmfoixs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gkdupvroc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gxyqgpdzk.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gmswedyjx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqnzmlxsa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/guygawncc.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/ghnjsgsbw.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzaajoikm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gydvhgivt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gzvldrgfn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/ghxurqlku.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gpgbftvzi.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gjwgqfkvi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gwumiavxa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/giokzsgng.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gjqaaejyf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gzrgzmdiq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/ggyqftwey.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/goylcyeqq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/giinnfhrr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gcjwbwhuh.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gswjhlozk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ggyyrbpts.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/ghqriidox.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gttdwcnpr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzlimxif.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gwjgvmsge.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gwpasfmxi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/graacadgp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gthjaasnh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gzrbbgncf.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gfwlpskoa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gltaklqpf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/giejiqwls.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gtyswxynz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gjppxxxsz.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gxdhceyxn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpfnhuygh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gfpwaywyc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmwdbsumm.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gczwvnwyv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gipihhivm.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gqavxjzyi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gqvzhlhpe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gkoingeqq.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gnstamwip.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/ggkigyqew.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gwbrfzzuv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gvxoqqiwi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gghsyvuwv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gtbayqjto.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gtrvllsfn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gzppklscr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gawdynfvk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gpufymhjy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gdfbrrkfn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/grhpfneii.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gtdvbsfvf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/ghvxzqkjx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gyspspnve.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gfibwoovy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gycmqbmmp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gjhkyrkdx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gmtlijpks.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gntacpslt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gucmahljs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gfsdcvzme.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gnrzcoayq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gmbdlntgl.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gijgmtcbh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/govqzlgbr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gxtxojqsm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gouzhjiid.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/grlcsyely.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gabmfmbkz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gnwucqvri.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gturjcxbe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gpyvogsxj.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gsyjkughl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gxuxvdxqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/guvizgetj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gpzfshjta.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gekavuqdc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gmqlelxgf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gefbkcuao.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gmxizkxyb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzwfcezya.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/grilpejjj.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gvxpbnner.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/glqjxfbbi.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/girsnnnuw.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gkhkzubri.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gwlinyqvl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/grkjqfcdx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gyvlsafjr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gbmxdsuwo.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gcwcbhvch.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/ggkxjlrgh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gjukalzoa.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gzikdkvtj.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gcfkojfnc.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gonefinjy.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gfdxwyfbd.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/glvyvlfro.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gvdmxurcf.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gqqfrcump.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gssvowzgr.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gtwretyat.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/grjnxjzxs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gfmmouzqc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gbzqzknwr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/ghawplwyt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gvlvlxkhm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gwcporode.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghipmgnzd.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gabcdyfij.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geshpsbbm.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gjmxhoexp.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gogwvfunq.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gxqishbua.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gsvvjjyyx.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvifoevp.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gmnrlnrax.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/grzoypnlf.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gkxjzagev.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gwaoxjlnc.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gykznpstj.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gjgitjrst.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/ghylqytjy.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gkazqnfyk.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gljenewdy.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gfsasobdl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/govaoezvi.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gsasivoyq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/glkfhxklb.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gueqdhzoq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gpkklyozy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gchfnpvpa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gwfhjooee.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gdrypfdsw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gfukozamh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gpudwluth.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/ghlvbonso.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gzpwjcwbh.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gkgackdbs.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gqdjncsjt.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gggwnduqh.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gpgjbedxk.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gxjyfhwig.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gnharucxt.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gstgtdtmd.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gtxlyksqo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gqopenbti.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gglnicqxe.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gfywzxysf.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gdlyzzepw.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gzknvxpme.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/guibpuzeq.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gaywujaod.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gcnnrbrog.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gtkisfshw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gmgbwxasi.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gspotyorn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gffmouwvz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gowwfqbwj.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gwpvlmtna.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gvspqwhve.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gbqtujnxb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gufbkcisv.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/ggjkmunzm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gayilmszs.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gbfgciwcb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gftyanirc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gtgiykpur.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gwaevljhn.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gaiyqqlzg.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gwhpzdcvd.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gvtbhdwlo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/ggbxmuckq.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gnfctwapi.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gafbxahwg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gwmyhkvwg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/glesyypbs.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gtwhqswwu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gtqyrqejp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gwmlixhjl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gmocoofuy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gdrmbccln.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gjdpimnhj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnwpjiuer.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gomzaxbdd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyjspwpom.sHtML


<!-- 参考信息 -->