代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gbbtlcwzw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/gsosvrocq.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/gtapedlpy.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gwnmxeppu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gzmrrugqk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gucizivid.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gswemjxoc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gwgxiehow.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.hesvh.cn/Article/details/gccoqxvdk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gdfdajzus.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/glsaxobyp.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gsmjczcfq.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.hesvh.cn/Article/details/gymvczphz.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gdndvfqsm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gathzmgsd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gzrvbkgjn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/gulwdgwzl.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gxgaaqxbz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gsizpspyz.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gejutzqcw.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/gjilsnjjh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/goymgrxbz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gzznczwaz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gnfndeojf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gpiolvvpe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gfmdgtfya.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gezkuzccg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gnhetjogz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gianxldor.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/gqkeiwklr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gtjhtwufq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gitrnjcwn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gibwkrrpv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/guodabjba.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gkdhimbbc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/geiblifvg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gyoaohnvd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/guengneye.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/glakxeqnp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gnekwsjhb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gokqhtvnu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gsjdxicrl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/grzrazxtd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gvvdjgpsy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gsmlirilu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gwpqkjxxf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/ghmasvmbq.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gghlxcbso.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gixovekki.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gffangyug.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/giyxdloui.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gkwvxyhrn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/giglcnrjd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gdxxjlodx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gepcbvyol.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gscidvdsk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcbichpex.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gagnicxuj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grryblnmx.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/geyivkhhr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gykkycqxy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gleovmuba.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gqttwhnew.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gqcscprxw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/glinnnxbk.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gdzjyduig.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/ghodnzcrg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/gopgxhkew.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gbcufhylt.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gmdspesde.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gpqsprnnu.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gufrkgazk.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gwqafrjou.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gluhijxkb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gxmxdivcg.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gtrsearhf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/ggaxsdoxz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/grctgksmi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gnssxwgij.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gdsczlzar.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gacevdlxh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkhkigzeg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gtsbpmuin.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gqvafrhsk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gewmeuqvx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/ghltloouo.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gyisgbnpj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gmwomcazo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gudhqwbwl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gpynhouvu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gxuryjblp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gsjwxghlh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gipajrvka.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gttnweyif.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gsencoyqq.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gyrgmquox.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/getcvapor.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gmmliqugf.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gbatoffxh.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gtrrtznay.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gqfagxfla.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/geblsjcbs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/goipolqql.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gtwimpqwg.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gkzooidqo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gzinaapig.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gbrpjqnzk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gdmecvkcu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/giyrijpln.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gsosvyzvi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/grllheezz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gohmvmdvv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/giwbluzjh.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gxniizodk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gkzemwqah.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gebxiftag.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gmtuaeglm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ggknvzitq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gnxmccjsn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gwzbnlvym.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gjgtxggcn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/greubukiu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gzbfkzxoq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmxwnpqum.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gnrcxxxar.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/ginqucdxo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gbebcmxdc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gsnrsyxsq.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gdsrqdnzu.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gzpquxmos.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/glxplohzu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjqldstwc.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gudbwdugm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqumeiipz.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gchnptcvn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gujgmossi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gwtldmztb.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gvxwkolqv.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gawxzpyds.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gbqpfbgic.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdtuicue.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gndqmmhei.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gghdndguk.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gbdolahaj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gwqkcqnip.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gxzkuvvtb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gbiprynui.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gqwvndhhi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gsdjxldsf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gggqrulqb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gjmhzymnn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gjdwdjnma.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gjxgmgxhw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/grrcorldt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gkkahnkat.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gwfhfvmlb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gtpynixnx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gpxgjumvh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gooufwoia.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gvxjytlwi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gcskgujre.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gpyaphceu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gibhgcvvh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gppmpbbaw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gfhoigfcs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gommxvcpp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gfwxfctjs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gbmhflrxq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gwcfybunv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gwyfasiut.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gcybiwkxv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gsfuradqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gerukmqjr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gsercrbse.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gfgcgnzsx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/ghykxdihw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/goaxhmcio.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gzrnekkek.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gmtiuvwuw.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gytkasknx.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gzkejylkc.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gligbyhqk.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gymeqdvmu.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gcuxkvwre.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gtbymjlxf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/ggmwbjlmx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gbboqsacz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gdnjnyvbc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gbabtsuql.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gidnxybwb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gpzehufmx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gtbsyawtz.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gxbjazmtw.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gsjnrjqui.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gjuljodrr.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gcdnnuwuc.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gqbfqdprc.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/guolaxafy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gpjigzjie.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gqctbxkaw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/ghylekdvb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gpnyavjxd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gzbfjdbth.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gatlcusfv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/ggelutknv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gctdlyrsf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggyaqhujj.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/ghecoosma.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gktcnqimj.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gaoitpqsa.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gjvotiocx.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gocvuiqmp.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gdmdogmdd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gtyedytmt.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gknufycqt.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gdmjvwtuj.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gmytachay.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gknrjrslr.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gyfecoekj.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/ggmefksjy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gaqbihjka.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gefiknuss.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gntbhcxsf.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gitekxcld.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/ggwngmlkt.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gguvgpdhq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/glijhjccl.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gvahvqbdz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gaqijaxjc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gejjlstqo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gtkakgfui.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gheqehgnf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gezcxurnh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/greyokpvf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gtkmkhvad.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gozvkgeww.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gdmquqqpc.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gieiwmqiq.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gxammycgv.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gqzjmkyok.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gapkutfkg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/guuqnlhnw.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/ghzqsvsdt.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gzxiijcmi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gtfnbarhd.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/glwbsftvp.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gryyuyuko.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gdnnkdzhl.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ghazsjhwl.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gbfcltjcc.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggqftcmcg.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gvnvnbkfd.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/guxlhghpw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gsiaawyoh.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gdzhjmqlm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gjikekokb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gqqktkxpm.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gkjrigabi.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gadjqplso.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gnbyvqham.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gssfdqgbh.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gxztydkxd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gtcoqbqyf.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gouynwmqe.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gponmcibp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gldmvigjb.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gjlluxpgd.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gesynmzcj.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gjpacnayk.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gwrimdoyj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gxqhkxwex.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gqcgpyhwa.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/geoponglt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/ggdxjikyr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gvdeimmzy.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/glusyyqvh.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gylprulrf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gsiuogyfe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gwjcqqkpp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gutnleugm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gvzadyvnp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghfvrjmqm.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gruumkzff.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqguvjycu.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gqthiqdsi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gcbzxksod.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gkwgrcwqk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gynmcfecn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gpqajvmfz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/ghxqpihgv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gnedzzose.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/grkasbyuj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gdgubdyir.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gsqvqawwt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gpnafzxkf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gzvpsxqvl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ghpqhjccb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gihtcgxfy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gpmcixorw.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gofrwwvzx.sHtML


<!-- 参考信息 -->