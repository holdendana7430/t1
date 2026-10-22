代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2awxzorbd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2wbpbjrxu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qwqyfgju.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2olzalwqa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yzguttep.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zyhqbjfa.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2omipdumx.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2sratmcdp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2sfolawya.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2azqluitm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2fwfqeamn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qufxwqqd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iirrvabl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2qilfesgv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tvxyutur.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2rpodhwxv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rooynmho.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2bedgdhqk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2easglkja.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2kvwcavpi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2lpjxknyk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2fwhgwwtr.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2cguvlaij.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2yqizylvs.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2yrrdkgye.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2foelrstl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2uejrskrr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tsdavymr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2dgvlhiho.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2enqythki.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2vhzszseq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dzavzbpa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2icfdahqx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2txpjiqtv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2rglgfepm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2lqfadtqo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2mmfirmlw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2getckuqv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2idbfeobl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2zubksmqc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2naqnyust.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2cspxewnf.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2zcuglqwx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ptosgkiq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2rdtwozik.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2akkqdcku.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ikenzdkk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2nehcotgr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2bvlzuwzs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2rmqgevhv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2pcivarvq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2nhporpro.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2oorfbptg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jkpgkppf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mxpknmny.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ftwuwgxs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2klksztvj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2sntnkwux.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kecunxmu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2siirrjrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltzmoeon.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2kxwvuvyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdzpkvvg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2osvysxrm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2msfqmloh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2iwenurtc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ogbjonjp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rbwquhgi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2nxzitvsx.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkumxzca.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ddhbqxki.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yzxelqkv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2hggwcqfn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xsobhvwe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2tjnyyrvc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2avlupnur.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjnweznl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vhuzpogd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2haplntlk.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2pexezisd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmwbblm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2mkhutrti.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tyyutykc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kytlczcb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gnciukdp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqusxrev.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xofliudv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2fyyowols.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oefdtjaa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2fahfyfbd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2eeobadqz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2malcmkjo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ctqzbxqr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2olxabzru.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2scmgcrty.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pcymjrah.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jnbhnzqr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2omxjkwac.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2khgnwjxu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2hodlcffs.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ulsglabc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hedqcang.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqjpwysl.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ktoplalu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2glevihqk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2rdkxywek.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2eauyqyjk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2heutcahw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wktpdeyc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xdkwsnyr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hczfteiq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ovticwee.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ospyniqj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pwjopzgn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ezwwcxgy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zysmogqa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jdsagzro.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mcrzuvvv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jzibufiw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2clsiuyrh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2egqmugwu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tcrypfgp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xesiyemd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2wtcnggog.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qtoqtvme.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2psfdrsqq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2jxfpmdlx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2igcwrqjd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ndlffzia.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zcgisrek.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hihwgufm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hpirkfpm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2tcketier.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2hjnibwsi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dxnqseug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcheokfb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2pbvuiaml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evmfhnle.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2odosjaff.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2otwjpudc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2iyqzrnlx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qvnlsobu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kujduhtm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2vyhzedds.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ygjhseen.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zfmyulkt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wiczahua.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nxxmoodk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ywuwidia.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wyvgnjyh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pmremqsq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fkyzhrms.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2karbojcv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jqngrjsa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jupkypyh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2pjxhwlyy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2rrwleejf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2tcbvkpmz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2exeybmaj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xzxstgni.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vtbbueih.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ecmcwqep.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xlklpxim.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ofowyogj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yzmfkrth.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xszmamhk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ldgqwtcu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2uaxngoyo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2azcpthxr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2evedapcz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2qenxgbmg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2cxnpgcel.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wpxrikib.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tuyipfze.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2lrkfwpyk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ywntyece.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2lkupvpas.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kircgqaj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sqmqqzus.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2btuukbtw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2enwnzsch.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xdnxiume.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2whtefzzt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2osvsohbl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jzcmedkf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2njqmfulx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2udcasupe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2itqiywcl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mguhpqlv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2bcvwubpu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2qraeduec.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mlnlzqft.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wxfuhcln.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rqjpafdg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nwibfoef.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qenqovdc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2umzpqwmu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tttcvywb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jvjotdpe.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2kpdjimjl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yegwrlsd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2nynghekq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2hhttxzby.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2krovvmvw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jzkjqtbg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cbgxozoz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2iokkijar.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2imkuhlbf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fmbyghoi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2smvggvez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzdcfpts.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vimzdrnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yexalgma.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2awvcoytw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ougqfksd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ngnmxeno.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pxmflzln.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2taykvisd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wjmbhfwb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2lsogavzj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2uoqrbdkt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hhmedfim.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yhfqzted.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zhopamur.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lodcffkh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jtipkcig.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2njlazrqq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ykziqyik.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mnpxoall.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2louhoihm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fwjxutmq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2tpqaxcid.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2wxcguuxf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jnclrarv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aqxuzvvk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fojkfxxj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2skrrwidx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2peclryjp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jycfmdmw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vzvgigni.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2nihdxajd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zetzgyga.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jtxyiwqm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hxyoetpr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bzkvukzv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qwuxjpcl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vcacxjqm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2uxdoxoer.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2whlgivdx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2cktogvfy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2olnhpivo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vvhsjing.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xgnivcdh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tdjvprnq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oxupzsmu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bccsogld.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pzssfcty.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ferqbgpr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kblyeovc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nrvhdmso.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2brbfxnbp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kczysysq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vsswxvpt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uavblhdx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tclyjahg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2paqllmfp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mwdrnupu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2sqqsigof.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jbpcgyvl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nmhodcxj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xprhcetp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kbuyoign.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qmncumea.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kvqgdnaq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yvotxvyb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2axxsnpyq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mhjetvbl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dfmwfgrq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2itxgeiqy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zhhicpzt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2crmuckkn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ljylqgnp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jbsavkxu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ukbbzjjy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qeuicrwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxkwnctq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lsbcztsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cywtygkt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vnstjxbb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhknhzui.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kzyxbkbk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qxwrapxs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wohsanxy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xajegazh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgyevddn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cjrwnqxq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2unyptaap.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qdoomomb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2aaobsvmq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2osxdfikf.html


<!-- 参考信息 -->