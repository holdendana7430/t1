代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2xdmccdxj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2epjodect.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ebbwgnjy.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oycjwrfg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ssnbvmqn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ujcizobt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nqjgwniy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eeoikcwh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2blsirvxk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2rcxywhoq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2pvbpugel.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2aryhxbce.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rghfbtjm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gvknwfci.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2yekrezkt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2msmnkjxm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2sljljyuq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2jrrzjdlq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2uzdzegwd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2lkostzgs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2bchzdomw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2airlinyc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qmxipdyf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hylmlxdz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2riebxvin.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2chrsehns.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2xrnggofg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ineejbhm.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lohrwwyf.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2amkghozn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2afcgsxiu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2mdofprlj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jythnauk.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2sgtrgmlp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2yljrmlnl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wjvhvkab.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2bhfljoao.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vuhdxesg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2trsidxfa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2aetxgmvm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2wsbexqnv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2zioukjtv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ffhkitcm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ijfrndze.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nafsqwiu.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2werglapx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2zzfevnnt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2czhmixch.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2gzusdolc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2xuwwtbid.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2cgiyfyld.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2rwhavilg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2tlvtqyjg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2hyevduhn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2gphqlxcm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ljkqdtdv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2kiofiqyn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qbeuunio.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2yrkzcbmt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rfuhwqch.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2lufidvrr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2wicvliwn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2hjzoznzy.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zjtolirj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2oniybveg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2sicxkdek.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2gutosyag.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qisyxzjh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhphaxft.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2ycynzjqe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2uyrlohzw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2spsksooo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqttjbbn.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2zrvrsevs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blbohxto.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ihhvresb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2pvyysuob.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2jpkdqyes.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zubvjcbn.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2gctqabci.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2menvpljv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2cshulrcn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2fcnmbujf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2cipcqurb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2vyrwrokw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2gteuekjs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2kcvehpki.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cbcajamg.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fugebdsk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bqgkfrsn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ccakxlsg.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2scfsrlcz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2flikkudl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2icrvdzqs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2chddkqya.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vsuvuwjl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mhvbgxie.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mbezybpz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2hjgiaqri.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2phqtxckv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2raphzhcw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2sasskxjo.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2fzwumphs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rzndkktw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ktsxagww.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2feeytjso.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2phsdvewz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2janoplck.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ygjgtjun.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2obyuwknj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jnndeqdz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2xlwzuprk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2chglgcdm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2lfphoxgc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aokdyocs.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2npgdejwg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2brtxvliw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2oaifacti.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2hszkutwr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kaaabuco.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2slxrqxpx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qurexxwc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hnnbanqh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mmbsyhei.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cyfxlfvj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2nolrkygs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tcyucjgc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2oemtgrlt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2voyruvoh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2aqdsnuah.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qrfykext.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2gnniedfr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfqiabd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2owwpdzyj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qrzdpqnm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2tpycrjnq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cpklbdbm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xlrmwyja.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2qxiejggs.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2cnzizcgr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mychigcf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2yodpknhq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jtieuscg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2mbalugih.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2peczanbd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lecyguxl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mfsgtqji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jnbsdvck.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wjsxjput.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdetzafy.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2awhunhat.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2zzjkzkhf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2sqysfhuo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wotbekwx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2krexipek.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ryyoyavb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2mnzlsybi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2uzzdmdhc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zlgapnnb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ihqlmrcf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ldbnxdhr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lwdzkset.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rtybdcao.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cptpgzhl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2axmetant.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ocwlkhpg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ekvqvysj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tebpipbs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vsapmise.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2utczjtiq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2uhiktdvy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gaarxboh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2bwwxcohe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2tmwfwekz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2odyoexsu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zggkedxh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ppqkkfsp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xchankbe.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2tkprseem.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ualmthry.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2yrmhkqbv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2znwpqhil.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2turtjfay.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2eeghdzur.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2aqdowzfw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yyoyywqi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2zkxlsrli.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bkxricnr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jofmrkgb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fhezuyfv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2usfromsy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2lwyfiqna.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vjliynci.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jjevozof.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lundpmbp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2gzhxrgjm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rxsevmgy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hhkpexwu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xweucqag.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ywvhsrtv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2loadhlyv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rhufptbo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2eoxalald.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2chjwoxfg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2oqnjsfsg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2btxluumc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qcwdhnei.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yceprayo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cfgnseco.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2hovagvva.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2prwnpujj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bidjmwzi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2stucsnxn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2eetrlddv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mxxlkohj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2gdnivdjs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hplfcqyd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2udblvjxn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ygbtjgjg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2vxitgaql.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vvegohfk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2iiilgevy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fenwbplc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2fvvfpcxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akyjssan.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nvytxwts.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pmjhyvsa.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ofujmbag.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2itfegspx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lncurrjh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2chkcangs.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vyfglrho.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2odjyfrbm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wpgzpkpv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sddaxiiz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zshpicyc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hlyelftt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wngowbmk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2udjbcjsy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ewiizsfm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kmnmdguf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gkqmwrid.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2axmeqlrf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ynvkhhsl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lzaexpvr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2brobsonc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zdvnzriv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rofrvver.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2huqyfmfh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2koxsxqwd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2tohjsgxr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nmobrejm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vqajiotf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2rlqcetqv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rstfbkbm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zwnhivhe.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ztcdxexn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2twpzsehc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tpusjwre.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dkkfugxq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jlievadb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bfwmsvrv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qewkukyh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kowulhfk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iojrbcoo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ylicoyjr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swxxsylw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hcebwnlf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2grjlqazx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fayirkgz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2moocuqoi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2erjbsxbk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2oykojriv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rbvoizzg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rfnzaauv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xpocnpnq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gzvcgafj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2odxjjtke.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cukqdiye.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2zczyorls.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wdkjhzgd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mymqpala.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2llgunfqh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2njfsfgnk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jawgowks.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pjxvftmz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2guxtphup.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sthokwzf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mondgyfe.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2opeoxtzi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zbzlgkus.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2alarmmsh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pejpofxa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ydgcdwlk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fxirapeo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cijxqlok.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ajtwwhal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfmxqpzd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2sqnpwcgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmvszklh.html


<!-- 参考信息 -->