代发 wailian999

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/gwqrynojt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gkmecplwt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gipmntpar.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gqeewsves.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gucyyevum.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gvtimyuos.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gpaclocsy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gqqiyctzu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gjsgwcaqc.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/gfxobjwea.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.hesvh.cn/Article/details/gufchfmqh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gzcoqjylp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/gockwqzaz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gdrzjybkd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gmupqhgyf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxaipbfsv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gjdosyqjj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/ghukpgitr.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.hesvh.cn/Article/details/gobygckor.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gdsxvpici.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/gvcegzvai.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/geagqygve.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gsnhysetx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gigfiyonf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gawapysxz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gapiiuvuk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gsrcmcvhe.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gmuuyxwuf.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gkgcamdyx.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/graixehpp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gvfizirnj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/ghphfcuqs.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/giccgvahp.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gjguotzqx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gzywdmals.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gqrgkrjja.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gngfyjftp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gjhmopnrl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gpgfrynqh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/goobygftq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gbgvvmuqx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gcocfggez.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/goefdzrgz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gawjxccvs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gurfempyl.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gkkpjndtz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gdibfyejf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.zdbjq.cn/Article/details/gvczwkfgv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gxjnwhymw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/gstwrdozm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gaxrrwiqx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fehbvm.com/Article/details/gvfllxcdr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gzygyopqn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gaikpozpr.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gmjlgcyig.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/gzhdywwwz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gkcezwhhg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gyavfmawg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkwuegxr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gdefiurgt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gbcqtmseg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/grkyxdaas.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/ggqokmlin.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/grjbvdbyz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gtmyvdgtb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/gzvsqmtvv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gxophdahm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gtxlkejjz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gixcrhque.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gpspcrrwi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/ghmynbjtz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/gspcccrfw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghlijdsxa.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/goglrhtuu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/garsfjvwh.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gtcieuhno.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gmankigct.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gvoitkcmr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvegucgyp.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gdidrwsnl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gfupyavwy.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/gpfbzuzcd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gceciella.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggaheoqvp.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gporjhaoe.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghdzysbnm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gxjzojyti.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gcvcasaew.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmlunlwdg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gvjpqufyt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gdhmtuvdg.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gktfuirbu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gqrwngxes.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gdmpgkxst.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/guhpzlovp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gkmssbsha.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gfqbpzdut.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gglnaooqk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gmmhvgyua.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/guayraboq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gsnsyihfw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gruyeyhyf.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gpuwaacjr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gykvrnkij.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gdlyolpdy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gzocqlnri.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gvyeukfsd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gdqdclwtl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gtndtktmg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gjwwfrbus.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gqcqwzibl.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gatserhnm.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gwealzgkj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gppkdldbc.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gbbafurfu.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/getxldqku.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/ghwkprwvs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gdmvdgzkr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gbhcaxmna.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gnzfrnrkt.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gnctpxxgw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gbsgvkivi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gootxzrtn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gtoyijntw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gtdkioxgt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gkkzgrqvp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gsejgpyta.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gpqsjpxfq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gypagokov.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/ggjudtjpx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gvmzghdjr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gtpwevmon.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gukrmngmg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gqpykiosz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/ggizjtsnb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/glpjwsdte.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gmojjtxmb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gahubmagu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gzcwuzvwl.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gdmerhofg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gsztnmpbu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gghdykjva.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/glwtnnolm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gbxpvzyws.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gdorbaqee.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gejpvqkmz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/grnoyswsl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geuzarqhk.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gkmtqmrrc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkknthtcq.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gjjudopjd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gtburlodd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gqsprvigv.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gendtoorp.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gldzngghi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gscqmagpp.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gwfebdoql.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gkjdbkgdo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gflnpvbzm.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/glirxkraz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gqazrvsyy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gzstakcil.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gqtmljuke.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gpyxcydfx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gjfmvxyiy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gecpjtpvg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gpvmizabv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gviejohpa.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gvtonapmg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gtzkevxjf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/ggmlogwud.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/ggeepbhha.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gvvlkaewx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gftzowuhy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/glvqqxjnq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gsimzkylr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gkfuecxrn.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gudfnwgdk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/glmkmwsci.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gvuvighkc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/grqjmilxc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gphhgydho.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gygkvsaxr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gqethbwoe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gmuaaakkq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/grutmkfoq.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gaiylefkw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gjmgyorfg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gapwatsgs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gyjpnepdh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gjcfywblw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gzacvcewo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gxoaxiyzl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gpuzpdxvl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gtvcmkqha.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gwzodpahs.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/ginjqpmnf.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gwwwnhwgr.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/grgwrejtn.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gazwfaraa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/guezudnnt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gdamgezqu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/ganksepea.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/ghnuuavtb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gyncfibru.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/guojesgkk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gevjogfuf.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gfzjqartw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/guvobjggz.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gfwwudnrv.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gyvsgkfzg.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gteqvgxyv.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gejvidnkv.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/guancqcyr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gtydgzrxp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/glozqdkjs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gvjluityk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gsqhnjefx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/glpkkxtox.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gbahweutt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gwgthwbdq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gybbimkcf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjajxgnqi.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gbeuebeof.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glhofihlb.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gxuyvykrx.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gxggekqhf.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/glnkxjbda.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gcdrmskaz.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gukbiyktu.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gzqxncagl.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gfujcmnvc.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gadcjywql.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gslkircdg.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gofqmqzhb.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/ggloqawmw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gvvgqoqrn.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gsxjsgndy.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/guoplybvr.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gjwwiprxg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gtqqqmcqk.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/ggczqwtau.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gfyolpvjr.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gnxabvkjv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gbzgsljqa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gomzjwysr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gfvpacynf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gkjbchhyt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gcwaytnpr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gwgvpwlqu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gsrsycgxu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gouugjwxb.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gqpvzdwfa.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/glefprxqe.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gwpotqvkb.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gcktpipzz.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gpoqmblon.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gtpkrufhi.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gtctcxmoe.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gavochrjg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gsuaozobp.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gfcktzhga.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ggiudmcfm.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gzwofgieq.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gjvtiytgn.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuqxwfnz.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gmyklduvx.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gvjkxiuff.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gsrxdwsxi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gafrswafi.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gogdukuxp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gozagffbi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gnouklazr.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gkltnvvjb.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gfxdcmcgb.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gsviktqok.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/glkmilizf.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gvulkanga.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gpeyhbyfr.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gzjiupdoi.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gglulhkhv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gwopdebar.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gmqkramek.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gmkmzrvoe.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gjcocvccf.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gzyernlsn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gjxbtlwwc.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gycwyzwuf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/ggfbjzoav.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gydekjirv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gubsjyzdj.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gzxewmhdy.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gcrzqkfme.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gttcwemoo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gnmouhgma.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/grxuuqxzr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/ghhovonxy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsnszcexa.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gcwssqhrt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfcjxrkan.sHtML


<!-- 参考信息 -->