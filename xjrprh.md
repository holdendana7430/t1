代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2cazxyzvb.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2mcrvrtnr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ewpulwvs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2hlkqzyga.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2iyvtiron.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2fkdgzxfk.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2cskeqjtb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wubdcldn.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2gipglmwa.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fiyjrnql.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2iircapla.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2yygrbukt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jpnmorxn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouwzlsjm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rotdvqvk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2danjwkiq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cggokkng.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2qfddkhrv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2pkuoqobl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2lwrnkqmz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2dkxplbki.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2stybnrpk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2awlpdzko.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2iaohwfqc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2iyfmorbm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2oldwlwnd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2fsdnfycc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2bbefxtmc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2jprjhqkf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2unpmzcdw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wltoluob.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ofmiwcbt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2smtvlxvq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2emrcxrle.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2xzhmwxdi.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2izmgmqrx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2etrbvtwf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2hmetndpg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2piyfkkvd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bcplyowf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2iywxbqlm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jdcyhcsw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2iojubvnc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qubbnplh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjurahnz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2oxascmho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2maoterxu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fcrsujqt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2eufpxzhc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2icyssicw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2addbqdmk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pycsefhv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2htvympin.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rrdydubi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2lecdhziw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dmihibps.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ibvbvyxw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xuheaqok.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2msqihkzt.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2pwbpnqqr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uwlfsbce.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ljzvfqlr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2kxtydcdi.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lptxulvq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwrdxryd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2osmbchie.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wlyvueot.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hfrwpoiv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2udagarku.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2iehopssp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ezlrrres.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2dqwcdlyn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2nuvtaohx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2otvnfqjh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2moerayqj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xhvytdkg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2sxkpsawm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2idzdykvh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lxexnakz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mjjahvne.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wnucznlq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hnrzrzyd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xeukxpys.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2qaourtvo.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2xqscpshy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2bjnnugmx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rofakfwp.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bjrftsmu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2xcagmbon.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2hsbnylah.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bkgrmbek.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2bmubgdco.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ajptpvzj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gfiyzkdb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jcwfxgew.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ittwkdwd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2sgkbkqxu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vvnscjod.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kzbbcnvl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zbkxghyq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2egsvhbpv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2rhhlvcgg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2glsbaill.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2vbtdfpem.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nqyuqker.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uwsnzqej.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wnziyasu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2enfmnsfk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zfdgsago.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hrqycnbb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2gnhwtnbn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2btqrzwyo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2frxdgejz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2djjujfbv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qrpjuxer.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2scoajszk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dvshzslo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2lqmvxlna.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2isctkqzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwcnfkxp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2mcfgmcun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgdspnqo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2wgkdmvvv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2pigtqzdi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2bbuxddcv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qbleruez.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2njavcyxx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2nssoebqt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hbywoait.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2guuedqmx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vmdpwtur.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iirkohzm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rgqvpozb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2acburorq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ohrjclea.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wfjpquik.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cssnydjf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2mejslerd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2wjelutyo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yujhkpiq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2zjqymuuu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qnhjzute.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jqytizka.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ysmgbejk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mldwxmzm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xavmhxaz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zwscwkvh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2qcuausqr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wuofqgne.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2sznycsrh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2aaclzghp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cjzwuuxp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ldfhrkuu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2grlzeujg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2gcdkjibc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2pvmczjzp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2litauend.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jwiletro.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2lbovynwx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2bftpxzfs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2nwwoadwz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cisyikld.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lqyjpvbq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2tjmmkaqc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2eakketes.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2txxzphmj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fkorlzmr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2dzrhqirx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2afwubyqj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2pjhssdll.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aeoxqcxs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2raptguel.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2idbwfyuw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2aymkerlg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2kkpdliyv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nilnixxs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hsyoihge.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rzcmxgbi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2wjybfycz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jxijbjec.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bxmiptcj.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2rvqmauvk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vluvrhry.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wxisbeso.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tayifdfg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2gunbvetm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2tcyjxiix.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ystqhkxd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fuwgzwss.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ejicjnbp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zhskujkh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2sficauzz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nhroyjxz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2emrlyaqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czdastdm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dysywlzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysaxblnt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2delbvddd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wlxfvssq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2nkrvttkx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sureligo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qhbyppbm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uziqktia.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lymiekij.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2udzbxaeu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gpgpkfes.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zftudofb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eezqovbu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fsmkvqev.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ksqhmzba.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2khskxvra.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pvgtntot.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2emktcutk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kdgmbihz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mupguwpi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2asdbobmp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xfonywkx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2vsxpsuwv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iigwetqi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eaqvesry.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2uqjajmmd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2emnerjvp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hgdcrgjp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2tkniuvcn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2cxjpbrwn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2atkwctpk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2dtdyqpoi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2smudqutr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wstjnifj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2kqunqnee.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2wnpmgrda.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jxoapufo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2myormuwj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fakvzbai.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vopkqsbr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xsonqrrn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xinfrkll.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ubntyxpc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2imxbuaou.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdimrkrs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rvggrwdu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ikbkohxz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2womycvkb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cpffugbz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jrhfojcj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hjfirucm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ueetdzib.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ctvycncs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fsomgzxq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ywrpymmb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2yryigdsl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2elgwwpnm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2syhfcybg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ivawpylu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nsnjxsfx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2edowgazh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ggliwbrn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xqfilqgx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ivlfvvzl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mdauimib.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2gunhdkvv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yfgnayjk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zkllgtbi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2liabmveg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2blzvwutr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ldafhfvy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2isnkoknh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hezdzkze.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rujjwnid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzfwvtuf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bvumzpsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sletcoan.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2iwbikfhp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgjibqfh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ttthcjgw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wbdmfszd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vxiqtmfo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ubvtajeo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2furebgrd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2btbzinea.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sjfezujs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mhnlnkki.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hbkcywwy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cwpqfeet.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xgzlrnyt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nzrgludi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2pmbxaxtp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lvdqpskf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tlkhbock.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rlmzeuut.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fqfivmeb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gbgmmmqr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fijtveke.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xqbyxuph.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yhzqcohv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qhhlaknj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2bumgvbcu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wsanrbhc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ctmafyww.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2crjbefad.html


<!-- 参考信息 -->