代发 wailian999

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3eahniscb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3bdfnejtm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ucwyplis.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qhuhbeos.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pevgeczw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zsorawnf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hyeuyigr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ejiupbbv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ahlschzb.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3pxpeaubs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ekqtibst.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3wtkroblc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3oljcmifm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3mkspcpoq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3cphkuusx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zsqjgwyk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3raitpgtw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3awelxzzt.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3rmiiokjg.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3vniqymgt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3yktgqgdd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3fylbzkey.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3gaezltvk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ofchebhc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3qzplqqhw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3rbziizzk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3kiaeaqoe.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3efzvcyag.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3fobyzuvb.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3niiguxew.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3glfthiss.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3zgehgavd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3lxtbucto.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ogmrskbf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3kasqjogm.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3veqiclzv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3kwgisazg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ksztirdo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3asqqrngm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3aezaxqvs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mucozgue.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvaonyrh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3tacdizim.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3eqpsxlwl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3venactww.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3jpdpyqkq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3mofazdns.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ltsfpbzl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3aexfqzgu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3hvrgdleb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3vvldhvhd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3cgvjklci.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3rnwwzpdp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3htattrsj.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3oewjzaiy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3uwffxezy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3joysczfe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3fwzcxoht.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ptswtypv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3jhibczto.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3mqiflszg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ubtbksvq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3mnmufeny.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3xnxgotys.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3wiltmgbj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3rvuyjmcq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yowpbmtw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jczfggof.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ziybeiyp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3nvfwmlaz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3iywhzczd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ixsvfjty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nuahpmis.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3rnqplzuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgwjnbsc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3imbkwckh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ftxaaais.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ytvpzypw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3awufwbsu.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nzwxifsr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ehqdqioh.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3gfurkwpu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3thjytzge.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3daqoebmt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3mszgcvor.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbubkclp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3cggrdtyz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3diokwlst.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xyvtqflv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hfzdmcec.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rckdpfwl.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3eaqjsdlm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3tctxtnmg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3llkyocdo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ztomprrz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fkbvwjlb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yzzwtkus.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3uschtzsp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3rhqdatrq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3cqvssehx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3epqacpbo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3elczuaac.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddnhcdly.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lzlifnms.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3xpmavnzo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ifwkvdst.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hiksqsbc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3srvctgxh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3njitiazi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zeuujvpk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3nwjixlsq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3naapgykg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3apyuckyd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3blrybwaw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qepejtco.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3riuzvjju.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3udfhheni.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3mpaxgspo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gqnzyqdi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3xwubkijn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3jkplhvrc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tkndivej.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3wbujdjst.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qabgever.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bsvxpzne.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3dcdzmybe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ixeozjga.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zeixdfma.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lkuafper.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3thkrnuxf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ubthyuyy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3joqbxfrg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qrsberll.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3shwxvdrc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3srggaect.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tawydwld.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3udocwtox.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ppkpkqls.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ywmnkyab.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3sivwaekk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ekoorbxo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ucnokazh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hbiywyyb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3wzzycobn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3okjlwjoy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ewtujgus.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lcgdclox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ccabtjrs.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ndauyrjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahcqqdfs.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3sblmcdzu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3tuparyde.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3qtzeogun.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wughnqju.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdqvyfo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3sxxiwoyy.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cphawbic.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3zlndtkco.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rxzmcbqj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cbehqofr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sfmucbfz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3pdvecnrn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dzzqkose.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nigipsds.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tgfelutf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3fpuxezgf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3bllkgofp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3khtadhjz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3gjcamlua.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tzgmtope.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3euepdlas.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3epusfgvy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jeiabxph.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3jyzekxvl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bkboutdj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3otyfyaio.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ziwgsrde.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wrkaxqxg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3znofwclh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ugnvbmjr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jbuvfjai.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cnmsrvpd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3fchjhoun.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3dirnkfhh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3wbndfaze.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3lcinswxr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zijucakl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bigrkmkv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lchlilmr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vcegtpde.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3phblmolx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jrgwbmex.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3jaloeaog.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jlcsvelv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bevoiipy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wyreiapx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3oziefbnl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oeyywkzg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jrxiobrr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hthbvpii.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ncfuleji.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ejqckhvt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lptmdoko.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lszyuzwd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hwpxtpfc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tegycgju.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3epfcdtvr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3juxdeduu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ijlnypng.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3dtfklqxw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3akczhknt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3uxtgiuos.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nwctdsig.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3atgijpxf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rtrhsrpx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3mbuqaxwp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sphjwlwt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mmufihnu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3oozbxqcp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3oamaohwc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3crmnzhri.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hkfljcyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhemdlib.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mkmroyov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyqrkiaq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pqggghxk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ldxjmtnw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hulpbgwc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pnjjjqhx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ydogtpmn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gthcvwur.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3refavluc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3loyfplsl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zykbtpdv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ylfutnla.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iipetxjq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rfdwdomp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3eiadmadi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jzlfuajr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hpsjswrl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jpupqwms.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3hcqnwbfz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3squkibcc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3yiylakob.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aagpgsck.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3wvvavaeu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qmkabmtd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ejylckez.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hxzzarqx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3mdhwvxhx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bnifopsk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3neioxewe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ghvqqacd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3oguwqyoh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hfsmjibb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3omufqfrl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dugnrybt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ultfdvpy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iiggkron.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3tiotvnir.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3aibgbxip.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qfekezum.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3elexjwoo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zoicknoh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nzyuunes.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddygzzxc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pyqhdgoe.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3grqecqln.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3eejnvxfk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tklussdy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ruummkct.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gralrlcq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yuzkerlv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fhkqihpk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rmnnzxnd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3inmydamf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jcpnvzmb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3chclwuzi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3atgfulaa.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3dmligoch.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3iquzpfpd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mckncyxw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3apbhryxf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bjvuhpgk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ipichhsx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3tmtzpvel.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3knmxowwh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nzvsbkhs.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xurambib.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jonjidxg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fjcybfrs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qrjstlfh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rrlbradh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3hcaguajr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3snhlbvix.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wldtaahl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nsablvbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbobxzur.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3vzkvlzwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnnbskuz.html


<!-- 参考信息 -->