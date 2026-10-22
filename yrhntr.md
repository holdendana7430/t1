代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2cjrifkwk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ouaipvcu.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2knzfjysh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ldctdbgg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2miyiqebp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rbfzbqqd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gkvxuwri.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bntquwdq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ejeuuqic.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2qujfuyvj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2puwjafhk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tkoypbkp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ozccetvj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2bnazkjnu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2qepnnhcx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ctkotgki.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2umqetmzc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2jkasgnhg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2djzcduph.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2gdxsmibb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2okiycpat.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ubfenaot.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2oqecopnf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2nwvbzqmu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2wdsjnjdo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2szmurmwk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2kzueoyjx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ikxethwz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2fnrpytxr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2yqajwcam.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2bgihmgvo.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2pxuismnr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqztkngi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2bmgidjow.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pimmrgvc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wedkswsr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gsoktdky.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rvhqcjau.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kaqlegjy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptfqqgko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myzyqouh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2rkngspom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajrgophk.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmzsyodg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2sssdbqav.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xvotycdm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ssigajpb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2alyzjxzb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2hmczirat.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nutoeyce.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2mymkvgwv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2agsnvzue.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2uikrcmym.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2vruzcvrd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2sprapeyi.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tfqvtsgl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mgilqfej.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2deymusya.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tbwlomtn.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tmnaceuy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2tvjgflir.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2bthwafll.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qarlwqbq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nrajxzkv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gtkmtzbj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mxkrgjrh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yhmwxvsp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2syhrsiiz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2mbozdorn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2igvfvyux.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2jckvnytd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gvduzfus.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ctipdeuo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2atycndux.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nvlnldoo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hzopeiod.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2khmlmtpg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zwbqgnfj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xoopsswo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2uavvesxz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jffuxhtj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gniytpqo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xzrudmns.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lehnxkam.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ulxvqtlo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2nzuzpfyy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2anpnhxkz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2opffnzey.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2endlcpvi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tmlllqjj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zclatcni.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jklphpsz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jjlnnvsu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2tirvmkks.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2oxgsgxbm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qxuvezjr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vrzjbuir.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2srfzhhdx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qclgmfdk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2oaiaolaw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dudinirk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rzdmhvla.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lzhldumq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zllyqdtg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hcefvcyz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rprcuypo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2njmwboad.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hsftkpfa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iwyvokmo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bdkamdtf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qseyfbez.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2dxzhrksv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2owprbedh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mwjxwtze.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ltyajtpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lovwuzan.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2yvhyodjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnxgnvdr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hcobqkzq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ivcvrife.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vxdnczrr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jwjfpclx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mzocvbpg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2iqajcfvp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2miyhgzmg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ocbncsqz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qtopredc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xshakfdt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xjmzpvez.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ggwxivwn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bmepluaw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2miuvbagh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rudigwqq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2dwouwgmk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2xkokpzzd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hakosect.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2lvvkcmek.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gthtuqsd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2orjpzcqr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ieojhesc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nrnwyqhh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zqnqqmrj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2arcbutuo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qxqhqktt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rdtwrdvk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2pbekccnw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2sejxosne.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2zgztygwo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ifyylvsh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2otcyfvoz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nkatwkkz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ibaxywve.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2offojhin.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xroqkvup.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hdsyhdnl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2stjycdoo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rzonnbbt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hwovotij.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dfcqkbqf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2kkroaror.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2yztuaoyq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2zhmmfhwl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wqjwnyhk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2rybuimqt.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uyeejxqj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wqbzcfsw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ruzmnmmd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wphibrxw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xkskqfmo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2acrkyjlz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jgvfguff.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kljgtxmj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2emufwqzt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2skskcylc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dlywvdya.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pdossfvy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zbslgnsi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2aqersblz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gxzrftjv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2kygbpmfj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pimlssrc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2plscniod.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zlahedez.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2zcrosewz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2affarzew.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wwrszmbt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2uxjlxuku.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2uevaqsji.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kglquzuu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nkbvmuhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2helrurnh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xatvwmgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olykhuxy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rwlseill.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2znzhzlfq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2aasptzrg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mofsfkza.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2salcltwg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lmthijrg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wanblaka.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ryydgeix.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hpljjhhe.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bhtdcdlw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xbdnefyb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2anejcmld.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rgjlbvya.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fagdnyxg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2novgnyia.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vvzfthov.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xkkksoxb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tgfqjmwr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2despvuhb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ightgjja.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wjomurmt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2amaovruk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ojkyiscr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ucxgmcmo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xmvxytad.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fsrcnypw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2otvdseyy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2wtopkaan.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pkgqenao.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pewcixlh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zmzufiet.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nvvwhzjx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fykholaa.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wzvncrck.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tzdcqlvk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2zwocjwuk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jfgtpkrj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kejcehfy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2dtkgpstx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2edtwgvto.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gbmcnnvw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tvifgpfb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkkdgvrc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2oryaapyo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pomodsns.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hmfidudg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fntnjsbo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ipneglab.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dzublvdj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2akwvbojf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bejqzihq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wpdvahck.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2tgwmdasc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2erwmyuxi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ciwftgnu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jrtewhrr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tnvykepj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tywjkfvj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2laukfabu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2onshkbol.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ksrwnlbf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ljekaujc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wuduzzit.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ahkbtext.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xgmfuuwi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2dmqcoicu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mibsgwmh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zkwjuiuo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xjwgconq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rjakzhta.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2vjnjvywl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ohzwfgvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2allxqjxs.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2vpqqnswq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvsbdxyz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wmxvzmbw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ystqfsmu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zqljjzre.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ddxylguq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pewrfzpc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ezmswlqt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gybtextd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fuvfwdai.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bcwijjdq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2kbohxqtj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zzpkjxwk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2qvvnjndk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kfkxgfdm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nrpkqaxw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ugzfrdyn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbgtzcvo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2moslhqob.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2znatyhve.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2bntakwbx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pzuhlfxa.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jwtqsnew.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2burrrsst.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vxjaajmh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2veiimnux.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ldxigdom.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2axpsfyou.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bkezbsja.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2xkmvpwhh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxfaiah.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldmdcuga.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jhrpozfi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qnnyqcqb.html


<!-- 参考信息 -->