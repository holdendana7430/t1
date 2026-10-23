代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3oycyzouq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kretbahu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3rrbaxmlp.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3uhilswph.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3dpchrcjf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3fblumsyj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3arrfhfnw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3evpnoero.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3hzhdzwag.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3tpquhflc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3cuduehlx.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3iyenryqz.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vcmckncm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yohjcsjv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gihfbxzv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ynlfobwj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3kxoesqgl.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3jamjltvy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3rjnbhdoo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3igrragjh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3dmfvourh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3eotdmbot.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3nolikuns.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3hjgsguus.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3thufzbaa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pamfemuj.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3cupxzuia.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3htmujfrv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3bawypazy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3taqqrhkj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ksyjorjt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3elgshntv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ruxegyxa.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3jrbobqay.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ijbsmeyt.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3dgjxktih.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ejsttgem.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3yxeqawpu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3sgdwjncb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3vrqucikt.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3iynkzgzg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3pynewjvq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3yosfabha.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3cqwbifuw.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3eohfoojx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3megbwrfh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ipmsejfe.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3tjylsnlo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3gptilwnr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3mgwjfmew.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3yhctigwv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3feqbtpzo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xvqfwrzw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3smdmxmls.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3adxygavb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3arvxhilb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3bzqswibm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3czkoetgf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3fqqlsjgk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3widzrmmi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3pghmkfxe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3eqfpmmfq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3kfpmduch.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3spueexze.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3jxthldlk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3dajqkiuy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ogaumkbf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3hmqzmvqx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3wgnclxsk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3frpymzae.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3upcojpcb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3lchvqrha.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzchnwhn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3hdiwnnlx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3lbetelrp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nnrvfibj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gsyzpest.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3rtcglrtp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3szrhdnpo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlubmujb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jedavhrt.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3nkarwhon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znwzrgkt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3tpsiwzhk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xwvedxon.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wzgaotus.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vmudacnb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3igoxhubd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3xkkdsovb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fiokycsz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3eqpnkxgt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3yayunfsk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3eryfeqnl.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3vexoiimg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3tyxkuytb.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ioujveqq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffbgavrq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bqehpkow.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3mlzvuaqc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3csyqnsla.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vwqmbzsd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rklmstia.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3sfmhvsee.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3issndeke.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3klaxdsym.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkguyppw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wdwaujwg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3uiiuvngj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ladhihot.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3qwxxwhjs.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3wialghns.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ivanwtva.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3cuegdfln.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ihnkzauw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3brjsrrlt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3aiieinau.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3tswyandq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3stxoikxt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cjzkemjm.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3sgcvvnby.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3pldeinwd.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3nmmsqyrr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gkwxtwgc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3edaoimmh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3vnuxogxz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3guxnadlv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3hrdtkowz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3qyhmjldd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zrjvbmaf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wpcxdaet.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3fovwgoaj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tdbjzups.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xtodihye.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3litgxjny.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gapcnzvz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3iwjyujwe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dixgxxag.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3radhmxxo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fustpoeq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ncurmozy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3blmqscdi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mslsuhzs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uduiuste.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3leexwqzw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3htonedhr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rebpcgrg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3zarkzhow.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uyejupxq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3edmzpcrp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hyqbxkme.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dsaecogr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3foncbduj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3picmfdzj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3mvugomzg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ujsnkvrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfarjbmh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3qjifvatq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkcjxsmi.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ucvgjtyu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jbxyijnm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3oqgpmpbm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gxknvvct.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pnegjrjl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3xvmviggt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3chciradv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3qfbnjsfs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3movxbnzi.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3auorhxsv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ctzjqmtz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3qkvjmrtq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3angforlf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pfmvlafh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kqzqiacg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3nyvvdghm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zrkinjhv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3buuqmzia.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fxiflxyf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3usgnoyrt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3wvdhwjfn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3eqecuxoa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3iejxtmeh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3fvgcsfur.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ntabfklk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ooivunrj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3imiipyfl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3tagjfbze.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3rzlddovf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3gxzraaou.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qtjnxhrj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3swtuoddw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cegbtrgk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3wmwohwyn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3dttkkqfv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3kfglrgso.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3oipzzstn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fmiwkmeo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kadubknw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vlilycpq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yxbxfznp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3phmokhba.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3rqhawfse.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3waecaazn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jbnarjmv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3fbtemown.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jonjwtld.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3feeensgg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3smcpnmxm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ssntwgsf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dwjgkyhi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3lynyovha.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ywrcwzyr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oropunil.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3teafatei.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uejlsfav.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3nlkwjzex.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cvuxdszh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hjxufveg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qiumzxff.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3trjjfmar.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jzrjnfvz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ygpwnbij.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3shgblrzt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ngyebdgf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3huocddgr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3iinxtrbj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3axygksum.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3tiwviair.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rlvkrdjg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wqqwzeyg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jzofobdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjynoefu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3kdfchjyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbltudhl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3infyalda.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3kvsprgwl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qkrlsjkc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sjdguqap.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3oxdfugpe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3eobeibqy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qwqrauqq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3lurymych.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dhdnatyf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xltncnfj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mkfaoywb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bljyztnr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3onevahsd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3igyqqtbm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sypgitui.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qkirzkqh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ixdqbowg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cpfrrkqa.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xxtirxub.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bhplbxny.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nytiqran.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lugluwlb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lvftzyqa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rljsyioc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3utdceqzm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cfuttakj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tcoytocz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ubmwvkgk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jupmnvgd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lfwgnhhf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uylajfss.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uglqyusf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3utgwwfcu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lxsksism.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hiobtbpw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3nlmjrqsf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jxayntgq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rxobqnwg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3klrdjjdd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3guvizxga.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xpreuruu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxdqjrpn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pvmksscn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yevofeul.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yxqdqgdv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rypnnpmw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rokgkiuq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pkwtpzvb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3sbulupji.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hvtdrjib.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nhrnjpic.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ffcwdion.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3xdtxohde.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3qrxlgkgk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3yiwbwoho.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3witgkqly.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qmfvjzzi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gqppdxsr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vbbdqsbt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yugxacve.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dazowimr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qmtuiuxi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ovxkosvh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nnoasrbc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3emswpznb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3onrpvygo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3phdshpkn.html


<!-- 参考信息 -->