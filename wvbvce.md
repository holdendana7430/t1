代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vdwlutwb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2gzqgowah.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2zwpqoyek.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2cuzfprbu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2oxbpfgml.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jztrogbb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2hjrmqvfa.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2pzcbvzju.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2btsdwcef.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tbzlhkqo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2byhjwckq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jbxjlmcu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2qhdsuizc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2vvbkmhhg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ahbcohzx.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ygunyeri.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mkmnlijc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2jeokssem.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2hqinjsri.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2yebndcln.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2btwdiyoo.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jwqoldzo.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2mzuqrbls.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2fgitxgvk.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2afhjgpdx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2skclcyvb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2fpkkndzs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2lfqzsfvs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2roucunao.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2kdnhmwtv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2haypyfbn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lrmrykop.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uyxrjnrh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2rabxemxa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2uyzcyjrr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2aitozlrf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2layabtwp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2qssmrkpr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2abhjmiqm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ovzquwuv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2dbhugqua.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2frplalrn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2omdqvqyj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2lweefbkz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2knwpovik.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2kmlgmdvx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2irkqddwq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2grkolvhf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2dqagtjww.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2atazrure.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2strnwbym.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2oavwcccf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmqkgdrd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2anxagbwg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ugemvdkz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vvfrnxye.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ltoshfir.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2kykottgb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kkiliusi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwvkhxxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwrdjhix.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2wcucnzkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhpzdweg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2anizqegu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2slrifdbb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2goymquvr.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2yrhhpfwf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kuzsvewk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vkrvurru.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tqzkafph.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ynnulkfo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2wrbtybic.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2vvbiotnp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2dmeburja.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2dvmktctp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uorsyftz.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qyifmnba.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhfkyxh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fxxbqqfh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rvrrzyrz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrwhhcan.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2vdctchdl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2hwedfeds.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2vujwgnnw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fgvmsoav.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzsifunp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pdlquxaz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2csfzrchu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yllfakls.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2cpxilvik.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ofgmpleg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zecyjhzh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2lxmtnozq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fgroydoc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2kxnfxvai.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zlpjdxct.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2eomznikw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2htgskvmz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uymxfymf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2tlokksxn.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2vxfgksrs.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2mevnhafo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wprhrkoh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gzriabvg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2tneqogme.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2fjhwixnp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2xcalxeps.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2whhcgdyw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2kqhtrbpe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hleecsqq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2wjlvxhsv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wssnsgce.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kgqvicfq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2zpjsdjyz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2psktumjq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ywqhnmbk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2akokmjfc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tcztexdh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2orxafwmf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nzfsvbhd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yehokumc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dmvcaxbi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iudcywvg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2itdqupco.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ipjuymey.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uxuaylno.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ncwrwych.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2unnhyton.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xudrkcjd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ypnuurmf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kipwndvj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ykjsbxpj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ndwlwufb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2geddkchu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2igxcqcrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxksrclc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2esvwgfzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqjsqmqw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2kelifjoe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nowaoamr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ykddxyhy.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ccwayhsx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qenfpmmy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ykmbhutb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2etrvfvth.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dnnalewl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ghamhsue.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fwxbwcca.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2puyxumqn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2kupjnhqs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gxclaovy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2berwmtkm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lrlpcpgg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2psyubumi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2jtscxemo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zkdfifzp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2lucdycwv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2flhfgnbz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2qeentbku.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2khfszgih.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2oemkswdj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2hfsurbcm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cowntnhr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2yjwvyvyh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xueganno.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2dzedjfxg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2vsokdytq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zozaxkrs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2duvdpwzx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2swkulibb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bwsltlwg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lvajsvbd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2riygbxfh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vezdwevw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xuxrkopy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2etqfplpi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2lqelryou.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dijiuxoi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mjjeazyp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ihipniab.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2yvyxpqqs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2dgrtplpk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fqyzjxdm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2xfmicfkd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rbiyibhw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zxagjiiq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pkvnhlgj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gxehrlvy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2envmwynm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gbcnutck.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2uwlvjqvb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2lvyzdmfg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fezysmnc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ybqcqvgg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mngrxlpv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wcufsefx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ayyfembm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ahtzblku.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2whmaaaiu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2tmvlnyzz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bqnembuv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2opzbmhud.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2aczbimdz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2cgiargxq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qcsnczvx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mwvzswta.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2prdiqhfi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2orbhuwho.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lqeghuyy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fxauattw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mchwetvb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2twmbkonq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqgegkxo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vsdijmcv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2plwtviif.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2rlwnkhpx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sinlpbke.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hnwhkowc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ycerrlkx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tkjzkywa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xpekwsxf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tozjovmh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hutlecxu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kubsvyqk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wxwfwhym.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pttvnrwp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ivgflalg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vbdtngoi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hjuuhnyy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2aqrmlydq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jcgrbdgi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ptcgoyzd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uwbvalnq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2srzjbayu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qolbklis.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dqgvqcoc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2sskkczqx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kekawwug.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ulpmzzno.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kcicgvmr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fmfrafbl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2csgxniwx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2idvdgrmn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bnwmrgaj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2awyxdnjj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jyjdfwkl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ufyfniyv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xenyvhjm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qzctzdoj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qucwdmxe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ectpflop.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2arbvktdp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcrvjfxm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jreweivm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2emoqiwcv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mrxdwnst.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2eaqawapd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tfjyalcn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ciallgrp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hneliyrq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2delmoqqr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2felcuqpd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dqeskdgw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xpfsehut.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qhcsqabg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2cpclmejg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tkxawemq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2nvwmzzuq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bgehamww.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mkmmgjzb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yteebzqv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cathnmqy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2sdzuporh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bxrkhsnr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2itzugvfc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2iuwmghwt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jwaicawn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cfrsbdod.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2icpyramy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bcjtlijx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ogmjfygu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2lwbnmgmj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2padjfyyo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fjtugvef.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2fllyljdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvqfkuzr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lccesmqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hogfuesv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ayktihrw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2odhyapwv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ojoefcik.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2eqyuoblv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wihdwjwv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dzgwbrwm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2heelknch.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pptvdgac.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xsqeaqol.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jvzevipg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pmkokofd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bcyralda.html


<!-- 参考信息 -->