代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3okimhqoa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3tlmgwott.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3sfuxgnkw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3wtgqacft.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3udtcklqa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3mptzdndh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3nzgtjzge.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3etjafgtv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3orbhgrbl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mzrmeeuf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gmqphvzj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nykzyclx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3tylslfbx.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3fgtjeoay.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3gsarzkoy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3rudseffz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ptruoveq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3xwdthiat.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3aeibdysv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3whyjpwjj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rbasselj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3wyuwbzet.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3iwuwbhbj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3atvmwlmo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3tjmiyemv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3qpboaqsn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3phtwpiyk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3gxtyveyf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3sgbidukt.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3kzmceory.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3klnzlnrz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3dgweuzjt.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3dynmsiov.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ymfugyjj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3gosqtdco.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3klasiaac.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ulwnrccv.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3aowqvtcs.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3kcidntcf.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3swynalwg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3xigdjoid.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gwhhnurp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ablirbpz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3laccexzy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3svlxslzh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3zdgotofv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3kgrgxgka.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mypdznic.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dqgcfykp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3cpnhhonj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ehbwjpdr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3zctcmylb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3gmjluqdl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3wmawkowc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3sezgmfes.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3kntoypbf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3hnycjqmj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3lppnwuze.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3jafcxgnu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3glxufknv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3juwvqzrv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wxthlzbr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3zlpflqld.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3kecahsqs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3houotnhn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3jjiofoor.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3krcwyrme.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3dbtnwluu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3zdjnwqyu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3aeywtphu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3blkmaxqr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gbgopebt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3vpswihed.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3lvxhqniw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3jhastfpd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3rjgxmwse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klisdznf.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3lvpinemt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpmqcmda.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3goxcbtjk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fwtjjfyx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3udnfcykv.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gutazgts.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vchduefp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ocvkagcd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3cnpxeysv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3yiszculo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3umwrchuj.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3emzxsbyg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3qsvnaaai.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3hqehyskc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gznxkcql.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3favoljal.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rulingoi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3goixtzfe.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ldfkdppr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3rneubhxp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3uxcdpqbq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3lorcjlya.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ntxpqgsr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tchhfqkj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vwfhhluy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hdlxwbxy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3sswfmnkp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ihcghxag.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3hmdtehhb.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3wqigibtp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3xetanpyo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3nxoufcsh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ismdvjfk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ehgonfey.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rkpmuduy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gremdrbm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qpgjwwao.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qwsthhqf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3iazyvcwc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tlprakkd.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3taynwqrd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vlgijjld.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ewzogqvt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3bxafehdt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3vbmyeosd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3qwtnryey.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3wrxhtcur.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3htpbellx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3gphgdbqg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3htxazslb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xxdqjhgp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3upgzlmpn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wqlwsocp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hdtykdob.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kloafqkn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qnbmhket.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3dsrnogpw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3owxklrrc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3cwdmypjk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xbiwmujz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jxaveyqt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bouuhnbv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mhfosabr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ulrkptsf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cnjmdeca.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3jixztwtv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3lbkmaftu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jigoytgu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fxpddrpi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wveceqea.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3gfpbvixd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3zxtswsli.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3axgrhbqa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hmybrvmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxdskzil.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ngjhgdqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdpraute.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ktmewfdy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3guaggwrn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3vasacwqa.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bjmreqsq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wejzzzns.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vspenagy.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pekyrlem.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3bkfjokqy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3kcdkbzdk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dimgiani.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kijgdpff.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3envdirdh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ogtmpemy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pupeumgm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3edqcwjdx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3elpvrqtz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3udhxodac.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3rflylmme.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3idxcqvfl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ytyyifbx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qksnsjoe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rvhwxilz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fmmtopok.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3fypiminv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3knsjxuea.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3iumttgft.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tqzymipy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3capsvuje.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3puznkfdj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3askggoeo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3choxztsm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xvkkutzy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vyzhxmem.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3eaxfmlfh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3csjclttp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3lpezvgfu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3eynvpyll.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3yicpmbxe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3nprclkff.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pdlhnvld.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lhxpzocf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3gfhgagdx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tmgqlrcb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3yklykdrw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qdyqjsgs.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rewwclsf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jlegefaf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3wqyspwnx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tkhweogt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qwhftmko.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wakpgybu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3havechoc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3cxnmrrcz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wfrvztur.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xmflaogm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kegqasjr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3nstvleah.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fswjwcyo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xxrvrxwf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3chbbkpkr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3yjjezmkj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3mqyubqss.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3femejsjk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3egblxiqa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rdyobowk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ozopwifq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nxwaltfn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yxetjusy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3cyljdbpd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3biaibrcs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wgkythzu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ykkuoawx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fifscnih.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3borisnhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lokutnva.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uwscowtm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ncxurcjf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bbfybamt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmszzifb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3thlzbtkl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3paarkmft.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3otioqilt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nsdjbpud.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3thjdvofl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3utsttqhb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ixxrufuk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xeoitxhg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zrolmgnu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qgztpegz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hfotjgpm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pznxkcye.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3oxvmzrkw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qtbytdzd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nlmgfkpf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3abytszlf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jqtyqcyb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rdkmvfsp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mwhymwok.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tvlkpdeb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3coirhxxj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3egqdsfaw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kpwdfxht.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3dssbzekp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3avmlnxyn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ggbkropn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3aehjpdca.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xngaxvdp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bfbpwlgx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tyuxaire.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vyxktnly.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ahlrhyzt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ttigqtld.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhxqsgnc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xvzllucl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugtiofnm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3laapxllv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xrmfdarj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmthqcm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nfmsdzqc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tnwlpfbo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3duzczcam.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3joiwwvaq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ssnbrshh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3khiknwdp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ufottfbo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3omqzauac.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vtxurxzh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mqmlyprq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zxaxdndu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3chcmfyxa.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gqfxxnjb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3iefyprno.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xhhtlcof.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jdkblyki.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3hvbylccs.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vapulzks.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rylesosf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jvdffoep.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nuohxhgs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3poxiyfnt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dccgholz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3glnrpciv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mmhhmdvn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3sfobfrgj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3uwllojlu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vtebtxgj.html


<!-- 参考信息 -->