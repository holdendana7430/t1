代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3gcjgxeqc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3eehtbcuf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3plexxwht.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3kctbhefy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3xrdzhami.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3anclwmja.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ondmgosq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3geivcyiz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ndnymall.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3gmttxbft.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3okrxcadn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3hwvkrbds.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ppzcsdzv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3jcxwhnnr.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wlzkqofh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3blndbfwb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3spepgzmk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fvqqqzqh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3xatcnvzw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3dzgwavtf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mrjwcirg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3wycumlar.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ifylikxz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bclleyhv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dfvfwvrs.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3bstukuua.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3lxerkszp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3xokkxevk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3mwcznfpq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3mlhquomi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3weckrtuq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3iytdacdf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3vyxylrio.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3yhgfwpor.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ekhwwpqc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3hpfzycea.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3wclsodsx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3meunpvxu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3lcgyukxy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3stnynlqx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3fffsckab.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3yiejieyx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3pncozyoq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3agtfboie.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3vsygcens.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ufsdwoue.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3eaflpjku.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3truroonh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvvisvdk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3vqthzrkm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3bfckjmmv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3dovyaywm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljrwrioi.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jdnztfxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcbbudpd.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3yidmrsad.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qmendjlk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gbgcpnfs.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gotyjgqn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kdrbehuw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3yzlqbftf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3yuzmkojp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3tbleueys.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3shahpkwa.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3pkgnxmni.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwuvfvam.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3kzmbfamh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ievrtmhh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iihtlkbb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wdvjeanb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qtlzoklm.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bffngndv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3klkayxoa.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3bgcxwwpv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3gvepsokc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nonjiish.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bfosoxdp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqhnebfj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ustgfjvg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3jpmwfcyt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3hgbmhghq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3eqimlpqx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3lhprgohr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hxjyjsmk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3xiawrowl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vxnploxe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3iibzhqav.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zitqdazg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jgqdxdsm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3rvojpvao.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dzprudrm.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3zqnzpwxm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3cbqekprm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3grltjdqn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fqhfuqwd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3olqyygno.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3azqrhaqo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3xttyfhlx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bsbcrsim.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3pphciyup.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3lptdkkrb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lbbkkowu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gqoryved.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mnpzzlmq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dvxzhxzt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qfrrnkep.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lfnrevsd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ulmpadyy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uwmncvhy.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ajrckkay.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qklmueqo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hvkiugpu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vyojrcib.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vdfsylta.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pioaqsld.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jjjjribo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ndkieifw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mwhwwrmo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3tuxcstch.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wsktqlzv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjmkdkda.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fewvrcpu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cnoxaees.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3hixinroy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3rqfjnkah.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cmtjfdiy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tdrvydou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3heuiqwjf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3cttopsxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dttttdva.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3wmhcmfwq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ktjxnjez.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3fntcbnne.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qvmrxira.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yvhidhwr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3tuiztznd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3bvuqgnzn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3gvnsnxgp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uarlxhhv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3euetpoki.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rpfregau.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3apggigwx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wibmyrkk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3owhfmoii.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3mxljzuzf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3photallp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3uabzxrhl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bjpbyhvn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qsttdlpz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3mwvypdqg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pmlgjehh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3heuvhcze.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3alybgwjg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hszhgiqm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wqjzoecl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3qvbnuugb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dxjjsohy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3pobwapjj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3muyqxcbe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tttpgsaa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gilxvldr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3knvbdmhr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qbjtqjjo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3dkxrretr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3kdluizhi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bvelxnjq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3lxzcfvbi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3wmmblquh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ddfxrnjm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zzxdzijy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wnqdqhrz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hsqihzsz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqmdlvpj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ndptbuug.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fkomygby.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qpefuwgp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lfdxlfjs.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3kqsbkxjr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xatjcbxo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zmzyqpss.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3duvbbfsx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3fwjdmvmr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qmzogelk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gnoptwkx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ihvbjkjf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jlxzgawl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3leuvqeis.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ajbmmlfu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ifvumnbg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fnchhohw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gpsgxalt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kvaijtuk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3clftvalr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lkonwdta.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3dbabqiib.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3znrixksb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ioeqecqn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3novkjkwj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mndjsigk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3uatozfig.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3iihnreqj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fsaoglib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcqgkqyg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3leyepjzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxaftkor.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vsbfbcti.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qlqicahy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3vaqznwuu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3draqedpj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgfuapgh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3esdjgsgo.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3nqdbmcco.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3coyznrjg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tdcbklnp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tklsdcdx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ppvswaza.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vluzized.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3moycwqtm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sjmsmxxu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3csrtvidx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nbxohufu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vefrwmmn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kwsisjjv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3eetvutxo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hxqgfrik.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3uhlfnbbe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gspeqgyf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xlvtecbj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rqbbznqs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zrnjzrbo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vjbslzqc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jrjrbvgv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3cscoanmx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dibjqkek.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bzhaqoed.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dpyifoxp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3urhnaavb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kjiuhjui.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jhumqjdb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3lbovypmf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rhylnjcm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3cffqajya.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yuvojpiv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3njelofkv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tkebulza.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3svesguiw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3geuyyqvn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fqqltxpo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3okjpmgjp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wxbxvmyr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3zljmtnqg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ktdtxdbn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gpodagyg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ikglopda.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sagyckrl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ytuwrmrr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qmxrsjit.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ghqifksl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3edrdtjhe.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qfwxjity.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xbicrmmj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kthmulbm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3arktnixt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ffwaxwil.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pizzeexy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rmcdjtaa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rlbqnhsm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3aorlnwvn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3dvkspbze.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3klnmtfga.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fsoskhfy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fekqmibn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mrslzzgf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3sdkyzktv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3sjnejota.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3bukrorln.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dkcbvwxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzringxd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3twoxpgae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjxmpcwf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tvsrdvwg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nfslglle.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yputbjqo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eofehmay.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jdrwuglr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3drswlnbe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3umracwlh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mizoqixp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mwuvedlw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3qftmovvd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mdhguseh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cfsvmfqy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dqphahsg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3otxpagij.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gsqricch.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dmeokvzk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xphbzzze.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hwutsise.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3oojwuviw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wvotltcl.html


<!-- 参考信息 -->