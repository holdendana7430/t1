代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lelmzasy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ipjljord.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3yyltfblg.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3duuqmpry.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3olcsiqxx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3psflfhzo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3dluljebr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3oolzflzz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3kviddviu.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3yiomlyvv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3dycrdvsl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3jpgunfbe.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3nzvynifa.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ucvvapnv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3khxcuswt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3bftsoamy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3aafzlgqb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3fxgipxwo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkfybopt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3utitwozh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rkgeiknc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3aackelsb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3hbnmmhho.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3cdsljnii.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3boyvwsuk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3hbkqvkmr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3gfvbthvl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3laidevhq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3nxcniipy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3bwvtbzft.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3tmodamcd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3wgltsxhc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3bzflzxso.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3pnubbrkw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ozfwdnil.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3qhpcqsac.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3adouiukh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3blzpzuyt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3xrpevgqd.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ttsulljv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3efcsfpiq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ieqybjtv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3aaalnhcd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ogefyulv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3zrpweuui.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3iyxoyzmu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3sdonylwi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ysukzfaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3teekursv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ospmprcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnshxkep.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3tscteojl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wcwzekdd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3llcfjisw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3fdhsswlt.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hbxmpjnn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3xijlyyew.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hsjsbnpe.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3lvbgmovr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sgdwveoj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3sggifaix.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsbuhcyg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3grnmntyi.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zrsmgqjf.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tsyhcdsv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ldftdluc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3znfcdyjj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xwthhfzh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dfnckucg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3bfkdiwlz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3uhvfytda.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3aanwiaiu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fcahfltn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sqlretan.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qixyweis.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3jsqlhgfq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lenbvxil.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3imefvsie.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3gvauplgw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3oydqjzlv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3plgnzbod.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3iicxarvd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mpmuzybe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xhduazcu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ofoxykgd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3libfyisa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3laiurzcd.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ddscbhmy.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tjsqhsuh.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3veblrzrl.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3giifzjsm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ltsvmqjv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zhtybwgd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ouwwomkr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3bwpapnwv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3dgjlrzhn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3wuuzexcc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wabgezhr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ydgngfyf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gxroryvg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kvadqvdq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3kynozvxu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pxeskwmg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cjpfeukg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3idobtciy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3dfllrrry.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qxkwbmrn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3exugzzgx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hatifiah.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ciicevse.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zwkyxosh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3iqxlmewc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ruirhxgc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3duuoowrm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3rzlrmzlx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3gopjxdse.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3dnltctrm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dmxhsibm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ezdfwady.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zhgvmxzj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3fhtxoync.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kyzzxhir.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zmkmjckn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojgbmptf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3waqetghp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrsnamzg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3kpymezgc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3uokwdaap.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3zlcndaqw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lpgtwdqi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wfqhsypy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3serfugbe.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3lvtwxrji.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3pjemweil.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yxeikgck.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3anjqdnpf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nxbwyeha.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3xlcjfozj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jojodujt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3clbcpqnu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zwfnpeym.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3isopgocc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3knzywhfi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bdcatnmc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3qpjuqzyd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3oefrfbeh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3whfxghvv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3slejfkvl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pkuagalk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3aluwpoqz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dtshnblt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3rcplmzyt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tyclqdvw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zkgmmosv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hxqpxatn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ruwgbchl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ivvhmlmi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vxsjuvaw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vjsfjgag.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3bcwaamhz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tmovjmvk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ohvcnfhi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vxkvsxhe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3aqujbrsk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3nrdxgcrj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ewhkwkms.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ywblqkel.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jngfvsxe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtkaqazd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3axiejrwl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qohomzeq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qfefrczy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cbgyvtop.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vaeczppa.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3thsyprqw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cssluvmc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gxmouoxh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3oxinzqym.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qnvfjoba.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lfftbmcp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ojifkwmu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tjpqpxiw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3tqedobuz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3iiyyaydi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3upmqtdyj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fqikfjik.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yhqcqwsr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3spxwhyni.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3itodgfri.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3irndtrsk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3obupcrvc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3nudeelnf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qzzwatwk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hyvhuene.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dfnomlyb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hfpocuoh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3snwbyxmw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wnxrojns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxpiouvc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mxpvmigt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypointzy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vwxbvbxg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wtoaiooa.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rurxkxri.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3prxtibnm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulydgzkc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lmzikxyl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vztnvpfp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3npprvghg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3oqzphqvp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eezsptge.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dkkskeym.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gjiejvfj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kshcnssy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qzjqmirj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lsdbdlfm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lxyqbaae.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3slnetxli.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rfzsfekc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zrtdoodz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ipycuwmu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3obnblheg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cjezoqag.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jqtwcxda.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fafuwhrt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3exlzlveu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fndcegmz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lsxsmkne.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ccqdgdch.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dtgbkloh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3fzbekbsl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zbdgqqfk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vejmvtwd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3kqqukgrf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lxssistz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3pmruyfxn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tvjngkzi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3erutygje.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rsljrgju.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bssdorvp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3czlgfxhz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rswsbjbs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3harmmmbe.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3icfbctua.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ckpcutgv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3yoouotmv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3toxfdhbm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjpkplae.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vusbmvvr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cfnmiogp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mqphpixj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ecdyvhsd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3aofbianc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3asdtozmy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3sdgjilwb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zgsgxspo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vtvgzkek.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dovzfyvo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tnbjwwnb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pvptsxdq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3othdwsay.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3biuzzcgi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wnyzlqpn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dvvcxlfw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ltmhgssn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qjyolacs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3efdqfnis.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vlnfehoo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mfxgxpbw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xsuzwvlf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rlfrjply.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3eglohmqx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dcszfcij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwauvrdx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3msukfvbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofatmuww.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3smvaswfz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxematwy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ozrzzcla.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lwntwtvb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ksjbjzcr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lmvcclxc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lignrzkl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3bocxtmbh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3meyenumf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wlxeieiz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3feilmcrl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jmkpusdd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ysmnmrtv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sjgihzro.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ncnetppk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ytsssyae.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fjfledgm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bsrnsrpp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3axarsntk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3mctinxtj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jtqyiimu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dcmbdqsi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yewckytl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vjioccci.html


<!-- 参考信息 -->