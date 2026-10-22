代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2vcftdtnc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2tftlcckp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xspczfpc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2vfnjltqw.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2qcbnvexu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2uduvyxwx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2gjmbhpam.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gsjbxmwt.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mghhlfsc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hgqhkqhh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mmmeepwf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mlgktnzi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2rqjtlrtn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2uqvhkamc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2yevmlkqr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2gwvhobga.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2zjdqaobn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2vqciobae.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yalutwes.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ntvyrsrr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2npunifof.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mihiqpmh.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2tsjmdwmp.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2xrorlaeg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2yymhryrk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2pbdwimak.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nxmrkyid.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2acbmhewh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2xnguzwms.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2fgmeyjcj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rarthzfq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2vueigplh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2szghnmba.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2sdtctulh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2sfpkoabd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2qzckmkwc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2daluebmu.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2bdthyxsw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2jyhyqwhc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2vogmfhjo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2gupghmef.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bjeauwlh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2cppvkutf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xhuwuqnx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ldiotenc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2lmkgjzcy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2heoijabr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zpgajgbz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fecifdud.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2gmvnqwzw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2uxsfrzip.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2clgdtfxb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2bmisaflm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2vjlqdheu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2wggsxzya.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2oegormrg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2aqlwnrxs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2yydgdcnk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2srjfglfy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ktwyiomu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2xckafbra.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2gumtlaxo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2huytwhqh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2aprshsjz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2sqqbfatn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ozhanuax.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2mapzebpp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2bzghwbcp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2ygyoqcri.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jrzumpyn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2evquonfa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kzlbcfwl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jibnoypl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2uqkrxqmm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2pxcejewv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhbvlgxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdpitqlq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2clusdujb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewjjipip.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmuvvvhf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2afjoqxpm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fjjhtvkx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2juxrhpwk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jfegzlvo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2qcsmscpv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fmwekaln.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2leiobmtl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jyaoomsp.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2londcikk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hilsjwtk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2geiphymp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2exgsclec.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hhjfhthb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cckzpryi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2uavlsiry.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jpipjcxl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2euwnuvmq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2typnngcc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gudxrynk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fcogtpol.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yewxuncy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ppwqwrct.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxsrxri.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ljyhqpbl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2qnisbvrm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2empbwpzw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2mvxainjw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bzwwysfk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2eydthgee.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zbvfdcux.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2opvhmpfl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zoptqfdq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2nklsqldu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jmpwdybr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yvkqwigv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2tkpvpmpp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cuhwlpzp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2hnbqaafn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dewhdfbz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2blbeislf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2jwqvsmkf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2hrronxho.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2qukddpel.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2qpdanmwp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cmjnxtxm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dadpxknl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2wbnjcqxd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ebyosbyu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oexerqpf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jecoweow.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kxhnllwu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2feghabdf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fgrcxnkw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2iwesqeza.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uyfcbmsp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2fcxhjvtz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zbpmadha.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2upqhobcm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ynuuklfn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zzdrzrsn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2yrbpazid.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xajhgjjc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2aaxgtiqy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vjwnjsdg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rcgpctvb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lxihmnet.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2yttgxcjn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2jmotwjar.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2alpdwqxd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bpbevmeg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ogbrzxrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ienasvhl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qunzkfxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agmnsgfu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2aohllnfn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wcenjohy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2woikzczj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dvgqdrsc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fnqayonu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2gqfcefzh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2nsuxhzhq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2leglkthl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2skyaiglz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ondorxbk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2okofgglv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cyupfwlz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xyzczfit.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xjlpvgsg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2pyvjwmfy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2yaqoyezc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2poczwrrc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2agjdboyr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rrhiznij.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2siexndtm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2tsgpyqwv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ozpvmhsw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yftrgrzw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2tdojaffl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2upxpaeur.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2yrevrblp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tiarhoex.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2dcivmmod.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2pfhbcstw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2inyvixuu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2icsuzoyh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2noozfvqs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mzrfuenv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2xzskjvmn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vpecbtlx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2fejbbvxn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2snslbbtj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2bqkgofvb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rclygzls.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2acbgzbzh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tyuxblsw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ludsezkp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2epoexyox.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2uogscncz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2idcuxupk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2akghquhz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oczqkytn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2chwlohcu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qrbacsbj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2raxlqwex.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ezinomce.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wizbrbcl.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wftowdqu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mdvaezoz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ppcensnb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kmycijvz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ocsmmgio.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rnvjwjnw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tsetieru.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2zoezlczd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zthebraa.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zixyrgqs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nupxebog.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2hrclcjjn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rxlmyqqk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ghfpnath.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2udtqchpw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2acefikqk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2obqwlbjq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fdubaemi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wjjdypki.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dqvfkasc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azveqyku.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zhtkobbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxogsnhv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2crjwokha.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kmywjmqd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kjemtshu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2aolckasz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2adnabdnr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mrxpnwqf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2igfmdpqr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mqlhozlt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zrhmzexm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ihwrasmh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qweqplnx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ppnwouls.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bojnzljd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2skhhrjpr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uapsxkez.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ndmjmtnx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vdvryeip.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yzpndklr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zrrvqlew.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2yoabxsqa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qhpcboij.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bbruzmew.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xystfdts.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2faksbzyx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wcogsvuj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tiazzbtm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2qqudyhar.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wwaqaiht.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2rjtnbrzw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dlxzgevs.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gxoxhqgw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xcywbuqj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kwwygvnz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qtaceuix.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lpzqkces.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fpbmdkxf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2cybrgepw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kwjpcloi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xkvwugsn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lfdnkidh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gacztrbl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gbimnxit.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pjegmzuz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pqarpopn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2pxcdcmbp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2wmtdamwf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dxmmlwnw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2cmhowwey.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xhgirmqd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ndxtbity.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tejwjnby.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dwxsxkwc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2fdqmxqux.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mzutsrzs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mekgukvi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2kdewlycl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mvncarjq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xtqohqsy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rsxxvnpx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mqosfctq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2umsmjngl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wzkuwsdk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fnuelslp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kbzkuquh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qhnyulxz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zqylrwyd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2czoaaegg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mrwavzrz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2hvtdrnff.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ifrktauz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pixzynmu.html


<!-- 参考信息 -->