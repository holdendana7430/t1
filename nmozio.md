代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3zdphdxet.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3mvzdjyud.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3xzidyyci.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3cctoadfj.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3dfpmurml.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jmpuomho.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3themcbxj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3xknzrujp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3icswaddr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3xqqttusf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3lvgqfsay.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dwvxfqrj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3kznhetfq.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3xhlmippw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3oensguya.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3fkvhgeer.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3izbphoyx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3mdxtrqcq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3oducyvil.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3uhytilac.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3fzgfegoh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3rcjgaixm.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3qapilswv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3xbrhletw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3adfexgoq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ikhkwxyd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3iwlxsksk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjqpucp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3afdfzcaz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3rlsgjnde.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3jzlxiega.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3zsvneupm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3tednddot.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3vmuikkfi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3jzcfbvng.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qgxoccci.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlbsrfbu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3rkjjibjm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3kdgalayv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3refftixa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xeoamlxa.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3gxswdjxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbwleiem.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3gthkjejz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3dietubby.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pkdumjfw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3klulsoui.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rphgoxwt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3fydgadvw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjpxwbf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3lcglukhc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ngxdsiod.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3iewnkrth.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3wksredxd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3uzwucqlg.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3moemryar.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tbshhxrh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nfpioopm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qgudqgdc.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xdpexead.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bovisqfp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3wyxnzbvb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3uaqofieu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hkpylsrd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wkbyexri.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxczmgd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tswtmmxc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3amnoumtq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ocinfxwb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3hrjmuhmw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsnxsfir.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3pwthbtdf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3nedukada.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3exeolkpr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3laaivxgj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uawalqfo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dqrhvczm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3swonydvg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mgbcskaf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3fqcnogci.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3heclcvvl.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3fwkjjgea.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pixubwpw.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3stugknlz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ysgzccro.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3mmbqhujf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hnwbchvp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3gbkgneva.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3alodkouw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kxwerkhq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3aerjzbaa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rpkgeluc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3htegjojo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3oihavgzg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3iumrqhch.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nmpdiucf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wtbxdvfs.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3epnsfigx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hwwpqmsm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ynaxblph.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uvzfouqt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dkisavbl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mlvejayx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wiqribqe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qkugkxcy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tkklklvc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ucautauf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3dalftrjx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3jxbnooyw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3uryqqmdu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ejnlezfd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ebsjlohu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3oetbsqsu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3hdsdymnr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3njkazqos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oruoblse.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3siwtuhjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tpkxjruc.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3agysxlkh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3gbhfbolf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3aesufkco.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3doiojbci.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ukivqwxv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3kvutiady.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pyxxtnbw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3uheysaxl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jybnrlsa.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3prbfhphv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3fqkjuwtt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3frpxseoh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dnoqcjsx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3sngltenc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3sfjhbery.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3rlpxgbhx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3rcllafvt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ivjnkreg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zfgsjssr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fzzextmu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3keqzpryx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3eukedsow.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pxwtakrn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3pxwdzhnu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mdzmrojd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3acuclsrv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cmhmibre.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3xpxwvxnw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdtymmb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wjseyits.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tdmscios.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3htbwjrth.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wxxxovut.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3titazscg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3fegbimuy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3nuzzusft.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wtdousie.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3iftihhpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3byuzihxx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zzubtaek.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3crqvhuze.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3qvvvxaiq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqgsvyie.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3cwtuzdkb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gwhutkzf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pylcocnz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zhckqjyu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mbmbeqzd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sxvmfwyu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ubfieizj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3elheoyle.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rmagmivv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3gjewmysh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3qevtydoy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mpaoqard.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ehexvgdu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3tkzprjxl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qgudlugp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cqmrnour.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pncmqsqh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pvcpwcyw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3hnisburw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mgulzexn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3iqqvskiv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3bdonzbxc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3lhmefecf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3okvcjika.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lppoqwof.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ibrjglzc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3flqnzwpf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rpfvukil.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gmyhajwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrpxoexh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rxbdmjbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlpemnfi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hnxjeplo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ccjadcak.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mrbvzkbg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3loccfvdf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqpwzemu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ptmytbch.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3apgoxadn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3htzvvrju.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3newgetrd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3riotkpif.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gsijaiqk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dknhnjkk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ecejphlq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yxdcfage.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qrcqhvhi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fxgfzbgc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mgkqhohp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oonpesrd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lhsnzyic.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qgodxszv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ckcjfxkx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nkwgayiy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wqpuyuna.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ftokwbsi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3htthsgwm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3uiplsoul.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wgyqbkzn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3pamimxii.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iexjbhjb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ugomgnqp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uvsxqfha.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kopvfqjm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3sysjpbpu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3glipcalk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3itmdzuzk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dxxaitqi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hysnlfsh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gvhdiiqi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3iihsapid.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ciixfjqr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzdnusmb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aiukozuq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iswylkqw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3pbflfknf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vzgmnuot.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3piapkogg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cxgdyedx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3grmdnfeo.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zomvmotm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ukpbazji.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ehlstlah.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3rwnzcyeh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kbsulaat.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3snckqhlc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qxgfeisr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3oqgiylwk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kxuqmlwg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ayoueyda.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rezfyitf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3oerxiinc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dbgamqsk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ykgsmvdu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3atoauzth.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3gszjgxls.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3tbccxuqn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fqugbkgi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3sjxpouio.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pkccvezp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3svgdwygc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3yvkvnizk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rgyvpqyb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lbomdgba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhsqlehx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wtibhclp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtliumjt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3asfjcvsb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ibbqomeo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zltpfasd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aqqnhsbd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bctvdbnf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yynbtnqg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xmwgouin.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xmhxgaht.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bzntikgg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3udmqlgjs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3emycqtkk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nztborvp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eutlqosz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vgdlyakx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qbymkopo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3scapcejy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3enjndcoa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wuieayzx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3sgfdznsu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3fescpans.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gvyyserr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mvxgmcai.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fuenxmru.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3unjzsamw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nsdngqfl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ddhiquot.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ylgfesjl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3hbprdkdc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qjjmsdsq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wbbruuzi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jnbhklll.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nnsbrkjq.html


<!-- 参考信息 -->