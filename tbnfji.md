代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3yzaamwkc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ftymcplf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmsvqnq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xcrdxbwz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3igjonkxd.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3swtaadeo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3dpnngjnr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3rzzogmvy.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xqfeobnh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3kpvfghik.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3xuzrbfpb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xnfespye.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3rkgbwqdr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3zivissmg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3pvpzsvbj.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3hrwgbvei.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3gecqjdat.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ywlgmizj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3aapphvjm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vqeuekjx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3tbeahdwi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3jexryuum.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmbtqxff.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wcaxyuez.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3oynbnnhv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3afhmphhj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3oozbzafw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3roimyumu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3asoozcus.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ntfhprqn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ftcolqri.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3xzvyassf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3oyhnwczd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3rhrupbdp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3sfxmtqrl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3fxikqtyy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3bhqrwryw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3idrgakuz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3phdnnuqs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3cejpfrvr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qdfyjipi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3elyrumkg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3drmmvxzc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ixotruew.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3zjejqfvl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3utxzlalq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3baszkfqa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uqrxcnvb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3dkslkxdy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3kyhihcoq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3bxocakpd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbtabsfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mveeryam.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3trjjggck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emwshilp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nvziuoen.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3cuuvscjj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3oobctlhx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3owvvwhqw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jszybard.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3adpfotvk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yucdohus.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3sbbppmif.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3uizcbvgv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3xtfjwcvh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3kxbvddkm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3fcdxketg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zgfsqwsd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ouysmhsx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jmywgopr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gqmwnasy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgwqcihr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iixnoywy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3vypccdhn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bohlfxgb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3guxcjzii.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3iokefzkf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tliorrjs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ieeyqrhf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3tuqasapt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3vpbykkrc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3jlgbgkev.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3yhlajmha.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3dmebxgsh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3haaxlhii.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nbelgvih.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ttmhmikz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fiooxivl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3npmliwwc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vshbczmu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3deqagufk.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3oplguwig.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eaqcyzop.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ewejcgtd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3znbtdqdg.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3turoibvv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3oonpurlx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3kvvpehir.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3tqhdypuu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3qtrijzzz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3vyxessrt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qgtxhxkq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3dnkixfhw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3guzlofby.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3lqunqdov.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uqipebko.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bvamigfh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kgcnwddh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cszwpkby.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bstzuirx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3miohnmkl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3amudngam.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gmcswubt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dwyyjepj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wvlbsawr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3jdahtxdn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3rtbgvkow.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yclvazdr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3cvtvkqdh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3xvgreqjm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bwzokuwq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dkzhxcik.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3aivnjezf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3fjyoxbqw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3mmingnws.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rxvzkpeb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gchmbbqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nukyhknv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3eyydewqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjpwqlrn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3bwemplef.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3amlhaxdp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3weihkbig.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lrdmtdbl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xwhyxomi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3gfdqboka.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ykdapdhe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3lxilynxy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3iotlwfof.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rpbvxopn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xtkykylc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3epvnmmtb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uedeltqq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3yyeungci.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yglzzxjs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3akrxpcbj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ttbetewb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3cwqwhzvx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zhncrdbm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3efnhyida.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qfslohxt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gyjmokkw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3peiyohla.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3txktfavo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uvgrxtuj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rspnrult.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mmyfefph.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3psnbscvy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3uejiffiu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lopvroqz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wyvoptwb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xbnkmwpu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ysjmugrj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3yamvewre.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tmrgpmut.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ardmpnwm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3obxapsau.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ljwmjpfi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3pfcnnpzi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qbapexaw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tbsqswoc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3euanzaqb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3astxghco.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ssfsypsz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wqsghrij.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3caywtzai.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iafbitnl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eszxrafq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ykoiqflr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fxiynomh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3srupfzwl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hurgiaxy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ktudvrji.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rfcppddh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3baaxisxx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kwjfdttd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vejonasj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3swyqqwus.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ynkxgcql.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3kojafokl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3haegitnq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3hdqzgwba.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yuppavlb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3hnowfbut.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xqlfqjom.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3evdkylyb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xsgscnhu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kdtxurwb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3panfefgy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dvgrxvit.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3oniedknb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jrcihgbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yiilbesk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3angwciyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olavnlct.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lljlawjs.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hqrqbuqv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rwefvmfd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3afznbsat.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hvufnevn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ynczeqem.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mrclxuzx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3sgqiutqg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dbdnbcor.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3eadezxvp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ysyeljkv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zqvnqtwo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hsktygog.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mvqezlvh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fylrgtcg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hnclkxys.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3okbwgdbg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fbdryatt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3getfvzpl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3sjjcigot.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mqwqfsnn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vhyanyvd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3emhrpuam.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vmozxpll.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mehhqcwk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wpsxtvxp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3sjxuhnjq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3dsflrqyb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lkwzujgd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zwrzgufh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3eaghodnw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3camjdauq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ojtltgzv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3frmsfzej.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ibmmcrzc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hzutlgfg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3umbylnkc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohdzwfuc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bdvscoll.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3stbqqitt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zfwoxrwh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3krouowmr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aqegmgfi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ujbacmur.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3efepsskv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3liclhmcg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jgidipep.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pwvfpzhw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rjetqojy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zsdrlnnf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gmraicpx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3dnbjxmmj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kofwqzyb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jglnjscx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3pbpjzkuu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3opqaglio.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vjuqxehj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ordqjdde.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cjpsxajn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ssbswgsu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vntmzuoa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3oeqzrwuy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uubmvbum.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3enazxhgz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3znkleten.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3bqreiyhj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yjwvefge.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pvsvjygv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3aiiismpy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jgbsoikv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bgukqwfe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3epmfpwsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnetjdtz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jzpiqrog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfwhfuoe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pawtyiyp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tsxxcgsq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ojbcentp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sjihbgwj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kyvpwldc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zrqxjfcs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fncziqij.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gevxncuj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yomneqwa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qqyoutyd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qkdtkecw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3taodwjfu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jjojdmpe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ddlzpztl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3pdakjhxg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3prifwweg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ajxisnbe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3eypbymxb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ljmnkhkm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zpjhtadc.html


<!-- 参考信息 -->