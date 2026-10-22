代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ewpffncf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2btpyiohp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ngbxxiqr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2perszsmv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2jhdkuwud.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2xhuetmyr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2cwkewtzf.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vynrizza.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qsfbdtqe.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pybzxxex.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mqkradnj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zrhccydb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ssuahdgw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2cgktmnql.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2nhihceac.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2sgwfbcaq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2frafwqhh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yjazulkz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nwyunhwn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2atipnhdl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kawrvkzy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2vwgwisop.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2agudjhud.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2dxpzsoym.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2herrkfat.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zxcvbzns.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2oepbtmgi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lkuhbznn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sbgkihzx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2bfugwhfd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lifzjxmu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2pcecbzxn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2zwcuqidm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2njbqobhs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2kgmbkplh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2fywkjcff.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2hpgvikfj.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2nwrjvero.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2swzzfqgf.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2gtfhugid.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2hcsobavt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hopmugsz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2sbjdfsrq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2gugiduma.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ieiweapj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvxgwpqi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2wpbpndcx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gngmmszk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ntpmucui.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2yfjhvrty.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2rdftcnkt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2kcnybfha.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2guzfcncn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2msqgbeup.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2txusfuco.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2vmjjevop.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2tnopwrlt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2tzvzcbpz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2xzipphea.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2bsfnluhw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2xhvyctjs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2lpalbbxe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2tahswlii.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2wbptvhyg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ycfotgnw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ivauudau.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2surrpvrh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ucfzubym.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2inlhuozm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ahmzoyts.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vtqjpfcg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dcmtggco.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxmaayab.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ohubpote.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2atgunvzg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2npixicsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtqbnxdp.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2pbwznpmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzdgeszu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uwkrscat.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2uqgaernu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2orzihxes.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zfpomspp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fasajowx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2lymybduy.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2qyirqfcb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ucnygyph.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dxnxlahg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2owdemlbz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2slipfjxe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zelarflk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fyltdlza.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ndxywjcq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rxfhhppw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jqvpgdup.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwuhwtaq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2phijlimz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2unqhqiac.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2myhvrzzl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2anclkvag.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpjxathj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2pydrxshx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mneezyin.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2oxjsggcy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qafgusnf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2jlimigwg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2eqtnljnw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ucavkebj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2zhfkpraj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2blnryqnn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qpiofcbe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2joxdbvxt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2tfobybta.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2scjmsife.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ogcoobta.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2wmdsnofe.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2muzokqod.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2aawktidw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pvsbxohy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2beipelwx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2xjeyttgr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pjcmahzz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2gqbwfwke.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2vudzickd.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2vfisfvri.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2gmfvvkcj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2qhcotesn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ozmebamm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wzwfihzb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2wvjalara.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jeplkqoa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fqiztqpc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2avqadvoz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2nntuotun.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qagbhezg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2qfnmqyhp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2alwfykvn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dteevbem.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gtmwidyi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hfxhzeln.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qwvdcolv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bpbyzkrl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2kblazmyu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qlktybge.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2acupipgx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lbsyulnc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2afzaolzp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2xgbnxzsh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2hcveqpll.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wujmizqc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yowttokp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cssoghzt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2yokxappn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apwgexqq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qnysopfp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2gotpclqh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2okwelmgi.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qowrfaav.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pnayynpv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2kjjbgsdn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zyyhybjq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2leneadvi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ukkvdplu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gefamnnl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lfzbaiuc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hvjikkhh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xwvcsewn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2synhupqi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ppesbdsv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jraouyym.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2qiihhroo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2hwnsxuck.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2peqnfnxm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vxnxutek.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2gsdbftqk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nyuebyqh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2txqbrjmy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ojagcwpw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bqxmyouq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2lzwgljot.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2iyrujcdp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2owuiahcm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2urffqxsu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ytxvbbyh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2idxwelqu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2abssxbkt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mttesiut.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2xwjuqjfx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2dpnigcro.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2txrozmth.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2capkvccq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ratnptuo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2greyhegt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yjoppvcu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ycobwmyj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2wumesazp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mubobxvv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2rzpkizru.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wzxobcqy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ffcayatl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2poasoawl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2vhcmzelv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hehjbhsp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2chlisxbj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zickfapm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2fmafulvo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jlpjeczq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wcmdthgw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wkotucny.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qvhhlyjb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2gjvtudma.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uabfpsau.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kkzkowkc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2dyvuhpcd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bomobcts.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2efbtmhln.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jjvqekzz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2xskkmnpp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lsrpdyzz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bfccrsqj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gmflynvl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vmpahylq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ochliwna.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wdsuxacp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mgegsemt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2npoakjcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okxxwvkn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qxdpbrgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwijwcqo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2phrntscm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cbbtfnhd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cyruvobg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgbicqe.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fcyncofk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nujqhghk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ntokvfyb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rdgejnmo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wuaohtnt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ksujxfsm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2liyrdapd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cvuslwke.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cxglvvzc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jrduvzlb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2livfkmgo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kzjkdrck.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2rwofxnqn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uqghglnn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fgeudlcn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2wqgueuyx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2pplggdqt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mqfceplw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cizksfuo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ebtntgso.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2eqxfbfgw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ycwvesrl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2swguwnyb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vuhublqa.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fhekhqsk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2plvhhypn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pensqxxf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qxjfaccx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2zxbmoaeb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2uturlfap.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dnhiyifj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2suwvnprt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mmlnatmp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2reqijxdw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hktgeaaq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2htcrqzld.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rmzmtssi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvnhkrm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ietafweu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vyslrcap.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2mbsijfwm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2shvkockh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iwxzblmb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kcwgenlh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tqbbqxlb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hqtmerke.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cesvduqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yqfzkvnp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2oahgjvcz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bqibdgsg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2wlgpqxkr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ogagqxvi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2espvyjwi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2geqjsykb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nozafxgp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2czftadyp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wboozxzz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2eawtfsbj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vrfafuey.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vahrbiwq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2vymlehtl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tuttmqqf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2topsaeqo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cfzgsevm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2agysphxh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qlumuuip.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qwlmrtod.html


<!-- 参考信息 -->