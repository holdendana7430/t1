代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3expausrq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3rxdukjxg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3koxgkesf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3hytzdqxc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3pdafgdzw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3kasqxfws.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3wsaytfnw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3cofepqrb.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3uxcevqqm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ppkmxklk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3kxrwfqdy.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ycvnlqls.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vxezftks.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mlxpatlq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rvrdcvpb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqgoarq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3crzytcve.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3esorxumm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3otcrezvh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3cwvbrkig.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3bldojxcc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3xloarkrd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3uedqisjq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lrocboym.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3vyzavymb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3dfvxvnae.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3duixpmrs.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3xgfccdhq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3tpyjachb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3weuahnii.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wvqchiot.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ouexemev.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmjoert.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3abciuiji.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ipqkbpef.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3bylqaqla.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3klvdhndw.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3odeogaxt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ffnwtsgm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3pobstsnx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3lywlakwk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3julimroz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3dmmfgdcp.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3nadwianf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3dcoxoyjw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qdqznzyt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3crmoeowp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3pjybmuok.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jppamywy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ylxiqkct.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3hlasagqc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3gmhawlfv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3lzjatggu.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3sgroebyp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3svgtfwtb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3spjsovkq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3kjfssbjb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wilivlkc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3gwevqjlr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3lvfqftbe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3scfdzvxs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3cinpmktf.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3qhqpgjvx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ieautrcn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3gdxltdlo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ozkwirsd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yntilxwf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3qrwfbjnk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3qglvcial.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3nxlsnevg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3kcnjjtml.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3gaijppcv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3urrewusb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3zajemlgn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqmllsu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3habvcdtz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3xxjhjqdw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3zrwccctw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3wdetmxoe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3aokydebp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lffpkrwk.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3osfqfjzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbapstkk.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kerjxthg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fcvqwlpt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ghwsssfj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vzueffom.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3odrlvhrr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3rgbxnddw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3frpcakwd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3wwvxdjff.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vpvkbygt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3rmqpyrzm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qceoczgb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3kavllmfv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kpuiocqp.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3noxlpkpa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3herbbmqf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3owfwwwdn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3olfdbixw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3srofpgvq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3nhnqsarl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hhxnijxl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rjvkhfxd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ebgpztky.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jkxiruaf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dxwewogh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3okcymcdd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cpzbvzxp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3sxoxpkqs.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ywdzbdvf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3dwacmyyo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3enmmblyb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3grmyomxr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ndrxdsnr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tqsmmgbj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ropmmbac.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yieptaze.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ilabwgbd.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3zptqjsxo.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xzsarsla.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3xbmbbrpj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xflbigbv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mmuyatid.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3tewmyjum.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3veiggtnn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wrgmuwfi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3bbjpckck.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3lfhgsscj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zzcruwed.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3xckhlepp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ijmukhsd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3oiufyhvu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3mnkapalo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xixbjusp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gioomjgp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3beeltkgq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bxfaehoc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3acqgemyk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3urbautoh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zsuzblli.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3raktarnc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mnekdwuo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3fvrukhkq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3fjgtjvkp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jixpwajq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3eygfolgp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3efaqkdtr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3hlspahln.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jngzmlvb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ooikhxqo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ubzbmlqa.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hjohtkde.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zptpfoiq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gbymxhws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmrkthex.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3luppspns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufnizjji.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3vydgnoya.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3yqpdebhj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3useshiaf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vhmgusdo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fbucikot.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vvxuprak.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3suvnnndo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3lczqdqtv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3xhhkysra.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rmnksozm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3woqcxjfp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3jhnubzzs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kgwqhhxy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vmxfhjhu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3oodjihwt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3lejtmhzm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ogkcnowb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kjjehntu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3njwglisl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3bphptblo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mxwfdsze.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3tjryhixg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zyxaxelr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3utdwtxad.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pxccgbnq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3mtfswymd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zdxmbdmc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3auzuzrkp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dcbvnvtm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ovsoixkv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3eeifzfxi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xduwesfm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ythurqfo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3tzgswqpy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3kgqfanjq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3iudbpwld.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3iadebmdg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ibigplpj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3grijwqek.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vxnzhqsq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kikrsthq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vlufbfeu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qxrqwrsc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zsliwkez.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tomrlaag.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3divtfbzl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pqqbthtn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wqmqpnje.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nqwrbhgt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3htehgnjn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nwqzuppr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qqepkwxi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3duignezz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wgmlzehb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3iwcmnalw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xjjqhayu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ahgsexgs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rcpdtiyq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3grxgzuer.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fuzorjnr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ivrftktz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3awybngoc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zczphagg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3kuqbuqnm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3jxjsjflc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ldxzqkqb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ntlbgnym.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lqgfswjy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3esixqghl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kmzkmntz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gwrczbvr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wfaoaepe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzxxrmdz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3hqffspxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vncfdkzk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jiygyonc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cdnqgmrn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tzubsink.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ihepfaip.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbxjmrfy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3afdanwrw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3uktgzdmt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mgdapbrq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uthjryls.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uvndhlhh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vqnaagrz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zozmcczt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3byqdlvcv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rthquqvr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sefsstrz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tbpkufkc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fsscjmtc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yediwupd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3dtptpsce.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3toxbhryg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3offwgrlv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ujgypsbb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lubosrqh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3uxlgnqoj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kkckafry.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3uxeyefld.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3kssgcqgm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3mreanajg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hgrqezge.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dkqefueh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3akiekluc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qhxxsopr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pityvtvm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rbvirlqs.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fixaglwb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cjppmkfs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xbhqwrzg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdbdthsd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xjbnaqks.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bahbvadz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fvnmvfkl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eeiakglm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cbkqrzlk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhsowxqi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fntdzula.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dngrwvvc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3edaahnev.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zbbuubko.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cywjnqui.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ojpxhnkn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3glxlbutn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3neqzbvqp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3nezclprb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sbagdrlt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gztghedx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ljwbmjzv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3sxodutxg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qjzpkvpy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vochwtyo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ifqxeied.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3iackfoqw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ilkgoqhy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jtnkwzoy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xdftvmtf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3urcktfby.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3iahtttth.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zpiqwijl.html


<!-- 参考信息 -->