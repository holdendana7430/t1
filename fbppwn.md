代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3icqtduaz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gltnsdia.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3mozirfov.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3jtshidhk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3kxvxqloa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3dclwapeo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3yuokdjtr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3wjqpnpwx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3hplqkpku.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3yfzmbvrr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mnhirkyg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3emtfhntw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3lnsvubij.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3tibkuuiv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3nhbtqbxr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3fhjotitf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3hlzvzyxx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3vrtjkdxv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3zzlpnimd.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3rvdupplj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3lbgvuvzv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3uaefnbgt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3hsvmjsew.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nzogaita.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mgllzlip.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3znpewrny.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ysmiiywn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3iffolrdj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mzqrgjzs.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3mlzuonbm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3axubpvbv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3uvraruav.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3epmauihq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ttgbbrxg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3bgeigiqi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3noyodgcc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3yhwmpzfa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3scxsxtfn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ovztyrla.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3qessrdqh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3sgkpdgku.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3roskmkqe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xgyelkxl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3jcwqrfud.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3vgiepzjo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3bmhtwznb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3uanxtmye.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3yabhevst.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcfotcnk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3euuekrau.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3uvlvogql.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3alzpffan.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kbpmluyi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3svrxqvbu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3bgiutide.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3hkbpvktv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byfmfeuf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3cfvtxsdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmgvpxym.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wduduoqy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tmyrpctu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lbbtvnwj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3melsjypq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vuafsbec.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3hrpqpoyd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3assmmwtb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3tjegepsx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gbaoujnd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3vkhipync.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3blchosdl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3hgrvedaa.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjgafbnk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wsoxtcsp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zvbflpjm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xuawebwv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwnzxhug.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3eltmkcpq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3jcipdpzr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3knfeuupw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yclxqltc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3gaiuvymu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3siucpvkb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3coruzovl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3olgwabqb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3roodxzuk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3zyrohzdf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3kyejrzda.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3snlvkdxm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3sbenbsso.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jgmnkuwz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3tlmisidt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vdvwqgut.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wlzthsow.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zbrhuhov.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jdcmmfok.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ngpxqatp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cyvljokd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3sirxmqgb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xgweodea.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wamqqlcg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3wpmjbhvd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zxtnalwz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3mhykxzec.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3pqyaretl.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3nkfwfeej.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vbtcagmg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ojwbqpmk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3sdrhxqzy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aqaychml.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3iydoesby.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ieshliwq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kqtlyhht.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ggdkfdil.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ibjlwuus.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iwexqkvq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ezfzigsb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qjwldcmm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aulfuvgf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xsdrhztn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qwaykrhw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3osvgculy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zospcyvl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3sjcfexlt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lbbwuthi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3incsxkcw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xsarhjmd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3iahtihte.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ivantjaw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ilxptvir.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3rdedczob.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hbbasttv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvpezvhh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wjmcfamc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdtoqkgn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hiiaxzsk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3adluccre.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wjhgnvdq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3cbjilrwu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3mpplqwjw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3orntdunb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3mmvsvpkw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3krfphfis.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3zwhkwjsf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3stlxrrxj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3judprbje.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tfspbplt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zudcqrkq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3btzphkqh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3cynaurtn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3nmjvwwbm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ufdoebkx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fxkxunib.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3usikpaie.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hqpexkim.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uezxbzpw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ajkxdako.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3grtpcjzb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ifmgqinv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rpowgesb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3cnhrnzck.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xdlgalgi.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3hrsgqoad.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jspkoqgh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3aruznovv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sdvqxevs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lputksjm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3novgaolb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3gnvvfvik.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3zojfivrq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mfdqqeky.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ikgvmwww.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3tcaepwid.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3yqxmhfrp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ogjykixf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kprzokkz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ocbbptjj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxkrqiav.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3mnmiwwfx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ioikagbm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tubgndnp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bkqjvnbe.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3twcbvsrm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pcdfzsrg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kkezjfgr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cdyxhnds.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3yfbsvpwy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3oivqcqai.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wymhnosn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ygfbyrcx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3qcrazuta.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nvbnaaey.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bwkqsdly.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dubkdpsp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ilgezljc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3czwhhzde.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nrrpkhpy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sloonuyl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3bvcfolvq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pjglvbxo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ohxrkbct.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yvbcmkvl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eyjmptai.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mpanyrqa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xejqpryh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sgjkdgwx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gafntryo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhkzoygu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3poyaujwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbpurmob.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lniofthl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qsdgvdvw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tlzvknzf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rvfyvtcn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjyvdggc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zaohcttz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sepshfix.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tpnbwzqj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3chirdabr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3huuysyxv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3krznmnlk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ohonoejm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3yabnydxr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uafafjes.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lvouttoe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nkodnwtr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3xjmnnzqn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hwzwbrxh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3uqepblad.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fxxwyckv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nnybtvga.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3krdzqwkt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xqvsjbub.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kaxsagjq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zbchkabb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3edtqtpqh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fclejuvy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3dbsxypvw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kuwkndnh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3upvojgxv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tftchmmh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tyfdumal.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ejixrkqu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3chjfuzvo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jvsfdtsb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3oooowjln.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dqpvmacy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymcifvgn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3dwptjjgh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dcvcnkxf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3trflqqek.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nlqomfqw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvaklund.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3aiwxvgqz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ixjnnilr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3einyeqqg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvbgoyiq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mgwtmsxt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ufaeefws.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3shtjkkci.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ejwyeich.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3pwinuxfh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3cesqjqhz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vwytypze.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3bcycbdcz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3draecjml.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3daxyjgfr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3czhkoosf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nesfpsra.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3hhvynpzm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3juuhjzsa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3opnekafd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ldklszsw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3fuvarllz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lqkabujv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3yippojdy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3frrakatg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mvjbqwho.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3uexlhnhl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gomqwdox.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3weiqtltv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3muaroivy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgylzwap.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gffrkosq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhqzffln.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dgohkopy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3diapgyaz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3smrdwvka.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bbhqtvrr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wugsahzn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifqzpisi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xqkhgbsl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3dpbffyec.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ajzwgpqw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tyojhuzg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ovkmarrl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sbdouxji.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vpdvnwnk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jfldhpnw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3fexmbdkc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3otofkpez.html


<!-- 参考信息 -->