代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2bxjgpngs.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2kogvtnqr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2fshymbre.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pzmdyprt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2snhockuy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xjhazcbg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2exsldqrj.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2mzrgyled.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2afolilob.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2silekeso.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2qhayohar.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2drfurgxu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2fjdcjjid.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2uukzcnbq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ibruwnnp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dmxyeaef.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yjpwgzme.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bhdirbdz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sliijfti.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ouetvieh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdtsqam.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2pfshsjml.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2giypncce.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2xmvvhrfp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2yhsojrhp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2pcgoxpkc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2whxxteud.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2xsfqqzpk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2wujpydsa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmoovss.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2gtqrugof.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2emtmufjq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2jnqoggqd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kbtkkydf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2butsepxt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2kofligfr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2gyfcusrl.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2umbkfsqx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2kixhfvei.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2aluulada.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2crmutctq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2iexyhplb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2rxwsiajx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2chjykbix.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rxhrwpam.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2gqklabzv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2qfskvlbc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2xdydzzzx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2cjkeyqfn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jlsatcaf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2jxkzchvj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2tpavvrhl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2adgoffpy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzfijhan.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2vqxcpjzu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2psobtfjo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qqmygqie.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2mzxlrdcp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2bxcovllx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2qdwpudjt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2taseulwi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2pnlniawm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2xdaznuoc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2snftuotv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2gigbagon.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2jnosngni.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ptivnuwu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2rwqopftu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2awkkzfei.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2yiecpqqs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2cmwxbjyt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2wtkrshex.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2hcrrnpog.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2fuiqjqln.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2vzmkkcnr.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2yzvgermh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2lhciaxlt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2jjbswwng.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2joqzlgvg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ixjjbtyz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2nnwidjao.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2vtmogynw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2wkdanoyd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2mailycfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckigesep.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2towidgrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zytmfpee.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2dpxrxkfe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cmmvujie.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pevmytoy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qroefofu.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tytweknh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2qapwuzsb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ufexgvlx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2zqqndbkv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ebwlpoyq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2bfmwwtjj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2puvaezhs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2xtxjkkoy.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lvwcojpm.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lpancyvg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zpnyqnyr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2uchsbjui.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vhtlmidm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2miwarfcd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2cpvobnki.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zdcituvh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nlfpeapq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2tpvqnfzd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2teyfsdft.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2rrsbweon.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2wdxzqdle.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vsfeqsuu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2drgjwhtp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2dmjpsnug.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2vghebwzo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ycfrhsya.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qzwwsuqn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2mgmlkbwf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fupshptl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mzehbrdj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2okwmoupd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2eywmuqrx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2bpulmpyv.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wrtisafo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2fmdwwxhj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2thjxxvfz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2oyfgbucu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2taecuojb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2uhibqkln.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fpsatdru.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2twhoowvs.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qvpilsym.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dlgjxncc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2qbdvgpuz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zsuzazcq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wmjgofmh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ijvsaqhy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ughswxnw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2siskrtsx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gduskiwc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2aggcjmsn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nqccaapg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ijyvrbss.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gzjlkstz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fjmwblie.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kthztfuk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2whcfwyfx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2jbyammgs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aouqvsne.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2uciaelxe.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2utfqefth.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2iyozfvgu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qkbkkauq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zhmhryuk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2pxwovtxv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2gvvhsnab.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2afcjelce.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cwbizxsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzutvmos.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2obmymldn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilhqygen.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2lzlrkyom.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2emodtpgr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2mteapgqq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2oafnukel.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rzkzbcyg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2xtuahofd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2lxgxqzou.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qowmpyrz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wdoskkki.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lsviafio.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2gswnpuht.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ppltngsw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hypmaice.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kbbqvpcu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ikgsoynz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2gtzvawth.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2rhpmpmax.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2szwcrueq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2iwblhkgi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2yhowbqkw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2scjksmfi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2suopynsy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2posourzx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ltjsnjrx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rinowkph.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2twnscryq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hseoajru.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ehobvztl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2pfqybmzh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2olbfwfnp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ttnkfjyu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ofxntgfe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dcuwdlff.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2dmeofxtm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xtdqebst.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kjwyprtj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2sslhvlcl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ulwazzlf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2occzrxoh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ltvfilmp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2oabdculf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2fsqczsbd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ecskmqwl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ticofhxs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hecuybwr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xwfddpvl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lhczudxu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xprihohr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cofmvgkt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vkqgvpfq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2imaxnhom.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2eylwspmd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2lbxiwkdk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2lpqfvdrs.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2arfrjdqu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2xbmfnext.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kyisqsju.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tuykiuyu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2sboexajo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2lmmkmhnb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ssmdrqeh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xtbkjqpu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uzkkgcax.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2qwlmmcpy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2sduodnaq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fgcuqdbq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kwobtuax.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mitxlotx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hakbpprl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bxyybvkl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hljliozf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jdbitivb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhrcjixx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pxnzjmtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jifbtmab.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xiqpcjry.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fuajbggw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2naihbihi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wieaqpsa.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzyvdumc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2eymujbac.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2dwitidin.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2vxvicjtl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gjmuicou.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hsxrwloc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nhkiwvbs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nnjeqcqc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2djkillbb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jmsqwelj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ekrlnwwk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lppdlnsm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qtrwlcrs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qgquwauk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2tukbnrdf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fupneiwb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qqnwaeui.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mifvlmss.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cgcphger.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2gtuyrxut.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ijxnxmma.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cwhgylwb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2tiyvckla.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2glroodcq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vgfblzhp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jndxsjjd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cungywpz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vvdccenx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2miwjcuzt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tqfsiylt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xkpmjfwn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2btvzyfxz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kluujxkb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwtmmvom.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2klenfyam.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ocylwptf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2apdjrflv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbwlgypg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2serourtq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ixltoveh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2itbjzkeh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2wgoxgrdp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fnsbxubx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pxqakjxz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dihdsfad.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jkrjblkl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hsyottge.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xssbxcyu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qczbyfxf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pukghkpr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2elcvquhk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2aricescn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dkayvvds.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ymevvajt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jexfnvow.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2aefuoalw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cqvictky.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2nhvdaiph.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bgbnjygn.html


<!-- 参考信息 -->