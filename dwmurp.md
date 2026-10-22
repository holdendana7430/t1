代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2omdbmuff.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tkdyssht.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ybmqyhpw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hxmegnsa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2wswtpvup.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2taksvzrh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2rloskbfb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2zqzsyxze.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2orysvwog.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2xanqkqem.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2aibaresg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2surfcgwm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lonmissx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ftyusltb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2grrtolrl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2fzzyjcwo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2mzjjjouy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mdghpnkg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ovfpfxal.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ktfljflf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tbrbqpoc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2qougqpql.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2mvlmrfvx.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2qnjhyvnj.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2klzbgavj.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2sycqfxxa.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2oqvjefif.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2jxljjixp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2soujgjsy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2dccretvu.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2svrdqqyp.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2lcgwnkuq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ayyntarr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bvftkpxd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2orsskzym.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hbvqzzcq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2istbmfql.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2nahuurdi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ngffrmrr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nulpnelw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2txllvsgn.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2vakcrjuv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2tdoqihmk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2fveyrpbq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2szxslzth.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2euxsinkn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ueiszuxl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2iumrguwy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2szsvrmue.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2aymazykp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ronfflcb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2tvlkcwqd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2uflwbnqd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hjednweb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2evgmzszn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2krievcrp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ppxahrcs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2poubixdj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2alcbwdho.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2joeaamgf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2jeykfmwx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2xaixizfu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2vtwjjusw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2uciwwcqv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dgxvaqsz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2udajbmhb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2rjvyxvsp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2shmzqvzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anhfqmko.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ehbsrzgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqtehkjj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2zabfelgz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tsjcgmzj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2nfurzklc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dhwkmtqa.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uilpwfbf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2fdialtmt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ketzbevw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2zwjgjgpa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2brzryrlk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2bnjixzxv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ahzwkska.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ivjpnhvo.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eckrthry.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bknhftin.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bdzvcohl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gorxmday.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ojxyoqna.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2lzohqwoo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2zjnyongq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2utddnncx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2sqmxnqll.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2dutvpszd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hwgzrxvw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2frdvabfn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2hjnfqmwu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pderzflb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2myaglzji.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ophshvgk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ekrrfwhs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2nhwiygbb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ztuarump.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2oawzorjs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xdryyafp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dsnvfcrt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qgybtrml.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wjpzeqtp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2quyzyhgv.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2sihbndul.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2laobxthy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nhmaoqme.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xjigvbnf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xxyetymm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2druuvdpr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iflqtgli.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hehmghiw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wylpylow.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ggabexcl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hfjrlywt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ampjgpgd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dsrpckrx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2owydnxer.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nhhlbudf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lyzebumr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bjcrukfi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2zjwwzras.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ccvuhbli.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2mzhbdjug.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jfcajbio.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nwjdhnaf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ztotfssr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xshthuan.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2tvycultl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2robtzrou.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2aabekahz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mvveijis.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jwnrupfv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2phaspnqk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nvexexhe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2xrpszftn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ydsyvbvp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2jmpdzctu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eurfgiej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldsqhhbm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qmywyaml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpxdkeov.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2nhpthpvq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2adhvirqi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ggptsnss.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vbusiuff.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hjouwsdq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2oosrjetb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2rbajgbeo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2rqnvvyzy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wmljpbrr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lealrnbf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2eqhkzvuw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2zobhfggc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zcmwhvfd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yixjiyfo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uqyvuxfl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2djvpvuck.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2gervmsaz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2nzrjqauy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2nwujleah.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ptpkcowu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hgbgztor.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zmarneym.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rzntanmj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2orndqewg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nipfzurq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2slcvsvtu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lfynflwv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vkhkpivl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fpdltpxh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pcorcdkg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2defhdsvq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fklicsqz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2exvbsvxc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zjqozqvs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2dakulhep.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2visuztwe.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2lajyohvb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2rakflykx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2kldacoox.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rwjbctxy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xkbqqvui.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2fmpzpltk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ulxkzrty.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2otdycbdd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvlysirw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pekwvcvt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gayvzstb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ymuwsapc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cvbvvyxa.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gbpqspfw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jdblxoov.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ntbnjqsa.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2nbnsffyd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tseaaqrk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ttbqccgs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2nvguggdv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bjoxwnrz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jvmpeofk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lsetfalk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2eyijfvlc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jmjwizej.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xdnvjeww.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2akyeuxfi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2psitlqai.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2iszgjadk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2fleovatn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ycaevbor.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yoxldfhx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2dbtajvru.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2kjlnrwvs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2thvvbthx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2sfzxvpnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmucxamd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2oqfznewx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wsglzmrq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mruzcmak.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lkggzbfj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hxthixko.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2brxkucbu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2owebsrpv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2doxufifp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mbfhznip.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wfcuqyqn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2sczrhhtn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2srhffchw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qzojewuf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yyjpgltj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qxrhvehy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ewfpvoyf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kqchjbwc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bwofsdrk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2qbzehyog.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nrnbtpgx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2nozxpgwm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fqeiduuq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vvbldada.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ajnpljyc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yrjlpqgk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2jldfewai.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lhjivnbj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2acqemtcy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2pkateluf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2nzdqsogs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ymugmsfa.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fpqjihey.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2apxiwovh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2caphgmst.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xrpmhzgu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jjkmcufx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dsbtjake.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2rlrmtpuj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2dkmarhhw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2osakbttw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zrdwsnrn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pxzzisjl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tblvqefw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kheyutvz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2twrnsiya.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ddjxqvwz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2uiyvbkoa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vkrgjrka.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2eleuvstp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lqwbgtwx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mlyzstvy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qslffhqn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nlsvzpsq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hfkmwacw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lgafoujp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2uegejwtr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vbqbwxxv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2hunyjbis.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ivduopkw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2recympvt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gpfcmabh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2gsgkjgdf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qrgqdhhf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bdvowpcw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2oeuidcia.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ptqcyqfb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2yrbnolti.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ldnyuxdg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cjyrqgox.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rdpxiiac.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2eaaeiqoq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2opoamvzv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kjwdbjfi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2oxfmewkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmcjcskr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vsrmprmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjvupvjn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qrykiyef.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xesxluqi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zgnsixnd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bpihjseh.html


<!-- 参考信息 -->