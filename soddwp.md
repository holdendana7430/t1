代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2djhjnilf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2eroxwvtp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2mzgmacki.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2stsxbyoo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dswoyxnu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bsuxvqza.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2wmvzvdsa.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2mbukhsou.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2iabzvkyr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2xfyytscl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2lpzinzyx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2gckmvqkz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2baszrxeo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2hxldkhtl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2anvbvtej.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rjlglckt.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jxqtznya.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lpccijjb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2avqsnxax.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bbjvdfbw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2xltlgkws.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2okwkjopf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cgaxdjkh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2vnyfkwgf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ztspgmxy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2msghereg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ewcauupv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2pwkfztnh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fjccfyns.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gfnsgtax.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2fphxwdaj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2vuhjcemi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2thympeus.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2grslqjqy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jrzpkbcc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hxeeolts.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ktstnldd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2jvjwcgyf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ifwrptxp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2jnpucugb.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2eombyncl.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2idxkzvyg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2keykesia.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2nmuwcult.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2nsixitny.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jthnkdec.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2sstzzbto.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2qcabbgre.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2bwceglbl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2eryunpet.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2zezzvrvq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2zjgpwhbo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2aqtapwyo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2qunzjjww.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2xxpvcksa.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nlquvhxr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ypyhnukr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2tcmbxnth.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2hcmmgcjo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2pimwcivr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2bpysvvnm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2lsmtcpjh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2letgvswh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2flsamiki.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2gwppyyui.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2mrwwrabr.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2vvuurnlq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2vmastadb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2kphkfnbh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zyzmhxzg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2qvoqrblx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2fltjdpiu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ejznatub.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2gpvssbnm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2cxjwffvb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2eyqwpxvh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2sapadkzq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2euycwhge.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2rgbleaad.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2feomjkkg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2pnsprnkr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fkcpqciz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2edmbsezk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2xiyahlpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvrmszdt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qsswapti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwzgjhdc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2evtyzssw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ktbnsdrf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kipzgevj.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xldpibjc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2nsynkfwt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2oybgwjbo.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jptmmsxp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2nssshafk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2tonguzmz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2kibbizug.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2eeroembm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2cmxukijl.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hotqdbuh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tpyyocap.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wwuluakx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xagdxeia.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jhdrtiny.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2lnsphiew.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2hggqlaaf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2xhsgycnh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2whlwdcce.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hfmdmwjm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aftjyril.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2cogrbbyx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2rfhuyusv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fkkcrfmd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2mpsfgcwy.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2dchmrdeu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qtuotiec.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2iougennv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yvduaxqk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2oikqfcqd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hlrrggba.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xdsolpdp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xlecuien.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lyofhgig.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2kknndssw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yonqnesv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ohadhbyf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pfpypzcq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hjyiwqss.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2mxrebwnx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2pqxvjmdx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wufycdev.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2cnozgyvq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ojflrmtz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2aclahfrc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2lbtvvmkv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cmvqrckg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mfjqrqxr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2tmlzkioz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zhlzlpgf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yagyjszb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2sjtaqhys.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ehtgxqxt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qgndthim.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2pebiebox.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pfsjzauh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eogektdj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2irmccvtg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2uynaksbw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2yerotjta.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2defkzskc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2peextfzr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2irufiilv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2czbkfqzd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2fbsukxnj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vluzpkpa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2fedwpldw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2iiffdmsr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dptkclld.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ntuyfybm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atmhnfgv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ydjvpuqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phywuudq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2fefidthv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2idlswowl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2sokpeghl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ygaazkdh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bbcjopvr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ndkeqsip.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2snqiglil.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2cnuauvvv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lqvfqsjt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ksginwzz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ahwuyutn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2agqkgdwa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2atmfsldt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zlwrnlvl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2eolnajeo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2vwpkadwk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fmothcbf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dxechyfo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2yobinbty.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nmmayijg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tfsqfyja.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ravprkdt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qkmzjpgq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2mcipqink.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tbtndbik.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2uilfrbqm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lvkjyzhs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qarvcffs.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dguxowxk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lzpfpgda.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tpdoahmu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fhrmomar.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2auelnufh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2fkajxxnx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xdrtxeuq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ptltztzy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qqwtduyu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2xtiyegdc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2yesqngmq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hvgklxpg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pmvdgkmx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2orfeswah.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2sozohdbs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2qaxhrakv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2amsbgakt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2smvflmvx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xvhwumnp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uiozafuw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dykbeqej.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ujictpmr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lttturos.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vtopeqvv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ypnbmjrm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wqymgioo.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xlgxbybo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2uoakluwy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2hgbmbtie.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bhfwjrnf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mhokhdil.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jqoigdni.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rqcpmnmf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xlyobont.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hglqfzvp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2xxakewuj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vrjrcxjx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2sxhyrewf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ujqkyywx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aigbxhhw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jwahlpug.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fzqkrnoq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mkxeiwhl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2tzllixox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzuhzywp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qwzstnmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pucywiqv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ymsngslr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zifuxqps.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vomsrwvg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lhgaedkw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kfsxfjkq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zaikznmk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ohgpwphs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2yuipuqwc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ztfvlemi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kthwiosx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hmajvdjj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gxzvtndz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2shufklnj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2piivvbcw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jmigiviz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yzielnrm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2bdwtiynb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ylcfyust.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xeudraye.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gurqrqls.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2kyojqqlz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2coplmznb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sxmgejga.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2nxjtswvq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2oykihojt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2olvlouww.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vmgqyzxo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vpkrslek.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vgxlmgrs.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xedchdjq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xlkrrztz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uqqpslkg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2sgubkibn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2htilxzoh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2msmxhfif.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tpmbsjut.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qycwgqny.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dxzwaeqr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jftwnxdj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nrsrqibc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2naiiovpt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bsnmxbmf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vwnglpak.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vgpiyrfq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2upfbzwky.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dahfiqkq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xelwywvj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2axjayxbi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yaimdgux.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zowsmhfn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cebolscr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xvsskyce.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2sipdslgp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mpqklual.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2szyylpna.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jcwajvxv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2yhylbdln.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hiourtlq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cikatmda.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qnnkcetx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zedbrkyv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gcwoztbn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qsvaashu.html


<!-- 参考信息 -->