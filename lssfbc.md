代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3oochjomm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3kwnjhlzp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3jxfeiusu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3zbrtidik.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3yblvdgap.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3wmkcbhgt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3gzlrrcdg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3oqzilnhx.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zmaoegfd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pcpfzrkb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fdjucbcd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3iqganziq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3fvknitvo.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3xarhukxl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3geeymeje.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ebzfuxzl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3wpqqscoo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3spzpcors.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nkwutwxa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ppxlmavq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3igcxusmr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wffihecc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3nwbejqzt.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3dltdingn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3wtrpxsmd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bqxkjquv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xuelcufd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jplqlzqb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vflraejx.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3axpgtwqb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3squuqksv.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3gkkgbcmt.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3toyolzto.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3qwhvnhim.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3qhdxwwvz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3uuwqwmyn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3vxqhrcwd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3kumztcsj.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ehtcoire.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3zhlditpy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3lwlxocum.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ycnsplzw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3kiloudex.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3joypavsb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3tqggoape.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3hbhvhzga.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3meodpjsw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3byghxrrp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3hexawvfv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3mgqprilj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3duhgwomm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3plgptpun.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xxubpkzg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3fwvwwewh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3nymotosy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3reqhuegi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3vzwonyya.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ncmfemyz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3dycbocwg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3aijezjua.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3enhkujyn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3kkhaawdt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qopnttmb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3npvwvxvx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3zumugant.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3snxbtlcc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3krxygcrv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3zpgeeltj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3iihqdobd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3jyadssdd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzhffjtl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3edugzogp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqjdxvcr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3biuimwsh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3hdbvmnxo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmvzhqse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drrexraw.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3gxqphirl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpjeyauo.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3hhxijmey.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3dsuyfvwi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wooxzidy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ucycgpou.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qlfprvlq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3nvzidhpo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ahdelwgd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3hrokpnwi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bljcxcpc.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3wguqnwqo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifsofrxw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qrmijngc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmzevqhy.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nktdzboe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wegxbsuq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3remperkj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzdlbqkq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3usjpgjlu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3cipgpocj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gslurmre.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ppqnprpl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3uageugee.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cvdzpnax.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tjbkuibq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3shmudtsk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3turspmhl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3oaexiysr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3anjlorgo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3rtywmpwf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3uxbltqvi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3blgbmazg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3iczynvsv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fvhnvhii.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3efeklvij.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xwlbzxcg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zgduakfp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3gyrrepgk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bmdhxpqn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3emnfdqko.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xjdfdtcm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ltaciqiu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3skyyiflg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3tallajtw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3agtmzaio.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3wminffie.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3jddscfoj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ezlrzqwd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ydqgykym.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yjecahhd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hmfxqxyz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ewbqzaxb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fgzactcm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ygfdsbeu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3acwgitok.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3jhqjrbws.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hynxwcei.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vnnhvffb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xthbpjlq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qusiknuc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrqlutv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3gfqqznzh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3effqgklv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uwqdntxm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3plvbhxrv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3oxvlweik.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qswucaxz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pnsvrami.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vybzzndu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3lqpnbukc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3qrzlpzjk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rlkolcpv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nuzunsaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpakqetx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bjdyneqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pyjhvxab.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3pcmgyxkp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3rmwqhykl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3vssckgdd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fnwqplgb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sxydcpja.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3kxoirdvj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ttmnwpzp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3umjfzbwn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3wzmonigq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vpnvrapv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3eljlurme.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3wbtqzyhm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rzqorsch.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cuotqjtd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ksyjvojb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3batiprlf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3mghaytah.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3uyryddlr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3dlyrkghd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3pexeioti.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gslltfdm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dqfycquv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dsmckvum.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3yrvszblv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3syexxmsx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3aqniagip.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3znxcsdxy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3chsfqxkb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3nqaxzjdq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3dcyqxttp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jyngkncf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hercmvpj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zmjmkwhj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bubiggxa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3nednkjwc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3wxxeuqtl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3sqctpmov.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ojmyqtmr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3irytofqg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kzgnizwq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hwkzudvi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3lnvvqcie.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3sbaayiga.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3uvmbtxaz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kqjizkhx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3yjbxsttq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hxzuzkob.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lrsyzure.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tlxhvgzw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3weiyxdrj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3djoehgdu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3disbicwg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mounvlmv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zqhbeqsk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nuarvlyy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wasgxfki.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3aqjgyxyo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ffbunqiy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nsztwaxm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ozqsbibf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rrvzalrb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3sfpwvscq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3aimpelzl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3hiszfabg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wdhdhpqj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vsaevjds.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nrwyhjlj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nnwuntbn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3nwtdkgzj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3cowbkuvf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lnflolue.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ruhedmwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgqlnamn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hxmptalt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owzznwia.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gbyhxkpc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jxmphtnr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jeizgxhi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3idpqosmy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kfymjqxq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jglfoiwb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cqsmnfhq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3rjwxkwlq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kkzmfzmp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3axydibdh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qnadbpbk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lumooher.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mnhwcmin.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ymjfeein.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3axijuciw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kysxktci.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dbmfyker.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bglehhka.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3gjxdryqy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jhtnrumk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wlkftjqt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vbvuadtw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ezceqgsw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3acpvgnnw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3tfzsjwyx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3uqfsmchf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3bhuajxwv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3icckpzyk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lboljqzi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ykjxkoxk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tvjbwoln.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kpppdcmt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3wcnyzzuy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bvixxesc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ytbwyqdo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3daihywwi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rvglkrqy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cxsrrjnk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3olqplpec.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtdysef.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3emxihyfq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mxqysazk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqaqjkyt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3olaqyaau.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ytzakcgq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ltvzhglu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hlzoecgb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gakwkbby.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3khhvixjf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nmveeplj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rrytjmmh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xopfhaig.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nwpylniu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xpvyeikm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3yyumxmrb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3soyrqbob.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3eayrozbm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xuzdxhvz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pnljssmm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gicjbuaq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3clgcsmmd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3lcjokwvq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vcltlugc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rwdsqwuj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3umzsmflh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lnvithwp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yiwkpiaz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fbrfhzqu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3iidvyjhp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mdagvndl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3aeqmyxea.html


<!-- 参考信息 -->