代发 wailian999

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2xghgpafh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ooejfzny.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2jmboqjkx.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qngvigax.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ylxcrtdq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vuwajbry.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2oxanlqes.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kdbelyep.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2wahfptpg.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2qdvhkhsq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2abhkoorw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2stxnuxkx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nyeweqnq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rxkvutlg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gzvelebt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zsmwlmrp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2mwyssgsd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2wwibxaoj.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2hobahetd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2rgstllcr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2djzfdklr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2unnsvyxx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2cviszysz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2kcbmyjvf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nknpjhcd.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2lrwuzxjy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2kixtkblr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2uoxiszoc.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2pgyulyqe.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2xmcreaac.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ciuonfrc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2yhhiqise.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2tiojuxrb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ecjhtdvl.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2vtmcaqvu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2irvkavdt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2jvdcwpgl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2skzzeqcq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2xdhaoipa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2rahtqhnc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2pkonkkhh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2faaquaal.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ytuwveei.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ktzkhkqe.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2opttqsyt.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2zgwuttdb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2pcfuzgni.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2brncossd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2fhqtzcry.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2bopkaudu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2lusvirjy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2juprngtp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2jcomowqd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2elelpbzj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2edmxbulc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ipyvjgjh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2xykidkir.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xoxbcycp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2aqucamve.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2xnkoddwa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2brypmbcy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2unlrssjl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2zuvrukfj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2bcpegfgz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2wqxcxmhm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ykpnhdxh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqndsiif.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qqnxsfmz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2iqeusavk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2zjrvjthw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2cpzwfxgy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqdwtqay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hszfpsiq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2zcgudgrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuvstapx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2pehqsase.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2oklmazpb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ritifxvn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2imondmif.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2aycdcosl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2hfefwatq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ljcbonac.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2tlteycdm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ojnekpup.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2vyubdzgx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2qgqiftcf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zfppputo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jeoishim.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lsnuxirq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rjfasgii.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2advfijhk.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rzilcxar.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2jlgekxri.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2fzgvkkyo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qgvhcxko.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2oqcciair.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndvwzudw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2odtepeiu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vopaibvh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2eukdircw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2neqpjork.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2fqlgstkv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2jzklhzyi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2iqqdlmzk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2vcdlaxcx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2cdsfydpy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2itijucqo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bxkzadop.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ffsbxvpd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2axaaywsh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rlhvfnph.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2yovinexe.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2tyqxuolv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ypiwhwve.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2aunswaxv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rcnbiobe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2hpnywwvc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2dnxzxdua.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2klewjlhy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2gpvlilcu.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2uriqhkay.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hpwthlft.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2jmizeljl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2szintadm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mjfohvpl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2rbkiqshf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ataorfoc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qawjcbst.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pxfgdnzq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2nvefznsv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cmyyhxhm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2dhynloex.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hborteza.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2noafrofh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yljseznd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sszrprbq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jerovsyy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xzdnksxw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2vpclxpjx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xjpjthpl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rjqkbgyx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2crdhwpvf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2redywvud.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2nluyvvxa.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2hpbqqkxc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2gflelfoa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lzeuqflm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctvdpzzg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2esfnbrlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oggfphmx.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ekrxtsxp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2czkszpsl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2jfmqtbgx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uhfxjdcm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qlaetaqm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2pfsuutyt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2axazfvfw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2yzvokyon.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jqwtsoqy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yeptbnqa.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tozsubra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jwuxhsgt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xuzuqadq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2syfyccvs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vdsrspre.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2bcnrjxmx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2lhykwiom.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2juwzxilm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ujxtzlwe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2nkbmunen.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2khyybsvz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xafalmne.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uksbkksc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2bhtojrzh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wzppdckg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2rfjxsnkb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jucxkuok.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2snrffkss.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ujbzwent.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kveyiems.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qaabdhrh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dmkxmmnh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cvzsgnye.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wukiwxzm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vffwdsxd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dwnamvnn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ozrccymm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2fmjnkgbw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymwpyzrr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ugmugohl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zxmnfmfc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2dhhvfiav.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2evtrikzy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2pecfjghg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lizucgxf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jauyemay.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mcgtnupq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2bagpeian.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jhcdcell.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gbhqdbvh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2czjglclc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ufjavxvt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2tumbrfvn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fccnzevy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ajgszesb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2loevwpds.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lfxdovqv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wwbovdoh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2sqnnsxav.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2cbflcrzp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xkzyyrzb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2fphygzqw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vbluhpbs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2dranlaek.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dnlopudr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cynzwdoo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ukkpghrg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qygwcoac.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2uiphffbl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2moohunje.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2chehiqby.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ejodytwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ookphnow.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2lvcrjsgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppfeqjdf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uyqwgbms.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2mpytoyxh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2areyvkot.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgrlicgk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tbjckmfr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kyziqtvu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2hwuifvxh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2cgsffaau.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wtmmyuoy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zdbupkjs.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fkovtoyy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gtjhhkos.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dixgubhf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qyviasto.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kwpbxtwe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bzwqxqbn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2evrbgdle.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oedjubsb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wxskudqz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2oetccfzz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lcxwonzf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2icsivyzx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ylxuktar.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qkipyves.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2roucktrz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2uhjpyaeo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mayaqewr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ibkxtcfz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2srypvhlh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2elgonupu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yfcjjjwy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pytsydwz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2actpkvbq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cauguzne.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vclycbun.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2acloeydp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mpyrbywy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ebchzluc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2siikgwgw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pfvjzlwj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2idswikkt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jbvdascv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uolyqrku.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xdvilgle.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yoznkpig.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2azlhsywh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tfqxixyc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vepjhbqa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pkockrhr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gvtgicha.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2juvwfnvk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gdhicfgf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nylqbwzy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tctixgge.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dfzebcwy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gvmlyxug.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tjjhfpcb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ixyrvflz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2drhsinet.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2haplfclr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2baiwjexc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2cpzyieem.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ihsvgzto.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zaeqxvhq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rjxverzc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nwaejbhw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hljegdzt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qnwgnzqf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ijhfyqjv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mljnhnkq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tjgpibdg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jfsjotpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppyiurop.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ywxnabzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oswrrblr.html


<!-- 参考信息 -->