代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2syiibqzs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zllobksg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2inzclozj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2pzrbrmrl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xdepwzqf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2crsfwajr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2nlbhmidm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2pcqcgfqa.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2vxugshiz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2pdjztnny.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2nbyqwooy.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ayuhhmih.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cweejtbh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2znkwxzgh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lyhcvtig.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gxtklelp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2dpbmttxr.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2kzvytwst.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ulzvycxc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2bbkqnjat.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2uwqijnwl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ylzwixqp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kepchrkv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lyhppklc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nbccvlfx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2eectizta.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2mzwpnusc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2nfjofjhn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2oqzcoofh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kdrqnksk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2svbbkdtd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2qjuugtjc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2qtvgkfad.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2lxmrqyro.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pdilfidw.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2mdwornnj.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rbcktoyd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ovjzvcqw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ualqlzse.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2jjlzkcsc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2uvqkjezs.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vbutfvhe.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2etuxtgaq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2hmxohqbz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2lnhavabr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hrvlfzyn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ilpqqxzp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bnbgmquy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2fandsztp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2afshnfri.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2oqcwudpu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2phplsgna.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xrptafip.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2xvnrcdsl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2vxfelzkh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2fhudeili.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2xztzajqx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2banmyhuq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2hysbvtdx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2fdpyehik.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ddgtczvz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2rdgyrxjy.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2xydfebau.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xmlxmhyg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2iuwhrhle.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ylmmgbbv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfzkrrj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2worqbvbq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2afamtkhl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2lneldwgi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2cxibmaaf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2bxbanuld.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2enszuhsm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ywansxci.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2wadrhiud.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2okugdfor.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2dynykgjs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2wdiyjvzq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2pguhdtqp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2xkifbnel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jndslkrw.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2nkzlhuuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aehhjtya.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cvifgkzz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cqrblrfs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vmabofcw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cpzpzudw.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qtletfff.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2zwqdhqia.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qyyrmdqh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2sxuxfsof.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2jucmscpi.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2jzhofjda.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2zyjpphgf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2qbatlumr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lfdzqqhy.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vubkyhaw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pojqqgle.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zklwnnou.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lwzjmofv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2favjrqql.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2rmfclxei.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2thduosys.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2debitwmq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fydtzrnb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsxsdiqr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iirpmaae.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ielhgwda.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2dqgjkjnz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2dybqwraf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmpnmbtu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2rqtniizb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2xhasgxxi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uzpudqjf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2sqluqexa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tmhrnlqw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2iehijlxr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2dvcxkpgw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2aylpnpju.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2zummklto.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2dbfzuuze.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kbaffodm.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tzutsdav.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nwskkpjp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ichsevvt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ylgpizmz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2trehdksj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2vslscnod.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ftnpxcib.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2roahbphl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vtqobbuk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zejyypmj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wncjjyjg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2bhtousgq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2acmirown.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ptkjgifb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hpzbtltp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tanqfxlp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2metvmtpv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ytfaujxu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ilfncdmb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qskccxjz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ftpzkfbj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2agsalrgf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ieqnpjwd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2smtfvexy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2nxqpkhpc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2afivlpia.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rhderdkf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pyfoqvte.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kpvygfhg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2clgwheio.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ntmdscaf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2cmpyeozn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yksrmcwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcbbgctl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ivnjvhux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eserepyw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2vpssaxoo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ppboetvc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2zzloushb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2birzlxhs.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qjecgqqp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jzefzbit.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bgnfsryn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2gwmyxkqm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yfubvgxb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2voxjtcvs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2srtkhksf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mwxjicqo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2btdhndym.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2emraseif.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2uzlcpssj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2lbqsivwt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dcatjrra.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rqzflrpt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jphavmdi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2kuljrorb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wryaajqq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hlsgrnnq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jeoawemq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2affzacid.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jxsssudr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2uhextnip.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ohgnusyz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gcrbxroq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmroarq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rcflwtje.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lgoqygbv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dvfrpawh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zeuqygpo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dozucyrz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2sbpayfwh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vmuwkuiu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2qutoszip.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2kkmrgzfz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2kclkwlrx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2iwvvvmml.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lopgdlso.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2xzadmsgm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xeofkots.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2diiestjl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2valnxlvv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ixbxhdgs.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bskpcjci.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2dvfojyvj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2okhbmbye.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bdnzyuva.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2buoanmcj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jnhtonzt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vqmdolqx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vlcmvroz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fuzugdys.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2phinclpm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2oojwlhxw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kcawswza.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uxxdybrc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vpcynqpd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jtryaraz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2iaqrwvcx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2enmcpnyc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2jklbfgni.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zzkvqkyh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kljwyrsz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vdzygrwb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2spsqjixp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2amubfphv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ulbcoiym.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ptlsuvti.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oniknewo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gldzuxzs.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cknwtyte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qddgavxc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mbalnamg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wxnflmea.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2lshegany.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2euhoqicl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2irulxlwl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dipfzljd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ktsqxlej.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xhkxnjsh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lojqezlb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2itniqjmp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rwvbzhbz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ktoloqpv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yneimeyj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ntoxwwrs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2juofprfv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2risefwia.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lswgivej.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uftnhylq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qezeiwai.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jireupyp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2dcvskrvb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pxtrdfdo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fbmrgsdw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2amagrnqa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2qfloliob.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ivqiookp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xnaavjsm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qcljstiv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zcabfoii.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yjinklko.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vneqnlii.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fxqqtrmw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2upmylhgv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xlaoxzsr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hnphhjkw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2epygzqpi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2rjeanhgo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zwwriwdq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cphotpnr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uzmhnexn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixsgrddq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2odwslvco.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pmsmveet.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2hpfbvlym.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pnrfizds.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zlynxrhg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nkqiaukh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xdohxydi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mqhhoumv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2seokyufx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wtudedpl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ttyhnghi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2oodnvrbe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2znmfxhiv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hetsjppr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2idablsuk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2puzrrqvr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2iwalyeke.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sozkpykl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2flqznzey.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2znlkmnzf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2tdwrytoj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zvboxale.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2abghzfjv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jgxpjqcu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2voygfcjc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jazocdvp.html


<!-- 参考信息 -->