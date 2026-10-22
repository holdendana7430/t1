代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2siluffco.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2zzkhlikx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2iqixeage.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2txvuadkn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2exgnmaww.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ohclxgar.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2rkshgzlv.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2iuhbbtgt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2thqpsoia.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2svfqeqpe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ipzcgrek.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2lkwmudaa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2boogbjrw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2itrcziee.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2lvmumreh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2uwnscyql.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2eftokvtg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2qhnysfpc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2jhroqszk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2satogyce.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2incausgh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jdxcenkf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2rniywttw.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2smmdqlyb.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2mmxxvbtd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bwchizue.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2azjwacko.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2heqjcgoi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vrbypsgf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2kqqhywgh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2mlzmudwf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wvgcncco.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cdssdtnu.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2fenqyzlm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ortwzybz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2mdghwezp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2oaahtjtp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2hulgkskg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2cipoziup.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2uerdbaaq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2grmsoony.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2irmkdpvg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2bifvslof.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2cxyqlcuh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2faudmwcn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bkmshgai.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mxauifcl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2fyzfdsrc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2wcptnxhm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2okxhxtmz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2kiaqsotk.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dggdatvp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2rultipqo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2gnltdopv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ronjinnq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2drblgiid.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cxbpmwcl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2zgtmmvxh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2lmjpvqlz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2kbcivbmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcyuejiu.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2eebokkqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkogbbri.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xvobkiaa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2oyxnithd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2djhhtudy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qynixkjp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2skxezsve.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2jivcvfff.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ddkczapu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2szxmbauw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2winflfko.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2yqdtdlgn.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pepfxibb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ufypmxsj.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxomnvij.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uigjyxvh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gbqpotht.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2offuwjbx.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rjdcjqzl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grlrhkag.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2twfkxcgk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2hfzeoilj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pttldbvv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywuhaxtx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffgrhstq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdxkvoio.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2uxczmyym.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2efuyvoha.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2pfczuwtv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvymzygn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xvxdyzsi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2iomhsqoy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2lkzyrezg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2znduffrl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ostixcsr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ocapzmec.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wkwkdnah.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mlgmsqgw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2uufdrrqe.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qifghqss.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2vjvmkbxk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lfzwqhje.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xxqqjpgn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2fkkhhemq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zkfylqfm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2lxyficwr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2exhikrho.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2xwvhdluy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tvfkrgti.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2gecopqfj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2faorexkj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vnlqxofi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kmkckhwq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dlgxmjtv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uawsaucf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2erqqabxj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nropeynk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ryoutila.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2tasfjxxg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2eipbfvmx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2viexqxih.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2akmkomee.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2wcxnlzpe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pgileayb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jfrnebkg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2hdenvepw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2uzdrxund.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kwnhjhgo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mstgjgru.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2asihelqf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qtpattrt.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2biolvraa.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2poxibqnl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hawtnxag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysxvcuud.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jvioozlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yywdfhus.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2gmihknxu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ukwytlnk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jjunyjjk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wmwrgitf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pbiqbzgn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ooxgdjpf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2mpcvquxk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wbqpgzdt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vtkdotcq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nnxuuvwx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2iuhlyqxj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2zbxiciid.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vcmkjlsw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xwymqbuh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2kndteyep.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2gfdvffnx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2pnsypihx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2njyrmwez.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2kzyrgqdq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mkdqfadt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dbzwthmt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2oufphdxa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2obuybitt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2hggkqgkt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nkiaxsgo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qvtzkvxq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2orknimkk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2nahztkoz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dvzaudix.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2pbffoqjo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gnjjjtli.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mvcivriv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2iujrzcds.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2vytwjeet.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2txjryxcf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tilqitta.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2bxpwezsc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ykizwuds.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2nbobdxdg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zmquirbq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fiyiwgkm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qawgthgg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2aditudio.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qnogllcz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ixudzvah.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hkjijqky.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cfjjolqf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ppjxrdlg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2scwdhnrm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sbtzsabv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qaicsags.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2yrkdrxsc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zwttrrkj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nsuvoxkc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pzkahqul.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fmbdiipr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fbqotefs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zrzaceca.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lqqdzbou.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2qlxaduqh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nuxxdxsy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2dpejekob.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2difivdys.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2azmihizh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dfnhscok.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hnmpwldp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dhmbylhk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2moooeuhq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2drrzekvu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bvjbduwf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ymrummzk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ghxqgllp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jygxcjce.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2shrluvrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chflohia.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2idzvockq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kkybxfuv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2iqpuxcta.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hggearzg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rorfanqt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2oetvbdgu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oboectqq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2nfrxslzc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zjcprcay.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lyipowlv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2faxqfuxc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2drknubaw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vkiranyr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zgrrwoof.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wulivezq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rsfuiyzi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rckxisra.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ajjduqvm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ykldwnvt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fftoynyw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2cxxiqyvo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nlzcotcd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xlbclnrh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ojdgbpoy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ygpullxq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hfjijzdo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2elvrials.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zwwlnmvd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tinacnph.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2bktiiiqd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bctaeizd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pojpxgjo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2llnzkzzc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2uesrnbjf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2abqykusj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tglvosog.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ohctbjyy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bmmmwfcg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lhjystjy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ticfexip.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nbswshrd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wywxwnnl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rdyxmbto.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2khecpukb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dldmpqut.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qelplsax.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jpoajcfm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2uqnglhxd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vdpmkbvy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2iyrknsdf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ywndgofr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ceatywoh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2sokshmjh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pkcqwcqv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jwtlsoep.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qasrdama.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pquqmxwx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ebqqrnih.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zivhmwug.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2nwttstqc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bhqubfhy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2wuxpwcek.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxhijlw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mozorhad.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rurumaha.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2tfvzjfng.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fpdbwoqx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fmsdeoir.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bnuhflbd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2lyiohiqr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2riapfsrn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tkhdgxbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfdnebjb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ivvzdbol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aesdlbet.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wbghiunk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ckhizwcy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pldsyxhj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2amwmotip.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2afqtelax.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2obsjhdhr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xegarsxq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2irlefjlo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wqayiltt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2isvwdrxg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ploqxstx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hhyvmwks.html


<!-- 参考信息 -->