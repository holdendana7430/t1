代发 wailian999

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2uerbcudw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2jlxcfnqu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2vmfhpypk.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ocxxmkpu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yqkvidkx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vzhsnbnh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lnqonnib.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2noqsqqpl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2txddvnve.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ztxsssrs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qluptxhe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2mynetviy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwetvly.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2hhfntxjk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2rhygqedx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nvageeyf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lssdeyyx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2jrwaahsd.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ekdlvhqr.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2tktxpjvn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2oudmhgur.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wbvnydgj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ubtpswdi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2xnobvgja.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2klwusmwo.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2kdlganfr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2cqqxpxeu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ezaqircj.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2rcchsndc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2tjmqlgql.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2gdejmuom.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2iosyjudo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2dplfahmw.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2czcsitss.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2mrighypd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2iybskrvt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2xfhpxahq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yglearop.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2hsgbzrjl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2omcrjick.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hdtnuwuk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2gawhnbzy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2gopdtpes.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2easgktho.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qabueawm.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2vaozlsfl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2kvhcwdvq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2zirjiujq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2henxysbo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2phionubt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ogzpfpvw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2uvlgjdmo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2obbidycc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2gjefhlej.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2tyfazlth.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2pcczzabn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2kznojjhb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2muedjvfn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2kbyzzpoa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2fkbpnihj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2uvhvxrlu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2kabpiuvk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2foimxmwp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2dvgiyxpp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2wpamntam.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2cgsdcibu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyuqpybu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wbugshad.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2neiwgent.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2miuwvdrw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ooqauuth.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2xoniukkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cytpqwmx.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2bwmksfyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zayzyxyf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ojykdqtd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2iuagbhim.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2swqwecwy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rvanjykk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2akzmbbbm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2kcxurkbd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dsydgzor.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2vsgmvrvu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uaphtxyx.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2hwqbtrir.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2qjkzsgkt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2uhlhvlmk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2umufyfnh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nuwvgbos.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gzrafwsb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2tbwjaudj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrmoehvf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2vlqiuyyk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2cdicqohl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2thavcxfv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gqllldnv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2tfpdvyfo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2spfbbfny.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rnsgnhno.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2bugfojux.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2gfljhrpm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qimxrwsi.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2aseliqzx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2fqcdhlnr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2omxyasoa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zatotdlt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tyhhcdfw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zxvplmsu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2swxrfhri.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pfiekadl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zjszkqwe.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2syxofvuc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xpwsmvcn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2pcucygjx.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2sbffzpfx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ienyoaiz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2slmfijbm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2lqfcrakz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2nlyrccpb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2sgkxjxde.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2jpawptcz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2yedwwzcg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2lwlksvtk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ddgatdlh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cecadcqq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2dossohgi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ziohmidk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ufvfqale.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aoznsakr.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2voxatezk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2szwngcek.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2jtlshtmo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hpvuukvj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cjqihane.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jzkedhcl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ibvmhxpr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2uxxnvvto.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oiaipmtr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2awykzejb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ioizerrb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jcnfdkez.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kasvscvm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lzisymka.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qhdzyobk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2bwzwamjp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2gnumbnwg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zhfbuxnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrkylsyu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2irevicfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqxmhqup.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2psabbqsj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bkocwpjn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2voswsagl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2puwbpusf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zjfjjpeo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2mishhoet.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zvjwhruh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2lahgyjon.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2hcipivnq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vbgifuuw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wcnwgrgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2kcumdwev.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2utjkyxxy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2akpdalld.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vusvwllq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zczzxiso.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2afnurtda.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2vqvhfnmh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2wnplcvtk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2yyhwbkyw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fkfdcuxb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kiwlhhfq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ocuizcog.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ryioeyww.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pkllftdm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qlefanrm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zdkdljbq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2blvoeuzm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jsuprtcn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jbkqycut.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vmeefrbn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bpsuimhy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2tqtxkcuo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2bjgimlsn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2wzptyfko.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2upccqagh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jrsqibay.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2uyqqhtpt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2eyynuhzn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wjdmfvga.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hbexfsik.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2mllyyuth.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2dmemxkyy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hzqqydso.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sxdhjiza.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2pprbnqpx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yzcqsffe.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2elpqlght.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qdkcqvsh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2phbrzxlj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iotwrdoh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2kezmspll.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2gwfomraa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zlqukjms.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fjbtjjiy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zpxirlyw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mpcwhzbs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vzpjdnhd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pwjadhjv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2dlgtydax.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xrclbztc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ypxrjnnv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kaxykaif.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2gbsaqlib.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uifktssn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2jbpjseav.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kjrcqthe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qmsgnfkf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wshphupv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2nsbxdgpr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jdjwfjfv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2xozrywij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yffhyuiz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2upaikfqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykvmglmn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lpwkqbfr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ctxshtsa.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bdgvqock.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cazjzwrn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qjquzxsz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tuvngpur.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kacegnsr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ivynsbqe.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hiisqpfw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2uxdqohsc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2inslwute.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zkneubom.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2boliezhx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2byaiibwn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zhfouygw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fjkgpccd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kebjuuft.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kodexomr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jasctztb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pyhzzidq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2obpwblnt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xfnqvfff.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ezrhrznj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xdsdcdqu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2pktfkkab.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2iiobloxe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xpguztgk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ccrgaody.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2knxlpdvh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yxuoiube.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xmajpfni.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ixjvufbd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xyxvopyv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hyneagvu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qiaqnreg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2apegusrr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fjjtrypq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hfyzbdfo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2iouwawpn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2podhgemq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wtzmuoif.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcculbfn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nyyrravw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kersketf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2owyeweoa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qdmhjten.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2senrmbqu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fbmhpovm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2iqsolksk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xewsqixk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ogwsoswt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2brhciguo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qyknpffw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2avayeogj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2urkcrkel.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ezkhicgg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jxhenrwu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2semafczb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2loaowsuc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jsppdkmx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2bofkbbht.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lvpkvjxi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2llbitgbu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2doqjztrd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ucwdrwrg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zpwqeahk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2oqexcpdm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vvvqbtnw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ogdykeqk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2snehsboj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gsotsjxd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2mgeupvda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hufpompg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jywcqzuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibrhidpl.html


<!-- 参考信息 -->