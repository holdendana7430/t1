代发 wailian999

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3jlqrfcby.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3cgholwdw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ieaqtsnt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jjubjemy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3dafvntma.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nqcpmzwg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3dxsiwdop.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3aizjuwtk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3btcyvelc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3rtuuuvcy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ysvxsrpq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3homyrang.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3lozcbueu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3uxuujloa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3paqbgohj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nnfqdfaj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fkqubpgb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lznopazh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nkfwcqht.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tklumclb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3yujurrtc.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3oeziougc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3qpprnajt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3dwcwgvxt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nuzdjqwo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3yjyirkmw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3fxleqrkc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3onwsqwpm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iennqhfp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3elhvftwe.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3exsopjxv.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ffyjlvyp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3cqgxhsrr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3nbcqldjh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rpugkkwy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xnzsyouj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3plzwuokl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3tlstlslo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fsvsnpol.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3jbxujqlg.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3lahqkaan.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3wmluoxdh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3nwywmqfh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3aogekiqv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3tenfpudn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3dapqdwtr.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wvrqexpu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3gklaelht.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ssqpbsxt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3obhtnjha.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3bilimyqn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ayhwqfxv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3vbjuzzco.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkzuozjl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykszpbwx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3loggjmez.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3axcycdxp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3pdhhtgfn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3awvxmxcs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3oxikceub.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3qepfrkgu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3dcngzmax.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ztcquugp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3tvwmovbr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3glgrbejd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3flrmbfcz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3toajolmo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3qvhscpyx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3velbypml.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3epqxgott.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3rffstuju.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3rdenyilg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3qwvsmkhb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3elluxuiv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3inabxpkd.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3idcisrkx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcfqcrke.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3fykbansr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfchckki.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bmdxiipg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkazkhsl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3kvpambcn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3lgbpnnkd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3lvgjsvud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trtrixpm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3xkcfznyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puibzpge.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yekpgpto.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fscvtmni.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3chpjcnww.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3tcpjrvtk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pljbjlhw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3qlpkfeho.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cwmbsnqr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3bsryfrbm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wtxntode.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3vlicdcuq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3pupzpbtr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3pzbbcnyk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzhnxidu.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hraksyyw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wrquaaao.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3cdzwrijq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwgwhocy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uiktebzl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3boynuida.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bdhrkjtd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gvdvlsns.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzpqbpki.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnavbzbz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ygkyvoss.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3pdmudaol.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ythirpzl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3vvesdooi.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3eossrpro.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yuejrlwe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3lsppjzyv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xjlcthwd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bafkaslj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3epbqyszt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zsikstvq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yxvmqcgy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jnmowknm.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3qijdesrl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zqhqoyhm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3xxiaxzzd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3evkgknuc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gupzkpuf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3igjfzsec.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3tnlbnski.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3shddlkll.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3xkqhtmgn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3geluutuo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hqqelftc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3piwtjjow.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pkfwdcws.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pgvqhrld.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3rqdwfuds.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lrjrohjr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jorbaxsp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jkmswpkh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3shvijgaa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hukvzeaq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3tfubeyxm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rjiksnbw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rauboneo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ylolmzay.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3lrshtgtm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3swyksvou.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqesoro.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3wndbxxgc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3nzodqkfx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3jkhjkdge.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3veolnmcp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3injegywd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3fwgyublc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3txezsjuk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nuykhftd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qljendll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysufmutz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3rgehieam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bywaqbqu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3bcpldygy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3szdkuzri.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3tpwtvvas.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sxpenind.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3phzinqfc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3zeeeffje.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3bvpayrev.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3pficuspo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3esktamao.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xbgglrzb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lyhcoodi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ffwgltan.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qgfxjzrx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hwapnrny.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3udkukogm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3bifsxcbm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fbshkgni.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3abrvosrk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3sicgvinf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3fbnrpurv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jkvkjvxm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qubktyta.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eapospgu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3mmwmpibk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3swjzqzgb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3lueuinyj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pgobyqje.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3gdvzqiox.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3xznfhaam.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vjthpbtt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vqgcztrz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tlvpwimh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xezdubtb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3vvoykzvo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jqjatwty.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3actyyagt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3muhmyoii.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3evvawjxz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3doynyuvg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ustvowsr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ldzvqskv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3pblfclqj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3krirykvk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3pmjtmxmd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qhjrckot.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xeialbmw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3supyjaxh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zmpmcymk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ftfyvqsb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xbnaltln.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3prtgksho.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hxevcert.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3nvcxithz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3icwmwkhj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bcfoqojs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3jqlmjqws.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jdbtaole.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lijcwfnq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ohqfcqlt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3exurgeod.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jvfmgxts.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ogwjqgrl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hmilumuh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xnmqkwpg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ernmelkg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3dknekfhd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3asykqvhm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zfboikwb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3tfyibsdz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3jkzewmsx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3aehllclb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vkoxuqtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjyivgfs.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3eyajrqit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbmojnrw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntdlxzfb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bbjnfguc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3vwinajyp.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3eiwdtfzx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ccxoadli.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cdxrilro.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ootkppdn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3endjwywt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wjtpoqzj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wzlhptxz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rhlrlorv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3drolmwnj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3onazoetr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jyivrydg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lnbkeasw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3naldnuev.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3nkdsayev.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gnkkldfp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nsjujidh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hkdoqakv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3dnujgqjd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3posenzdq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3duhlknca.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3amzlxvuj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3mghehomn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gohyabfb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ptxhzpvd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3breycuos.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vcpogxsa.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3yqmrcvqj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uravdisn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3voweopjh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ivhjpuoj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lgwtpkic.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tfxkpyuu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3autgdbcn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pjnnktif.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cngbyvvt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zlfpgxgc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqjzhuyv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ikpzggry.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ojnpbzth.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wkjfbrmw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bwsjdxuf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3kdgbjqet.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ffrxjwkv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3flcaaceu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kxrjcrhw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hapksxrp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qdaybupr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3kjnwxics.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zfaqwuaj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3exbscktx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vxdihyde.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3cyezfndl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3iqquyqyk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hcmxidxa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3iorppttb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3igznjtqp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zwzezgzk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nvfjgjqi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wouzmlqf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lppspbri.html


<!-- 参考信息 -->