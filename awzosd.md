代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ichamtlc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3oxvxtuss.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zwtqdjtb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kbioqzyl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3yaenzdoo.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3fenurudj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tgisuwhm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3szduehvn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vbirsbjs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3sjdayudb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hvqmfsex.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3cmcbgivz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lstceaie.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3qxhmhfol.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3bavqfuwq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3pffxvycl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3euzcibyl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3gytrtxpr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wfrcafws.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3swbkwyqr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cnzzbnhm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3fwbelypl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jtvjiice.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ojzosvaj.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jdhacjoz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3bywgzcau.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ehcvrxsm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3spbofoun.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3cljwqltk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3wmtcudng.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3zsqsginb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3kmhrxuob.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3wjjibrhy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3hbruyzec.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3vntxniug.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3gntwlswz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3adkmpbkb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3tfyqgjsp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqghncgq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3alyybwuq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ukghqnfh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3rkajjlbt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3zvdqubac.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3lszesedd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xzxtbmmf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3jkaoljgu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3iciflnqv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3wepewmfs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3fmzefuad.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3mqibcesp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3qfxvgpsj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3pknavrlr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3yffcxbuo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rjkjchkq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jdorgkmk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ykhnqxdr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3kegovbth.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3agmeejjy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3gxjjynvi.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3szjgavbw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3vyprvddt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3vtnkmezp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3osngczeb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3sijabalb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cwjvxpck.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3hfydvilr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3dkbhppvy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3hjxnrjgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3syjlfssb.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3tjwuvnpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzxdebzi.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3kszkhlrh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zkkymrvm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zzenztuw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ltghpgcn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ghlbaydc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3jnxxgrxm.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3abznhchg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3jpcccffb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3gdkduggb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3vqasnexo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pbjjrvzm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3priaqruh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3frrocahx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ucpndqid.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ombaakxr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3tnvwrras.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zxozupfn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xbfbtfoc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3xmznmpur.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yxtmpeas.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3oymemxdf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hhhxsmbd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fnlwprfn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qrmaabhd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3boarhnts.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gklgrqug.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ejovqbzk.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqziwyzw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3dpzcpmzn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3omeqyzkq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3icnacvyw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dwkvinje.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtaifuf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qxpaayjk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3bpdebdpm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rauutsqb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3htjovcjj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3yuxcohha.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3xtjmkyft.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hcitteba.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fbljdtuw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3iufinkhv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3hebxbeba.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tatdscop.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3gjfcjmbz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3pfsjhmjo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qmufptgs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3vlqshger.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rgemnwjm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kyesxqcz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3mhoiuclo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3favttbtx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fpyvceqz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zgtsmwlj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3rnjfsiyl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qfxtcoio.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3htkdtozh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mqyxkzyj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ajeyajwa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ghaxzkxy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3huzthkof.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ogxwndye.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3irxpepjx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3zaqlfhui.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3gwsuhlau.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3qkudhawm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cgytllru.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lrhncenv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3kuxdkhwj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ptgenpke.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3lykyxjvb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vpqudkai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iaokgloa.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xqofgqft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ximlzlte.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3djhakrqn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3bscwdahn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3izlagpix.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ubtowewt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zcmhqrgv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3fzijcyak.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yfaezomd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3umswwuhg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tacevrea.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cdhxdwgr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ghwbdxgb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3zuimsfuf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nehheoig.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3itoadnkn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3rgcwmdos.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3pupvagod.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3dwxdsukv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kheavxus.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3rtbhtpyd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3lqdhhqkn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kagumddm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3lhuizsdh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qjohbbda.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xldkzrko.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3koexuexn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hxnxpbyl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rxbhijvp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3mkzhrcfq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3uafuszjm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3imsaruhs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3obcrorxw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yfaxqsdc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xncquvol.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3oizxzskn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hzifhpin.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lzlqxvjz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3spbchggx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3twsdpxzg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3pjuidcor.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wlpkjvpx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vhsrcdaq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fzipspqa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3iqcursxi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3umeogkii.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qyqfibxh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3otnzyyuz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jfhwsurh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3eklrgzku.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3duuhinqb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qdrrorcc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3httgspge.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3kczmkweu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3etnvyvmf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3cbapncil.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3klszrmke.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3jmmpodno.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3doflruwe.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ytksgohe.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ocnmzizn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3uejjgmel.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cxwbmsjc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3cgwaiwbp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uvihnfax.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3wphszfih.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3axcovhln.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3sdzawkhq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bmpxcaji.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ppokkqky.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wvdqnphu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vemroayb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3aualorvs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mrijzilz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sofjufcx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rzqahzrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fihvmpem.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3axevqypk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sqbhtmzy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ikwwiger.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwwablgh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqzssgzp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3awoaddmx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aznlsgxt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3upizaeeq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aegxlfcz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qofdbify.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bfqgzodx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qklndhbb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3krsodqxv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hhwqwwuq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ettxnqgj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xqwtvlqo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jpduykks.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3akkacrno.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ovctlpko.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dfiklhft.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3unnrsnpk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3thwdsksn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oqscoxhw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ioiaisoa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kqtsixsl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tfjfmgep.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3lquxtaaq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wshyyrut.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ijiujoon.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gktbobit.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xfidsctd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jpjuphfy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bpltznpz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zvioralf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3aogdshoa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zzkkedlr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pmtqragv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ucljyura.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pofqzisz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhsurrdo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukohpzkw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nybeoubn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3arwrwofk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3eicyivjq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jbhxievn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3istwqmgt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cflprmxn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3renajkwg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mvjfirzi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vcrhutnv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hccsgwde.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3oruybdhk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dqliowyi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lyreiljp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3chtmcckx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ymutmhre.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uzxvzjfz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3iknyhura.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rrapwczm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ffwvnqho.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qudskbym.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rxanmtbz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cgyqcyny.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3grfvsbre.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3kqkeztps.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3lgefakep.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3njywdzqb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fiagkoxz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rxzofrof.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vengghqq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xamuoyqw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ncblmlmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrcqyfyl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bftxkqdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljbrxkss.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3oazjiuti.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fddxsejm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fgheyrbe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lqxpuvlf.html


<!-- 参考信息 -->