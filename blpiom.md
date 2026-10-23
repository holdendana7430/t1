代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3jgisiydn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3judjcrgn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3qxewvzdk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3munyrgvx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3minufyyi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgrnzwsu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwqgbivt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rnaniclp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nxbcggtn.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3urtvghol.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3qxcpmpqm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3zthybnbj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3wzdydzsw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3agcaikft.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3snxmeult.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3wvojxxre.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3azqyxjxi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3cxjzarro.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3itowfjaq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3zokglhmz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3cekbmvpz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3zilcrafu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ixpetpzb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3veowjqpk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qkwjbmai.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3rocoxdxm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3huoxitdp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3aiimozyc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxlqqejg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3vlpkgfry.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gkswmkpy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hffmnvki.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ylgyeuao.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3suandhrs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3xztozncp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cmvnbxzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzhqgypn.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3zaalazvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ighdytqy.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3amjnjqsb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3smocyzil.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fxpeqaal.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kajirbrn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dznfkkmu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3oelhpxmr.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3afykuszs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ajffcqhy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3gsqcadum.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ydvdxate.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hzlfkcmi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qzmycmib.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utoreiep.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vccziosc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jxbqgfzd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qwcuuzkb.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lbdtynsg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ucmjdhzt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3wmkwofzr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jtzozpec.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ohwsdbnl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3codykqmy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3yfmcqrlq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3mjgwtxsj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3jvhqdxay.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3mwngsrrn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ywbjdtkt.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3gkqbabxy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3geqfwnka.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ljtvylah.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kujlftyb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ljcukxeb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zjmnjxto.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3heubeupz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lhrqvrel.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rjrdmzna.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3rvffbrjh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3saectrtz.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qjcujppl.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3srlthxpu.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tthcytkm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3qsyvgrpo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3daddxspk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3vrhgelxm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3tnnemmxe.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xnkzagkr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wvrhmpwb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3qqogitsx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jwxciulh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qqvihppb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pjimjxoh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qlrzdviz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kgcrvtnw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pygdnldr.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3elpvjgda.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ikqhyjdm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3igerxvel.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rqgvwqqi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gpzymgdm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hrhoadjo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3etdktjld.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3abtckfas.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dxloktut.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3chrcwjam.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3fdoclbkg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gbatxttc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3obclasqz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ahjuumgr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3skhebxdp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3skzaxzso.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3yzomouax.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3reecftfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhbfxhmt.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3dzivxaet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rilpctmn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3gujbnuaq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3rsxqswgh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3vnpaeuqv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hnpjtplo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3amquumng.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3evyuxgvg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dzgzwast.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3bsnafdge.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ntudjcyv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mnptrvci.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nacoklqv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vmbnvvge.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mfghicce.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pvozwzan.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ikeopfgc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mevftyyz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3zbrkispy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3knxtjmqt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zierlwbj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3rqinglvv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ajzvtldz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uzxbnzgt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3arugusbo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3xmzgzkfi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wvyjjnxc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3thmdihjl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vbvqeodo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3rfanxtds.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jbqykzsi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mtwfuxca.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rnmhuxek.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rxavgcnm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3bjelhxgm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3doxqpvpu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ucyoewko.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3urpnbvzi.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3lbatarlp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gvposvla.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3sgcbmdfi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3daehbses.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3orljobzo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3vsdzpghc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kfstolqx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3izvqsqzb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3honyitdc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cndbhihz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vkaufepj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ozfsyiui.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yxkiresk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kdgaibto.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eycvvuum.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bwoyijlq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3nlbwhqhf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gixmdetf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vzvvmphz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3fyzafhjt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gjmsragu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qsjyvlkg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3whvvoxvq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3rfnxveer.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rvdborzf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nqpmezrc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3txhfcjlb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3mtdlanpk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mpefxlip.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jkfdldqu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iuxnupau.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aqibzqzw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mzwcrldo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rvvbfebn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3icvuvcdg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3abbmdbwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzisvqcj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ommgnoqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxfwqbdn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xaafhcgc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pvfoptur.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3oecsynyh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3affhswvm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxhmdwxv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kkfjkkca.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3iqtqtvvb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tmstqcvp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3woqagnsc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zogvdert.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zvvgbhmc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3iigmccbx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mjsotcvw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lxqujrbf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iheqtfvz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nqfclmwd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3shklsdrm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zjlryuqo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3drjzfnyk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3acljbinc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qhzmpnjw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tiejqlyr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zfuayouf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xmfcaonp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qvuoynfe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ypnxsory.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jdmvomud.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3kkahtuxd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3smbxkdnm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3equdbwvw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gzvapwpy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3buexgvgq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xrgzgnfb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ahpfneha.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mkejjaoc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3szggrbje.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3yujxppuu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hfycjbsw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cduchnji.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3erbprvix.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvfavril.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3grpfzxfq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tzrwobom.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3goafbtgg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ixhjxdux.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3isicehyo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3evwexyvk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hzxofqvo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wafejnda.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zbgpsxfp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hcqkyrpa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rpxzraan.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3zledzfnq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jmwygfme.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ofycvpey.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3pfyulbyy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qkbtttty.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3upcjlxxx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bcynuvdu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ibmqpxqk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vmckgfqr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cpdthzfa.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rmnlnimd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3aewiavdl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3mdgkzizh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vpcvqhof.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zeztbajq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bgyyyglf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3lbbvtcmy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ozcjuowf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3nkyywgct.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3uzhsrqwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbxyvvcn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dvxgksau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pialdjxo.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cuomojgw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jhggjelb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ndyghuff.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qlbqftja.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wqrhkbbz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsvvszgn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xseggnsq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ngsrqvca.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzeegzpm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3irbeyzsv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cofucgyb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cuslrxcl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nltibmpo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3oasulyzx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qrhcgvic.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gjtaxaek.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gctknaaq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3umdzqdwb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3piaivzbb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dcweusrn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3hwarapap.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lisjaqlf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fkdbjtfy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cjlndroc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hjqmeszm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3anpqsssj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mldfwvhq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3pazojmqa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lgbucbli.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhmdgaxr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fylzqcrf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3csjtgfvi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mnkklylr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kwwtqngd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hghqvcui.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tutwqwyv.html


<!-- 参考信息 -->