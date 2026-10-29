代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gghfubdbi.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/ggpnclyjq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/guxngfcux.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gydncdaxo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/glawvdfbg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gtujhzopm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gntfhgtnx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gudchhvoc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gqxlthqpt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.hesvh.cn/Article/details/gdqjiqsqd.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gmnlovadd.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gmmmpqpzl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gzaatulgx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gzqkdmwgb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/guixmrddp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/glmqbydfq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.hesvh.cn/Article/details/gpeclhphw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gsmthinzw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/gieodtcak.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gqbztzdac.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.hesvh.cn/Article/details/gvozjdhsx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/gmvrhaeyx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gdvzhswav.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/giwyutohc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gejdobjoq.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gysmznikl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/gsvvloyaf.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gyjlfocri.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gpvamajzl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gtumnshco.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/gzsldajqq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gyligpbrt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gcvpwpkpp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gswrknael.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gyupyyhhw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gvbngffua.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gjyyadory.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gdjfvqguj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gfvvtlbkt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gwczebgbm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gpzzzwghc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/ginnjlwqx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gdlbqyqnf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/gywzndcpa.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gpgvoqguh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/ghheikhmj.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gbvfckhcr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gbhpugemh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/gckfcjith.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gulntnqru.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gdvkevrnp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gflpkrfpw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.zdbjq.cn/Article/details/gffebkzrv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/greluvirc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gjztqaorh.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gbbqignsh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gflheyjqa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gbnvruisr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.hesvh.cn/Article/details/gcxximaum.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gyyovpgbf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gyuixhkoz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gqubkbqdx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gppsmonyw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/ghfjgedxb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gklrdqxji.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gootspcvx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goxhgkqfu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbwozhutl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gcspmvcta.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gzvqmvlyx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gxmvgwsju.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gjedzxavl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gtxaowymz.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbvcshptm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gvgnixwss.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gwcxhdnzj.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gywcylwej.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gztrejpbo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/getsvrkpv.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gynydsuwo.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/grehuvwbo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gyfzeqhdp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gevegtpdr.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gfjskjeht.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gtayndnyk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gwnhysgoa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/ghgivcrqw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gwtguueiw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gcbtpyfho.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gworqzuoq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gcbtgoqqv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gewrpgync.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/glxhjpehy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gbpyhnxzh.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gqavtrdwh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gxlquulqb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gextzxmcf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gusftcbzv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gmkefwobr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gylmrxyap.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gbvysvilc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gzeymlwkl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gqoxkwadl.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gewsqjhay.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gjmrprxzy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/ghtcpgvnr.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/grdyesgyd.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwbirwinf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/giwilcvvp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gdbbycdzt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gijqxhtwb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/grellghbq.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gtgydpchk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/giyuzmkkj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gjkssytpq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gzceaeklp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/geikjnvou.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gkqbwievy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gaysokfjz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gfzrukhpu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gtfomydfn.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/ggacgsvqz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gslyhjwhj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gaxsxxgdb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ghuznfwed.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/glrtegrpq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gqaujcuqx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/ghkjufzry.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/glgbdsyjh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gcqfscbxm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gabgnsuab.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gjazfjqoo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/geyvmxrlo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/geywjlmgf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/giqiaeldc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gejciuvrf.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gpdteoity.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gtrqdiali.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gfsgtkujd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmskqkcca.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gubbxqjpe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghmnztrps.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/guheqmmsk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gvcqhtxut.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gntwwyhho.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/ghkjcrpuo.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gntbgiglc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gsswzgorf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gcwvyskge.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gdveiyqlu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gnaggaxwi.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gdhzhciuh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/grqywziqy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/giucztfef.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gxlxgqtoz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/ghdouubql.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gdckgijze.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/guyryexsk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gpoofgcyb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gubhapbow.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gtwjdnmku.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gphsmbwnq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gsvgfazck.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gpqqbgnzq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gjraaosha.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/glpnahmqq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gkfobqddi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gkruokzmk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gjybtvfxa.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gaykeuwta.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gahnmfenj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gbmzhjogj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gvyzfbfzv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gldhztzdx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gdngglclj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gjvlkavif.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/ghexlhbhz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gkzsepumw.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gsxvqkspi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gvrsdenwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/glyyobgmx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gcznmmxkx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gdvdyjxbo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gskdkdcoh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gfobfppub.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gqhuienms.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gbcbbcysq.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gjtydvwzg.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/guqsdeorc.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gyscqvpys.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ghwzralzo.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gcqobonly.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gsadwkiuv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/ghbyybrdf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gyqvtraqe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gvabyhdoc.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gsdhxbsds.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gpzehezlx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gvxgzzoxp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gmenfkzsb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gdwnsrkac.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gyacwhasj.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gguqcsviu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gbuuglggv.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gnnhaqugc.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gcenavrjt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/ghrcnvtbx.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gwpzpvves.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/godvndiqh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gcfeqkofu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/goyzqvfau.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gceaecynq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gsqzsnbno.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/geahzufdl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmlucarsv.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gbdsqrftl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/govpkyawe.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gpxannzoj.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gllmuatuf.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gdmlshyvx.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gvisbbpki.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gydqtmdbx.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gdeppowlh.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/grfdljfzb.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gqzidsnto.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gsbofxwgm.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/giznrhqaq.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gtdxbbhwf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gofxpzylo.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gmrgdlvci.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gmkgrjecu.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gtaojuiqe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gpnnnztnx.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gbtxqhuyf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gbqwfunye.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gofiblmuj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gepgkmqon.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gxjwocidk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gxzmruxup.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnhnzykoh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gwurxswoj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gjplsijgb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gfxtbsbaw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gpyuimfsh.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/girniczqk.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gzkrolmeb.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gumghtfdd.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/grvovoidb.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gypslnwsb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/ggjkaricz.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/ggudojlxi.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gxzrvxuji.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/grgsisszs.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gmjlvuqgd.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gxeldcodi.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gqwhdwhxo.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjhcazkbg.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxsjhbtbl.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghrybuccc.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gweyzzndc.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gttphiars.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gckumdhli.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gmtzsbpbb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gziqegpdi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gvvkdvvdh.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gqqccossl.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/glqsvwvux.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gebzpcttd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gcczsorcd.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gssqmpvol.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gacjmwkoi.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gygtuaiii.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gdyztgurj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gxrwacllk.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gpveadmuh.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gzeyatnty.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gswlqounk.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gxrcjnjlo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/govttxbkx.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gqfagxipc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gkitcszef.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gddngihzq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gbttkqgrp.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gdybzkrij.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gkydxajhd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gicaqyssy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gjxpjnpkp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/ggwfpwimk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gozdfrmut.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glnlbifip.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gevprzmdh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gypglgfvj.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gpofwpuss.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/ghmedowlp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gwtwgqoff.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxbgehfj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gpfxfspwq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/guvznindm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpiktadfy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/grcsyfpyl.sHtML


<!-- 参考信息 -->