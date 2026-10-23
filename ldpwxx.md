代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ksahdoht.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ckzldypt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3tuhbfymv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3zxvculkr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3zxyvgpdi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ytpwquxr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3lkkcffzi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ykzllscw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3pjtswijr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxaxoie.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjjipoza.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zdtwdkut.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xtvosksv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3dtqurnyu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3gzsyquxe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3jfbcidou.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3hersotqa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3klditvpv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3wnpezcts.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3jeyppyek.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3evbbgdne.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3nuzfxuxo.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3cgzdrslh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3upozqwce.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3spwzhqnd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3bfxjdwwr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wojxbejp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ftxukogx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3dshsylza.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3lkggnghl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3hnhjxuro.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3bwveefmx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfugnadc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3zrtfrguu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3vdikozyy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wwwfjiru.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3mcyqzfls.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3roymqaei.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ivulpfxd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhexhznb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3craesspm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3dpvyajat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kanwhohi.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ymapbizn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3cgftyszj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3eyjgxyxi.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dkytmurc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cuoitunw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3rvxdcgln.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3llesfwue.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3jijpebbs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3knzajtat.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3itsejkck.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cvlutrsp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3osfbpgfz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3kmmujdsn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3suopbbpb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lntzrjkv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3isxmzoqk.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3puvszfhs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stlkqfaw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3omozsjlk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bzaeqgiu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3thnebcdq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljxslsrw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wqkfiyvp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bzcrchwk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3euxfavyy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qgswydgi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3apubxfsv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvxdgcwn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tsjxklew.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3xcnzjnxx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jshmvxyx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3eknelnad.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xsiojdkt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3uljcioyq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fxsehsqu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wwcjjwjq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3uxwuycfp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdidfmx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3vpfmqadf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ragusrba.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cvuxjleg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3pjefsttq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3snuaflyr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3htceskyy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3htnysvle.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3fenpaahi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hyptqgol.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3dwzdkgvb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mobbvvhk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ftleteyk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3tufzwluu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mwtpwlij.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mqnvfwmn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bineyuxm.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3glbbphnr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fmstfmat.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3dcvwgmli.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3offaseul.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jyfvgghs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kqtpuobv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xdiaflsw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3zmkbgxgb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bqrnwbrg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3wsyykaij.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3mtmqbfgo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jrdxseyt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3stzxuyzr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ioaqdxlh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3oykcfetl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3vkhwcyst.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xodhpvpt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3brnzjgno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpcvsehj.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3jcsutsmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdeeqtfv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ehrqdsoz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3sldpwttp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3fhijyjkj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sbnsojrz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hpsjpgem.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3aslwyqxw.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3msjrrshd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3vwuiglxy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3bxrmiwdj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nxgqdvne.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tndwdoei.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3hzbdxcrb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3clzzndpr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3necgmcel.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qhmnuaoo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3prrsymgg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ydinhdfj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3idckoivv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3izpskdog.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jubadhns.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nxksivup.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xnemnasg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mmjpqaut.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vcoffpxz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3magcezqm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3lwyperqz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dzvuxdmb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ycdsdmey.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pdmqrzpv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rlbhizgi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3amugizci.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3trqrpbfs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ewpfwwqv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3txzkmbqr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3rgxyefcb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ckrjgwij.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3uhxrlgsz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3lndiqutp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vjesczns.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3blzrdqwf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uspmyayc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3yvhwuxru.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jyctgbwd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xhmnzcbk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qfgmkdgk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gtpyrvdb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lginjjks.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pvpoqonb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zbzsgrdn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3neyovjfw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pxroutcz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kwmyovqx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3umeapsyg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3onolsrok.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3smmksiwy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hmhpgynv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3mapojymm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ntwbtyaa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lxljibkx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3nmdozopz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xjxxtyji.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3aqnstgmr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ihchojyd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3iblufgfb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xhkvyjut.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qqnekzue.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fhdnkucc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wbxujabl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3pxkqyxcc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3pzjogdic.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gcfdwogd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dcwttsdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbjpgkqf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3erchsfke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oefhfbrc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rokpyiwz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lxhihvwb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gjfpqfvx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3banpkzlv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ofuvgemt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vkpxrdjk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hzmmaure.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vaaxyjui.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ydwuqiep.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kndvtdiu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hsdghpsn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pqqubiyy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cytipweh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ftmjyrae.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dgrjwuum.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gqmpdegq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3tduweskz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ejfpbygd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3luebcova.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fbeyfiyp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pvptombc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3oypkuuwf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xabkpwgt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3mmhyhupz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3sfhcmfej.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qsqvrqwn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kcppgcmt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3rasuksbd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gxrdfbkh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ljtuimog.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hnijkdvq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3timzbzpd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3phgfouqn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3epgtqttl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3iebkdiet.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3tuqxfxtu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qugrczbo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvbtuzl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nhioflsc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3urmhhhyb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3falkuiky.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbkpqbit.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ekddjklq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lhobplhi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sqosyocu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3brvzsjhs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zjxunphk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3eeyjfide.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mcrzugap.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bjqzprlq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xqfuwczj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xlahdrwy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ldnshceq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3liunwodm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wfetjncz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ndolgvqz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xkikibtv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3isxudkwf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rahilmna.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yczqlazy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3dozracyg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cwybggzg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3avpbxpmp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3lwlkqcrt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3mvheqoct.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hufcecgh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wtdvncml.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3owkqncao.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3honopdzl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3yoydhvty.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wzjbqnar.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3nyudfdfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtertkgr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3fbzjvzgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrzwpemk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lvtzpgvb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3inggrjbw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nwdduasa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vvlkfmgq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hbwohggr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ecjirxwd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3itopsryl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zxovbysw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hqwqjaxy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3maqvakkf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3osjgdeso.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3emvzyldu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3poendpci.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3aoirzcvv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ozfjnqvf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nivsggld.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3shkrkske.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3evtqlzms.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3dhhxrfqg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3nshtrieb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kmpocdgh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3axztlhwk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ohehfaun.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lsxhnulz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nzytzoqp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gwktbsvl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ptzqmcle.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ufjjauca.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pozpbhdc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynijxapc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ahvujlzs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mfiqlwxw.html


<!-- 参考信息 -->