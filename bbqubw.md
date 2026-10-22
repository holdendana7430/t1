代发 wailian999

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2czrcjpcw.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2evwpimmx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2upyhxqwp.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zjftvndl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2pqflukas.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ouzmzouv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ofzwnyaa.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2zqcysmua.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2fjiskcqk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2bjmjywud.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mcraaptw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2bivadpmg.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2gxtdqtuq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ogueiveb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2zrsbbdwl.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ihlyrcgx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2isweocmi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uihzqjfj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aeidhygc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bcdasfhc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2wwpoolza.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2dnovgeft.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2luqdfzzz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2jnxeutrj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fqpixglu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2tixdslek.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tgywcbdf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2jukpzntf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2iqcxvejm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2pjlsnxom.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ovxxdhik.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2mkonkxpx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2vwtfxzil.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hsblgwai.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ubhbaiui.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2klyxrogi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pbihieif.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2lgahhmjs.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ohmhxlyd.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2lhjjbbal.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ohmvbzei.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2uwyjzxhn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2jscpxwef.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2kfmmvwqv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2jxxxtqth.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2shrrsksx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2yfjjpzui.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2cwlerlam.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2zrnsqhlv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gsikvvgv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ezpiedwe.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2amosrjgc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qmjjaeum.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ojnpcpvt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2pklmdsst.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2prhgyehn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2aearcxwc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2bevutdmz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2uvozfifb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2kkrjcozb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2xegzhhua.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2nswojiil.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2gcaxyhud.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ghggarll.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2eqtwccfa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2bczashlw.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2jlcgbmsp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2tqpvzqsa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2lzuoaafm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2swdoptns.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2aptqrlol.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2iomhttez.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2fnuzyove.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2kxnzkbcs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2mhstgtkd.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ihomjbim.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmakfhng.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ukmiilju.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2sufhukmh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kvtgruuf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ayovgyzq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2phocqutk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2tggfrfzl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2xgskcukr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrouuwus.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qrsuwvrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wriebflb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2rkijcpkw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2pnugxrpw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yhmsagae.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2kwofqioj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2thrdbpep.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2itorccgf.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2djzaecif.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2awflrzbs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2phmbkuug.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2wsisfwmq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2fitcwsxc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ulenmwjz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rrmeflzu.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nwmonzqx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mtsqjgwp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2bqstxyux.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uvzkdkvj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2szadevsj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ibimuolk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2crwpffop.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2nzqlhmfq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nnxhlkwt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ccbeltro.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2pvchzaal.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2bgnzcezt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nwnxcmpm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2wvbeidok.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2hoqlznog.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2snzuxtsi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2atiblivt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2cuvvxzdd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zvaubsoy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kyowmkvi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xscgozei.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wfajharf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jbxdqbnj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2yuijgcxj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qnfkglvb.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ohdtfzha.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2umedhvsz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iozyrcac.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2jldbkjsz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2hmlctljq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zjyospzx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ebxplndq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2jkzerhbl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2khhvbetw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2psefdaok.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2clvojahi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gpganmik.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2jhqpsnaz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ieqzbyuk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qzkcydlw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jhjzdcmu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2aeqomjbn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nanglkzw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2gposuaob.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dakwanpt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fyzfpayl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dmzesgpa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2shrkfsht.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ntxgzfru.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jjobainx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2gjgndttu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ainwwspx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ogvilzdr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xvntkdwb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vfkfrfdw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2sqetlcqc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2antssdqr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2evvslfgs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2thkbmkyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvsxhmfm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2rjgrcbhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwjieoke.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2termohob.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2piuzpjpg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bhkiyftu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ygmwusqx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bzkagwfa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2nzfchdep.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2jcjjixoy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2uiusvvtj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2puntlclh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ibqpcvxp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vkeuihgz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2fmewrkvt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zxruymjb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jmnopite.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yeaboayy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2phqgachh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2osphcjzt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wyrqiugm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gfwlhtly.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xhlvzocp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2miqirkuo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2eqngudzo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qrxsqmdc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ugchkawb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dzkagphs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ofhxkhhs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cryufhsd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hnynsbdp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2damcdshs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2uysbwpjl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jmvqwnrb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pvdximxf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2qoyrhfgi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nxjkobms.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2stnsrelb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2iamfspks.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2pcusgkol.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2jcdtjber.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hdzemzms.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tlbukfqt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sijjtgro.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2irdzdonw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxhyyzis.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lrcxacqz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nfnhgzbl.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yzshokws.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dodrcwbv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zeialsdo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xpqpfddw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nnswxgdm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2auhplnsx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xducpgtr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2hmpmdgod.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kjglnujr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zpcvouzj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2udferchg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2pduklgzk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2oukbbbrw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wprqhmrr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2nmgwgpls.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rgapxvbt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2iibyrpxa.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fwqgbrbj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2xiyqjfzg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2sugtrixv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qfyvtugt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bwqtcwas.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2daljsdve.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2spdkadjs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ewasvziq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zhhcsnhc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ywqqmyta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovtssmuw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ihkepnoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vphupclc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pjscuohh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vnrvmhuh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jghxvvkc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xtcabttw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2iohkrtdo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vaimkxay.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pngobcrs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2iqbshdzl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2sgocqnaf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2uflmwotk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ywbcwsna.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ujgciuro.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mdzakzqv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lfjgnhfb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wfkiochu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2diawhbyy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2dqhzwgrf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2loemngxl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2juxsnxsr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cobkstfo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2awugcekk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vgemjxyd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2agvskmbl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mrpqaixj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gkauasng.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2galgftlh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vqrqngba.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rpgysutp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wivqzflw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2wssyxmfv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xbkcdndt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zppgbwao.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2vpmdxtfu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2veppvqeu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hlukasjy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mpzhnqvd.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ixabeckr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvkuvoyz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2dxokgsby.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2voxdakhl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmknwjyp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhygbadi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwqgabds.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2erdryxhj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2uwbxrdyx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mgjwnixg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bjeklctf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kpfomltu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wfrkfuex.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jnveyaeq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ranzosjx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ulbirkks.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zlcqajbf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yepqlhda.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2yvhofdwy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2oqidjkug.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qbwtzlzb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gxfsjsya.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yqqajsez.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ooxlttgr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ehoqxmth.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qkckgjon.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjfmpqo.html


<!-- 参考信息 -->