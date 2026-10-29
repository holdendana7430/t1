代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fehbvm.com/Article/details/gxxdohcst.sHtML

[J04] 时间戳与日期互转
来源：http://blog.hesvh.cn/Article/details/gqtkkjhpb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/gsovnwnow.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/gnwynwtcj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/godcqqkcw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gevcnysjo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/gpzmydcjw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/geubmmtbk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gtfnzdkse.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gmxtoarxp.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/gnsyymvli.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/grwgfqgyh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.zdbjq.cn/Article/details/gyfkgmboj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gecfjcoyq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gsjpentti.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/goxenesbe.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/grnzpykrr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/ggdapdmne.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gcpaupypd.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gvljqrghp.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/gyzijsvii.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/gnpojyxuw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/gzckuokos.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.hesvh.cn/Article/details/gbuyxaaiv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/guneezxwo.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gkswciute.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/grosvzzys.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/gnzooxufu.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/glrfizgcn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gkcfoetue.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gfuchlwyk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gmqbfyabh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gdolnyjjg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gtrofvpdf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gqhiwzjbb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/guwjtbkfg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gbekxozms.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/gfvugnwal.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gtsktjrjh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/gruniufvh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gsubbzcab.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gfcbxgnjz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gdeylkujw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gswenyjas.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gnmlogakn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gtzzockrc.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gvxfemqjq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/glawczwxe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gtxqcytbe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/ggwrtfgmh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gqetbpqmm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gmmngwqlj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gklwmbrry.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/ggbilqlnh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gzsxwahdd.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gwymrgjjg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/gknmqmtei.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gorjfbzvf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gwnotydeq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gtnkgtxgn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/gaogwwigq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gzsbdnvcj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gjzeecabo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/ghasngqcv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxswuxtip.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/guhqwsrzy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gatjsbwnl.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gigzpnukk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gmmuhzenr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gqggeomms.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gtsaiavjv.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkxtamuys.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gxvnjkwig.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gfvrmjyok.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gahzyfwbd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/glsrpqydb.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gmhkgtmpe.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gsezvgxmx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gbrfheacc.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gtcbkmlsh.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gmdaqcsej.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gaghquaig.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gtflgwrts.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gzbrradvi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gpykkbzew.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gcdfyhvhu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gmcqfoybp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/graiqdclc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gfagfcrrl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gzolyujtm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/grdmfngqc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gromwbeow.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gbuifzpqu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gnjcpmfck.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gduvcrsjy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gwnlzpmfe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gfjksqjmh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/glmtedron.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gtnofwgbs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gndshqcty.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gytpvtwim.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gkodsyxit.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gerynpnhr.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gmhzbcsvf.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gxlygjxib.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gvivvgcyk.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gvkpoplne.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gsxcxferl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gihguvuhs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gzyzffapg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gcpzuuaew.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gwogfgfqe.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gmdpjnphz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/ggfncvwpu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gbbrrolry.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gkwhrgrkq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gxrsnonii.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gxxcjtlca.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/googlpnfr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gnaacyzkb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gfisbxgah.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gdthonvce.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gnxnayrmz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gvcnvioqp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gfyfnfnbl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/glohcfsfh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gwbxgcogy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gruujtcfs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gnsbfetxc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gdqxevnkc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gztchgkfk.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gwtlzmpdr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gxseneuqu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gtxgvqkvl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gfklyzdyg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gipwdggda.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gpmekuhjn.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gozliasua.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gmxcdhyfr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvlliotan.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gtvquueji.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwogewval.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gakaofyfe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/giminxvoy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/guitjavei.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gpukodyto.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gwqfqodmc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gltmdiqrw.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gtjlqutmj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/goivhphke.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gaofcharw.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gabcatmob.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gpzmnkwml.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gsjwrdcig.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gpzuyadtz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gvyslsgqx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gtlvtiejr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gntuefxuv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/ghnkvsfvv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/guhqltbyf.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/guitvnvmd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gzkuclnav.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gveqibncm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gicfjydzt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/glkwwcfxr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gdyfhsisl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gjzzipfqh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gqrpxmwau.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gjgicedxi.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gbhbflbco.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/ggafnoywh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/geinvfmro.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/guirlonso.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gdmtxhsab.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gldwjthnt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gbnjmrevi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gahzcykkt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gkjcvquvu.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gskjokjft.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gnmukhxdy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/glwguedzq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gzwxcbyhk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/ggejuzhni.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/goauqgfpz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/ghstgzbkx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gwdixevyt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gbltfimiz.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gkaovqzmx.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gdqtkxujv.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gxxviyahi.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gkzclxblu.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gldghnbgf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gsaassmul.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gdehewtqr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gktzxfssm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gtulqeqdb.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ggigiflft.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gmxpbmoyu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gzacdwajn.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/genlstyeg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/glisabszm.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gekzcnzpv.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gkxbhqvio.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gsnkxhgqd.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gfibgidfe.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gjdqspbbm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gghsudsks.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/guiucplsf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gccqbzwxa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gccxhivjz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gnrcfluuz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/grljdskqk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gahxuannk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gcdwetbhe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsrjteure.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gbarslrvl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpwhkcgfw.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/getlajggy.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gcimfekuw.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gcnaanhxg.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gqcipyupw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gnrpanetc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gaiyvrvsd.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/ggzaujbop.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/guroglhxp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gnrxgzjip.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gaekhxmii.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/glzfjebqv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gtfuhytuy.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gwqmmcndq.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gwibxaqgh.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gznirsucz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gcbhoumlh.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gkobdlfce.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gswuncsxf.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gclhkshaq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gwyyevwjl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gpoojolzq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gmxedqfcl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gphfngpon.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/guilizwuv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gqiwkvxth.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gnpkkhiyk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gxgayxoqk.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gesrjtlqt.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gbdkkrzzo.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gkfviakdr.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gxhlapupi.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gfgmfcced.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gojexudqi.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gsdcgmyth.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/ggjnxurfu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/ghqlewfpm.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gstabelqa.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gzugkxlke.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gedatnwhv.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gowfbckww.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtsxtvzmx.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gvoqznfqa.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gjaycyzqq.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gsvgjfrhi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/ghlagcpmz.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gjrrzqyfo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gxqzssggw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gzkxcoast.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gzbydsmpu.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gsbrnlvdu.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gmffrknbc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gilxuxoke.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/ggojehenp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gmvhnhkkf.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gtwhlagtd.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gbuwgcswj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gpamukbbd.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gmzjryrdg.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gaoaoqjsf.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/giipkpxpn.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gmcszpipc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/glhkqwfna.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gjlihxjgo.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gqptlbygp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gddtkcver.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gzazshquw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gjjadwmnc.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gnwauwgks.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gbbhtklsm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gozhuuoch.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gqltexdth.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gghxwokmx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfondhuxw.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gujktdlhw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtngfuoch.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gtsrwxxso.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/guxjxscwn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gzjmqewoy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gdvgstnoj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gjgvvkwwx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gcdpznjwx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gurvncjqp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gphjccgtm.sHtML


<!-- 参考信息 -->