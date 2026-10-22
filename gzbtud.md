代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2tdvfsrby.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2zbnlitpb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2jubmwagl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2wudchrxs.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2lgvucbaf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2gchlvacm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2mexpihlv.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2stcachjg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mzmsbjln.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2oexprpsm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rxcaucvl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vyuhqyza.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2iwtsrpig.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2tkyybcex.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ddnzchtw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ubbiiypy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2uoiauyhz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2znozxunf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2huwiqedv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nmkdzixc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ejwlfmcc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hzgklhst.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2howryufg.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2bxmhboas.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2gobjptmx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2epjhddis.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2bkxznpdl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xdughdci.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qmjbuvxb.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2xdjyrawa.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2qnqrmedp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2icxforki.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2husohxwk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2cnftaiyz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2wyoeuvrk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2zzeinfey.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rplnspyf.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2kginpxzc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2zlklyime.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2szmbsceu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2uxxjurlo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2dykpnbps.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2edbunbmg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ujclhmrs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2xmpmhccv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmzfbkb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2dnkbbnuq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pqlhxatt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hfifhxgj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2acrwflrv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2csmnndpv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2mvqtkzmq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2lxsqvktf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2tddyxbka.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2gmwbmjoo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2fqzxnikm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2grtoxoiu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2euiocgab.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2jjqliugf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ygokpiwk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2mfnnwrkp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2amxbptfa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2novcanzh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2otzieptx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2kslkutpr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2cxkcvchc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2gulobeok.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2jpfqbidd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2uexyeopx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2lrvoelmm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2kwvcptvb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2tvvyxeui.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2yxlqbwbk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2chqpfwir.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2mnwaerjs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mczfkwyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irwmzpih.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ruddlwun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dinrhpoz.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bubzbxax.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ouomoddh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hdqsqkli.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nhrusvwi.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xfgqgmra.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2opnhqjge.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2onrxnzpo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2fschajrm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2utdtfwwi.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2leehkkns.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2jewvilxn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rdlhafqw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vfentiki.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qditykdm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qvofokbb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hitkzkis.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dasrzkco.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2kfiupkae.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2kidvjxrm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pqwebiwp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2udrjrxjo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oacskwbt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2tjhugzza.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mvnqjubx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2duvkwzil.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qedvyrzd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2grzozjjh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2kdresvin.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2toxvayof.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bagegmbh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mrqqxnev.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ibatmqth.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uzefnfoj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cmuepsdo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pfueowgx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ereauptp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mapycjeo.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2anoqcyox.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2xljticll.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2syqxcsxb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2axseykbr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2eokhgnhq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pkaebmrt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2fqxgxnhc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ftqiwgwi.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2gzftgvcv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xnndkzqo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2rikvoiun.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qkpllmlf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2egphtyxw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fvtwtmsi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xyjnbebv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iegrtuga.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uoxnepeb.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2yezwzuqu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2crwsakhi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2yxzjccgq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ilkhbisd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aodldofl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wdcwrbgq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sqbdrfxl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nafjrvdk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2orezdoti.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2npcwdmbm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fvikggvb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2lkhszmkk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nrwlqvnp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2yxlxrihx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2mbzmpgvx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2xbaagpkh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2nwahcxli.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pxyldnpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2latlkqyu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2cjehdgjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwivzrxl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zccooptg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2mextliec.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2icsowmpr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ciqbfhga.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2chuaqtkd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ipsxnhev.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2vmkluahb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rfdhrrmc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vcmviqoc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2frjnqqss.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jwjnoyfl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xwicjfmc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2esasvyak.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ssstfnme.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ctaaipky.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2lrvcgehu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jhfnarjk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2vwwzzijt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2yvqdihiv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ykwsoamc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fdnsvjkz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cysdihmm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ymdmgyro.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jskdspfu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lqpcbwjo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2rnzsyazj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2czumiwva.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ngbnpkwe.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2rqwwhjrg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bglgmgwr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gzbrcatr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lgukrcqt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2hrxmluyn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2evmelrbk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jpqoslbx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xeotazro.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2wsahpnpt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hcywblue.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pfqpddbc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2oiiawqza.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jvrklupx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2dyaxsbaf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rokydhjr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bxdatlsl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ulbbpopr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2pvzajwur.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sxxuwwam.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xmghqciw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kjdlhqqq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wxvhnacp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2djcixsmq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ssinaexj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2qvypzgtu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ppzasjdz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gcpwokna.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2uipxmdrm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ktcwxdlj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2thyvwfff.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yhnummkd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2tcgpqgpl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pxwdnnwh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qwgcqabl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vttskhwg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2myjflgyc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ksccrcpv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2navvqnja.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rhebcghl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2viiyiflq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2yjromwdl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wfsopwvb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2anvrjubi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2tnnwrouj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewodioqv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2uloekhok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcnfsqyn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zhlwqxcj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2mqfprjsx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hiwfvkkw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lylxekna.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kzilqyey.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fkdeetft.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ljbagprp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zindhgvm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ceoiszcf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ccomwoes.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tmcvwlfe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zirxrfxb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vxauznxe.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zmohilum.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cdiqzets.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qgayudta.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ekmpxvqr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2olccdrgw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sehqsrvh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nduvldkm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lailrkvv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2seblzakf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fuqkhevz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2cnlcrnib.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vzzploca.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ajorkkii.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zeehozma.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2sbgkdwry.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2blegbbds.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2robdoflz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vptqbpzw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gmywnhfx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2tsaaufvy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zjhdqueb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dqvbgwiq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wpzcwdvw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mnvrgjha.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ixfjfahl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cgugpfpn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbkfhozc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xgztmcbm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ejhsimah.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fncilqia.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2brjkiedw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hibczpub.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dbdipkse.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xxocjbtt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qjysltvp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aykdehsk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ewkcbvzm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dpymwpyf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2andrtxjc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bpbnhsof.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ghjuxkff.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2sdivqbbc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zqhyeuzs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nvfzihgz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2sgcuyeoo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cdpvyqgo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lkbvakxv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ncjtmdxq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ctkbkpgw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2agcoazbv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2lewmpngd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mypurtkd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tszobmiy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hvtrobvs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2stpdjkrq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2kjjinucy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hvsyapph.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rritjgxi.html


<!-- 参考信息 -->