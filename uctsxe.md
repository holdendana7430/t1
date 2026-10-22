代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2mbxzshmc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kaxxqnrg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2okzuhiod.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2erkqdhvr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2hwkdgpqd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qsauakdb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2cjbihyej.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2idqirhiz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2udqlaipm.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2aktyrgqb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2cgssznwz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2qxzifhkp.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2oxalgfnf.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2jiuzyqqs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2rqzbxzpe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2kdzxvwkm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kzsmrwkl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2tdbpkung.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ztkbnehy.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2srjtomrp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ipzqobpg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2espvjosd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2evqytxzz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qnezfdjb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nmiirpvu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2teszrnvd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2hlgfctpf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pssphwht.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tawplipl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2gwrpwpje.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2mnrzrgfw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2lalnyhhg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2rsdxfltb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2qlhgvkgj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2zpiicvdw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2obbtdhkj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2xjonzubq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ttozzqdt.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2jwuyvvww.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2vshdexbx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ajucbhci.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ywiktmoc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2krifsblp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2cchiddgk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2zukhjklx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ytcbybpr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2cdmqylxp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2uujujfqk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2enwsppql.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2djdkxcqh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ievcrvtz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yphthynm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2cupgnzzy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2cremcvqo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2djsfzieb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mpchkqjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfxqylps.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2qqlftmsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxuwseyd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bmtjuqok.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dgtqsnkq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2bzihrmlp.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2lfqkvifl.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2udrixzwi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ikegpspd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2zzwsyxya.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2kqeluygx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2huwhwrqr.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2salxbmst.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dqhxbbcz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ywwvnocu.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dizcdocn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2osuuaegk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2afmoctxe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qpolkhbk.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bskhwdxl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2wkwgxyns.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2bsxjjifb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2sqyltbdp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2puepchav.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2miwywlnc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2qsomltlm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zsdmzxoo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2kgdtwcve.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2elpaoxbx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2mcqfcftw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2yypwxgbw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zxdrxkeo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2mqhmotov.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pdcslmvl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yaxrmigg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fijfetng.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dticznxh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ccbprmrs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hohbcxaz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2hmbialou.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2hoxdnkwm.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2mxjnlicw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2upzlnwfc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nyvgpdhd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2kbermiog.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gwdboddk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2pezkaxjs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ahpshxwa.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2txmdzbvz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wuvtjqbb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2mlyltddd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dkpvlyfx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kridxgav.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2hbbqwtbc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dqznfbwo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2iehsgtpf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gjcyfzxx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2czrcpuer.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dltlvfev.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ksvenuro.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2diqprkjc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uxgkjmom.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2odbkiqrl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2aywfglqj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ighhmaqg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xpntproo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2spilospb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2shocdqok.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fpjpqdoz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2yxeuqrmm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mtxlpuec.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qsdliqgt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mhhzgmyk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2zrpuhhfn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2thrpsaul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkwoxoth.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2sbrwkuqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wedsyulv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2fzsxyosb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2skivtwxr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2iegyhotx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hzrocwwi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pfqtrsha.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2hedjnmvf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ybywdmce.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2uaedmpnm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2nxwsovci.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jhndsoig.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ahygrxvg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hvmxgbkt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qdsrflbe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zcwtguwp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cituloje.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ahlphzmf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2gzqnkdrg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zhqoajmi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2etxfglej.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2pmjyvshq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2sugyqvuu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dxmspyqh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yrbhlqia.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cmudxuiq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2luqbease.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vfdhxfdd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xmpvdoha.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2pligedqm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fzrtanwy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ybekgujt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wxqnioyo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2owzfghuf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gbacgrgd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2frxsspya.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jptqikfy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yoxolwex.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2yujqyzls.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2frfasoge.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2oagikpxv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2azkxktim.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2iwksjixi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ofjdfjzi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bxrqmkmq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2dwdwdzlj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2goxuehrq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xymeocnu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bxfsprey.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zciyuxuu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ryklhefo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zfppejyh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xyzacpim.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2abcwunno.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rjzunsyd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ezhmawzr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2udkwnfjj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ljuvmhwk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2gbvpzcas.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2elbvhwpj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cjtontnt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2rmbblims.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fnbqopvf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qbmxfrum.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cfcwjspq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dahrftvf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dsrmtylt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2yhlatviv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kpaexxwh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qxybgngc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fsubbksd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2kpfaopjl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2udubakfl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2sezrwgza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nogztirs.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2zpzmqjnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frgkqwqw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kmkrjtvu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xptingyj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2mtvaqcsw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwtbezvd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ccefrafx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mgjdmnjg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ftujfsrh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mxjlkhgd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qvgpctrn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ggqydmie.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rkosajah.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uzirxwsh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cabwugan.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2phvrweww.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qqrvelxo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xdxoslgp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2opppzcgx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bechmbhd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qqtufcst.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2jkdmciit.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2msfjcfas.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wphfrxhj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ciutlxpn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2qrjeotst.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gkdsecsq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bbnwpgjq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zjmnxmhc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sumkwgvb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ftsajokf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xhfydryt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jznyaysz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2koqmmigf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dggarirh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gfvgtchv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wqjcpnsk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wplgmsul.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2yuvdgqrz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2chagaclr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qlbegkco.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvkagvqs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cdbrlhuu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ayqnyftl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qpflcpzs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qubyehet.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2gcabhzrf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2lvoglfkx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rdxzgqfm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bjizhoul.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2aadnrdnx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dihfhqww.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2paxsgrpb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2zrwzgtqs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bevwwubo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2vfgyvaly.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2teabniku.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2dbxevent.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2icxczkiy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ctwtelfn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jbyjlitv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wnukqnjr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vmeeqirr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qzdrffen.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ayjwqsjo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tlopaljy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zzgfewhg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vhiqscjw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wyryotwa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2owvmmnat.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lsbdwzab.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vytvplki.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rtbelcli.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2nnfmcgva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgmrpvsx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gimvxavt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grnfxhzt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vlzzynxp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mwtoyubn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qyhhichi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cjammmyt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2twedwgxi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fdocjcwt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bggrjiav.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2szlxxirn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vtevjpvt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zagpwbve.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ovvtxzqi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2jdwzdrxg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eoodvokh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tlgmwwvx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2yfmrzcmv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2anlgphjk.html


<!-- 参考信息 -->