代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2xkkjvbla.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kcsrxmbu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2bniifaer.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ftbxnmkc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2xexygtwe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2abckfyxl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2usxtlclr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jgwlausy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2nwbyphqp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2pkbgqpox.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tzifoqit.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2zzfalfwr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2llsfchph.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2gwcclpbr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2auvlwgof.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2qvwgealb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ppgttaqx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2bjytjryi.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2xutdynjf.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2zhhhlkjj.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2yzjjslsj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bovjliab.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2mlhiudll.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2onyuqjas.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hsdewrrk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2dsqsbuxg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bmjlzuzl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wihvujii.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2khlyiosh.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2lloqdzjo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2mmvkzldp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2rvneqtbq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2seeoafke.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2qmjfcnej.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2posyocgc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2hcouwort.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2wlqtjwcx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2aqqfdqqd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2kwjuqjli.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2snqlieyp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2meqdhyhi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2zxmlicnb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2homkejfr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2vhevixcb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2kkybedfy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2anjcswbq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2lacjjxid.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qwypbfom.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2bfdnfrsi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2azajmuxt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kdkhurit.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cpuptwak.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2vqadomga.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2oovzccsq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ficztitf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ueiefdmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnpgwvrv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2zzacvnrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmtzfnxt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2lwzecptd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mwlvtsaz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fozogcyg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hibwkoym.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2figpyfdt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2mxxikubx.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nixgrkwu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2khrygrwv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2deyqpjkq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2nyjocbmz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2wtloxsyy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zqonzyku.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fsdlvazo.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kqoowtxa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wiqdmwgm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2opymkacm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sjraasvf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hztrbcik.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2itzjfahc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2oerodrpp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2stilgysz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gazufpeo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2dryiaydd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqsmcpys.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2pngapbrs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xofcjwru.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2okalbmzx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ykwmnuig.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bstvojzd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2huzgtrms.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xzmwjsqy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mkyjjrao.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pzqlhiqc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lzgqtuck.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kwjwkwzv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2unkjrdko.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ubunpwkp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2axchwbsd.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2bcqrtdqi.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2anrxxomf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zcafqath.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ehoopmfw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2khbdojxp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2fymynnds.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ecpneigo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2antzypqx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rvathlch.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2kvpodmlo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rzgzxsxk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ijfnfpit.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bvmfabsv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2acsgurrc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sprzwykz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jwocifzi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2qvtrdqkk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rklkeorz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2soalscps.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ybsyczxi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vdezjzva.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lhawizup.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2glfsnjfj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrrymnr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2clbyohfj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2triosyht.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2pkcyseuw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aovainrq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zldwliwy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kirdchhp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2fimskhcf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2wbgbvhfi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2zqdnghih.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rwlrgsxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wochptgw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2kazpuqni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcjilpjw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2fhrhowkd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2guczebib.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2llwtpgbl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uftfqugi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zskczztw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2brxebhjl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cxdbrrtf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rgryslny.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dpkoaerh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xiiluidd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2yygvfqkg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jwufdxnc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rbucskvd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nuyeouok.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2pgabmzjg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2uexliwid.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2bgamtudv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2pkobcqfc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2qspxfvzc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2cdzgrmfi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xopvijnu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gylwnndi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hfsrxvmo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2tsthzufd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gawuwsbp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2rmupoqra.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dylnzwao.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2dartzirx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qtvuppdi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2oghybpfl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qryvytce.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pluoipld.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wslopmpb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2yvqrinfs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gfuajbbi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2npgrhebc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2srbvubhi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2bkgjxaxk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wkkcxosb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2irsnwxlj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ozrdmerw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2pfzlngeh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnkotorw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2flbuzqeh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ycddajtv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2shamowqt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tkfdohvj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wvepvyio.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ubfpgfam.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2piaidooy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hvikbzbt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rywqctry.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2btlpdmxg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2pwnoglau.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bwcgnevk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gizdanqt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lbjvdobq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vwerrjrx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nnrjobrv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2prkvldsd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nvczobhs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wmjxznit.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oltnzsuq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2agmllnan.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2nuvjgkpn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2guiivxtj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lunyhnqg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fkmiabyo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2aylzaxcm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2huarpwhd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fpowogvk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2defbcqit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rypxxtqo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vzauidxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfxouayb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jovvydnb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2arpzcsop.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ubiaihrv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldpdmmin.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gbtooguk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zgqxuvqt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rxbltqwa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2uftpyfgg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yewzharg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vucwijwf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2saroathy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2skiginvf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2huwhpqtr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2syhexjxj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nytoodqx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2otgldnyz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2qftferpj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vycwzgtr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ypxertuc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pujoflor.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fxebarag.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hwurxsmt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xbuuquqo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ohpcflou.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pfhugmmx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tqlpowgy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ywjovukn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hfnougbc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2yykifdak.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2unzicgqh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cpbrijdw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zopijynd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fhbvoapo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2velwhrmi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2joighrgb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xqgimsoo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qfadltxi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lahcmapx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2alfxtfcv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onkycpkz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wbnosvbw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vlpgjjaz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pjxtuxjw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2anckhgty.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tzyfnsvf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qgvhdnnw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zlarhqen.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2icvsfnzh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lbhogbra.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ghelmfsg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xqefjeta.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2sxzcevla.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xsuuicmz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2vvhdvsrc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ggiclcpr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2yrrdncvf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2uluevvyq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ckufdhau.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ncpawsyq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vzzoxoxb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tyjbhyfg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zhvtiric.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nknwumcv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mignvnhq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2uwakuvtz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2iyujgqgm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ijutodqe.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yqywqypf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ngqpkyrs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jumiwymh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kmpoupvg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ouvgfakk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aiozewme.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hnyjromb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juuezrfo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pxgxhhmk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kperwrdy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xlgwrcxz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2imifsjgv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nlsrjbuv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wglrjgqj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kecqzvbw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gwuqpcih.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uagqjaph.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gyiwdlrd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ecxetqts.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lajicdfp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2stkcomxp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sgdlqoth.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uzykuuzr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ksykvdxl.html


<!-- 参考信息 -->