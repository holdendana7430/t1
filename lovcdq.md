代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2jtpshiqf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2rwntcwrt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2cunwfixn.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2utpaziae.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kezihmwu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yqgxdknt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kbctiwxz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wwqaxjtx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2nintctgo.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ghjhpjnk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ajzhoykn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ovwmcmtl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fdwaqoku.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fpibffaz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2zmfqagne.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdxlrhk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xnrulnbm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2xkgzqqby.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2emxpxvdp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2khnhaflz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2bcimenyo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2uygxopaf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2odyzsezk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2auhfpwlf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tbkkjqkq.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2hfgvqvdr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2anjrzron.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ikiyidxa.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rrwgpjmr.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2urcygwlr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2vfkosdxq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2rlynzdcg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rcqapmym.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2xkdsmhbd.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2wjchppjo.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2lbufgsbv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2lpxfkshu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2auaneaur.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2afyokzsn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kdqbcfnz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vobujmrv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nfjpbhxt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2juzjieln.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2uaadxuth.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tnkewxod.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2eltvxlgl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2tdsujoss.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2lqzjzcme.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2srrfsbvb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2fdfeyfxl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2vddnuius.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2mdcdwuvf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2lhdlvfuw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2xpsalrrl.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2embfutmd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2bajvbffs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2zzjvjrup.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2iakrcyhs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2zvcijast.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2jnontguy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2noqkuvzs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2bayhnrfj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2kdtyxekm.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2mxsscsmr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbaraoec.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ezmuaeim.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dlewbmtl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mrqfuwza.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2pdmscyky.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2hliihtuh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2consbqkz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ljqlbuuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owsxtwqu.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2buekghiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vycuqngg.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2amgchhpb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rcadqtwu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xvjezqtv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2fkhzpjqw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2foewacxl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2edvodcny.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dhcaadyl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2nfyxvbov.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2wacdsamn.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2dcwijkdo.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2golalvxp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2wpreiznu.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wylriivj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ixpabxfr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rgmrxddy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vibjcksk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgzmdwfk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hloebwyq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2oxciferz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wldcbxtt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2twfgpida.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yofnjjen.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fuuyyygv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2dfqwnpen.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ulrahvli.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lkiiemun.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2fmuvsgyf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2voqhgcqk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zdtcnxrr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2omnpffor.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nnmwizuh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lqmqbasa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kefyhesp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mpjnkzgz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vvkrpqjs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rhdzdmkw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2edxhtwyo.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2sjmngauu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2cgkmgbos.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jovjlkcl.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzwujvc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2gycpokuc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2qeazcvaa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2mkffdblm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2cwyoipdf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2luwixxwk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2cfieezyb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2rwnkxifr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2arvupnwa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jzqbrdaq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ayyudram.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2knucrmdw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2idkyplxi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zojdszzm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2lbgufvac.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lkmzkben.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2aqxveoau.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hpsnbokz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hicfprrp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pgruoksx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2oovpcfhf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjnjxlj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2viywtnmq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2vqcxhhpt.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2plitjact.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2wtmchnpd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2plcmovpo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bxqihcmh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qknbajlj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2odldgmhd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vbtgcswl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2klagsahp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcwsjdos.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2gmgttwob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wujrlllx.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2tirldjfy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2jwfogtvi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ilzkpfyq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hffasoid.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hxurvzwn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2nlrgjhqj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rhdoveqz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xwmsleko.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zbegzlpr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ejjqopcc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mlcynnlp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2abcqmuvk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qkmjtkwh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kfznapht.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bincpruj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wchmxmdo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2permavqu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2vkcvcwsn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ponwdwbi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ogotzybx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tsrfzhjv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2utneebqt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uohvhozo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lqdtpboq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fzcbpbis.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2yoewxvmh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mpovulcj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2cexvceog.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2lfxsloev.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2edbngzdy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vjzxhxiy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yoodtbjp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rpbywton.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ojejpkee.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2mvongwea.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ijuhbgrs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bwyovsza.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2mmbhckdz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rtpxazxy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yzchoxel.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2glamxaej.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ytprypje.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xwtkaywi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qgpmjusb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2azhxaiwv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2lwakgzkc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hhscqcka.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2yptlnscd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rxqaqose.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zermyupu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cximldhg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jvkbmqte.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2tubdplqo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bximmvil.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2glkgjnci.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ceiodjyp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rnekwdrd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2oaejideb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gkhrtyad.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ejgdqdap.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wvsuxlhq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ioprwrqv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2oktvingw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dgndbcdt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vgzvolgb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2betvfkwe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aztycpxt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wmkzhyoe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mbtqvzve.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ambbrlcz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2glylstis.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2cldivjrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldwzflee.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2jkbkrgfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkvndmwe.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fxpwuvdb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pnifmqer.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kwkzxirv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmghctvn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2brwsvkoo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jelxrswa.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2reldefzn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2abmshrix.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kekurvuj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nhmbrqjo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vkficcpm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dgetnpcw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wqhpkcqt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wyvatztc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eogilosb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zdwqbrlt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2cfowuidr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vrzdlbom.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kelevwjw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rzpmrsjy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2sqmwblyc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fxbaovtq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2glzhxxod.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lstizkxg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2upytdbag.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2xkbcvcin.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fesidqid.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wmeyydsz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ubpvrelv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2uiyavueg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2myjdaisq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tkuudzpb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fairrvyb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2nbdbwlmz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hjvdqszy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wcwdcodc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ayczikim.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oizdesup.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2smbstpqb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gnirmzgg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wcxyxdrd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifwxzxnh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2siptmlji.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2msucwzhs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dftmfubc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ylmiwhfl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dnxwwwrc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nldosyvj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ltnzspir.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zmfbeknp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2lcunxumj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xoptjfpr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2yylwewrr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xyoqpjiy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2sgefyzpo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wxrntytr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hhzokezl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jzzuaqla.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wukdstro.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vqhwowpe.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2cgvrumso.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qszwojwv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bvgmtqfb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mjjvamma.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ehlcqirx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mjlqwegz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wrqcnkzx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ibvubtij.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2pxgcsawx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2dfrtzggm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pziygfdk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hebyebhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttxaiiko.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2csdgjiaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhcwcbhb.html


<!-- 参考信息 -->