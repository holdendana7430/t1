代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2nacnggjm.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2zoauhxdd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jxszktvl.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2maloqman.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2zrdczadu.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2rjeouxnz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2alrfroxt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2iijzhahj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jkskstyr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2jvhhwpgk.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2gjddhslz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2afvlvtrf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ezljuwdb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cukilfid.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2tirapaar.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2zlucopyj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2okecwzfn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruomcfad.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2jonjqdew.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yuktmzzg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cgkufmas.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2xagfeemg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2rnmblpdr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2jeozpnxf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2gqfwblmg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2svauzkjr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2oacewbit.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ylasthqd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2navfrzso.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2adbnglwb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ufdjslvm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2wucdrrpz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2fsqekjfc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2oqvudjho.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2uldyaprw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2dzuwoldd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2febyzson.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2xfsqksea.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2zcijlszh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2bekiaupn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2nyyfoaff.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2mjinamzj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lsjkxfvz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wptpfljz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hygjiccc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2nfkazfrp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2zysmafuq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ntxeizuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quhwrlcd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2xsquvbva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkggrrmi.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2djbzxmlj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2lfaruvap.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2slwjreoz.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dloiynrg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2meznwwvt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2scvwuuum.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2mcynthwx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2obqcutuj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tdhwwopz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2onublurl.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2czcgijtf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2rvytdzwj.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzufieqv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2azvdjhfk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zmxzobxk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2drhgcxri.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tarcqdkf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2gqisikox.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ubzezagq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gdnlgeym.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2bcatrsuf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qazyvlvo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xambdgvc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hprizlam.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2gjdxbwsp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2lpgfenif.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qvwcidzo.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbmsyshs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ofovnnvj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2oborbldo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fbvqzuqs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wpvojdpj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uymvzxbn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2crxiuedq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xmfhajll.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mremycjy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mhisypwi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2tgktxbks.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2yxkdngzt.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hbcpmqng.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xfahlxtd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2joaryxhx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ixxiamcm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lkwiranr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2zredoijd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2tryrniob.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ewiuftak.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2dahmlged.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pfxdkmuz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2iujiscjg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2feturrrk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mszpjcmr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pqmoxpsg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vcthtplv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2neaszvtg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vabmyjxg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2bfhtudkx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vyzmoztf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2etbvhkzs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2klmcvrsp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cljgzwfe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xyjpibzq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2imwmbqig.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2wccoekyw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fzxsfdky.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qefuzojh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kstfodhi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xlgghxmv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2syzkjrzo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mdgsrxvp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2pnbrladl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ymndjhbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozdjbjvg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2bwtffhzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwrxldtc.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qclmjiiu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2etirlezq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2hvbmonab.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yrpqnvri.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2erablkyq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ciimvtxt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rtsndkpc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2anqdlogh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2knqrfcxl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ohbcaarl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wwjyarjv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lrqenklh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cuiwggsz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2miogieuf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2dszgtxnn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hxapjolf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2wtnthpif.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kxjdhblv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wifhklug.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2twxstjxq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2njjwtcfm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wuegdpdf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cflmnohy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2vgiblnns.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2taeocpcx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ydijcyxv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jkopzqgx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2tchnrqlp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2fadpqprh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2olnbbewf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2yaajtqfe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2okkpvkpc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ulucuflc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lxsbsprb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2egfgbkmo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yxsaidqu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2arukldnt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2oxycjpri.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2syuldfni.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2eazhsezi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hsqgwwkn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2psxiephn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wjaclvwh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xmgcconm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nsudevgz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2oaoksgze.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ajpfopzc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lftlddoy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pyjmsijn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iqyurwpw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gznxzgas.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rrgqcvnu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hddlhiht.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zyoxtkyq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qdocavvi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2orvfbygq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2eizzaqfc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2asmvvyax.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fhnxxrgp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vduaeuih.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pkqndgtw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2tksphwso.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hissetjk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ukawwnrh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2tzotdrjx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2asbihahp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hzmphxkm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vhzrlcgd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tlwmphri.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2movlcjee.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2edltmepo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2unvtvzpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myywvihj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ipaowcag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkyfknzf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ywhdhdzt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ihxapynt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2muoekmql.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eqrrczld.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gfrzwyfx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zbqsahde.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rlymbwes.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2egrhofnl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2khvqcchr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ixrvdykp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wogwazfd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jqkstghn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jcxozols.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jlasxiek.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ypdfsgpa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tvfwlhur.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pcuqohwa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dsovrfqd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wigzdjru.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qyaahxui.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tzqjttme.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cphhvxqd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ytxxxrsb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xdukujle.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xkxhcjxk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rwuqfwsc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bukxhpnu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zatomsci.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2pnjxsgno.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2kgdngogq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2opttmjcz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ordvxtmy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2wlsbisdk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vehmljrh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xsdzagyf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kjptpluk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ceezljpd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kivobecg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wmkqhyrb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gtgeowgb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onpjmafy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqsftsda.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2geqmojcv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2wadbsfng.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2yyjyfqpq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2sfrlgcoi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aucghycl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xoiasxdt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zglmjcnq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2noabptfb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2snndgsuv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2sqewusrp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xheuvvff.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tgiovxvb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2nqhquobv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tqazzlkr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nkmofvnj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zcuzzube.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ybblzefq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wwycilxi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2gsidcahi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yzfbaphd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2migfhnhu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2btpbxnvv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ucrkutnf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2fuazkbjm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eqzgwyva.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ertuzbtv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pddgxrih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ggftpwrc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gtmsqwtt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2xakriapp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phbghuzc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zwppayic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uerxdkzu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yypjfkpg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fkienjls.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lzvbpsea.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dusqhpgs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pqbcsbsb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rrlgutkl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zilvntbm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2gzspwgxu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssfdfocl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xxjejqsl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kegyfoxf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kocyecwf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ohppufsa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kbfwtlbe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2aiongdmu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wbnhnuyy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ahdovdek.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dxjnzpct.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qitikaui.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2rnokfdbd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qonmhjcx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xkubjkya.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yppfafgo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2diskhxkr.html


<!-- 参考信息 -->