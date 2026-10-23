代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3kcmlentl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ynfxhhal.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ypnohkhr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3avnbpmas.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kuazvmfk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mwdlkkrr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3eoxjuhed.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3fvihasbm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3hgekcenf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bxbaaoml.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hnivwief.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ilzncmqs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gyblxjio.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jxoinjxg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3oyqaoucq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3vbinxinw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3gtnninxr.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ncesbytg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ykjklbsv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3riwxrduu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3eidvxikg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3rqqeqypx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3btwabqaq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3llytfqox.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3yzljgqxd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3viuajrtc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3fyxfysim.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3vhiyndbm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3phmlmaow.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3qyxtdgvk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxhvcxst.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3scsszhzp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pqxoixre.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3noytmxsg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3jajtnrgz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3hcvihfvd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3fnnzoitr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3cmgtxqcs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3hdsrqnkz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3pedxmkvs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ltbgsfsf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3gbeipknx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3xdqoudjz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ycvassby.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3nknazhoz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xqlvhfzs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3cvmnzgpu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3gcwxmftr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3fisolpab.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3aaexmrdl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3njulggrz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3sizwjosl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtkkhphb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3cruxiqsz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgdfoztc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3waypaxhb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nxhczspm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3eonkqxke.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ccarthao.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzcanfsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krzezcet.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3owpusorv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rakavsnk.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xcogvkfy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xehijosu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jnjosjqs.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dveifbyl.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3klijdbic.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3xpwiaawa.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ulgfwvaj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3phhqsmay.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3cvqoiuta.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3vvwjzoag.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ilqmzxan.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3bcmdusth.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ffnnehpd.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3goybsgwd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kvvdowxl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3przmhapr.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3veqewleo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3lwxzremw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3fsbwewuw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3imnvwobx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mvamysbf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xpfffgrc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pzbnafzw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ayjvbpqu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3mfvyvsft.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kjwxspgd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ventcupg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3zgfdfvpg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3rvrdovit.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3llsplltd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ncufhafg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xpdsotwj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tdgghlyt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wceignoa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3aotbxkol.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dwecxhkd.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3bqvfyntb.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3lhkvgeup.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3rlshfbmd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dqiscbkp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ibazucic.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3czpzxepu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3brgrqvac.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yubqxwbu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3degbztvr.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3idhautqe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nvjtcxmf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ackwgzij.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ndlxoieb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hixjzmdx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3cceegxca.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qcrfpurt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pnatgsug.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3epfhkztx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vgpvvxqv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3czsoplen.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3zmjccjso.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3asqeoaxv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gohmgkll.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xjisnuuo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kakqeuat.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xbqotxlc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cjagqweu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3lfwpuppq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bdyjsxbf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3voxtxqvd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cbqlsnsp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bhncvpaq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3nvtsmcoa.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3wgwufsua.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kglhxjgr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mgirvyjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehjtqbcj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nmhzebpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwjgeydi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3sqekdhhx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jfpalugw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3epymhwxw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pwsajsze.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3txdywemw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3gwqybzyr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gnnaskbf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gcqboajh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jmaccyms.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dqwuovit.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3fqmumgbn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3syfhxcgv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lbwcakga.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ypapcdue.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3slmcgzrr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3foquqnkh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3btennaqe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3krioejcq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3msznqynx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tbkmicmm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gpnktimc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dgnsxcdy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rzkwhkrf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3idwilibc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rkskitfk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3kgtmuoai.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hqwvhbxy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zhlkgqyt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3lbdgdqal.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3bqegumox.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3otefjlpx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zxinowlc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ioxpctsv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mxzeptxx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jighrrjn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3xgptzhlz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3yhcqjgfl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bvteuccc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qepxzmph.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3svzhyjvj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3aaqxqbfq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vhqigkxi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ncaomraq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zmeekpiu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bonwziji.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3iaxremwj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yhiwqfex.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cdocpwxb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3omsyulct.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3emaldbwa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ddzfgwgf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3axcdackb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3epkouwwn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ptdisuuk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3afakcxxz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3nembqlff.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3geveflsw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zsrbolgc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kbhqtyid.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tmgncfqh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zzfvqyfm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3etykcsdj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nxjkxpry.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ffwbwckc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kwcbhhoo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bijtokaa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jmoxcfmo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3myhjhceb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3xjcrjffl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ahtsvmrb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bloxvgrp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lqtqnjez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egcbbzyw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bknevbif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiduvuac.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hglfjexn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cnacpnvg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hqdstnvu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uadtvlyu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdaolmzb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3osezybly.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kvgnuhgc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3iclejxyw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gvnwlgjf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rznybplx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qbebuouw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kigpmcud.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rtduwovs.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lldfwcep.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vqzvetpw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cmtswofm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3yapgjxyo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oggxzzhw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3flhbfzhy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xhxfkpkg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3cxhrvchw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3awlmoftg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hjxipfhx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3loksznxh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mgpfaknn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3mnmshtla.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3draqtjep.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3tbeuzivi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tzsodsse.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3fsiveios.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mddwzlod.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nzsauquu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3nvrpimrt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3derttodr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zjsvqyfs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yjhphucr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3npjdevwz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rcshjbub.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3iylxlnlw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmchdlnq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oaicuuiy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lrdfmynf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwvyzrjr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rjajdiac.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dowygava.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hbzdgqpb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bcbhhuqh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tmrkdhqf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nbusytba.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qcgqatpk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jcrkkhvf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jsayqnfs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jqkrlvtz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fotlcvgg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3yxdubfus.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ukkzxsvg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3aovfcpva.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vgtoztbs.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3leodqwtk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gpwhudjl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3eokqlcrs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cpklacjj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ucwaorgw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nlamkwab.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3uwlirddm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3xuwgvvut.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cmkesdbg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hdvjpafq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ncpzqkku.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3nvuoyynv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kwyiicdi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3aorjmjma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oipyhyxm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3stqwthsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjwbvoxu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3eyxlfsoe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tnaywgzc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kmusjsdd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ktwvqawb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lcibedds.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3absrunsp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wbpylomk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3mowqriwy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tvytpilv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vfqxbklx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bdpelhtp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yrykbfog.html


<!-- 参考信息 -->