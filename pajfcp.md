代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bajaemxz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2unoaaprh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ptsjeubz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2rxxbdqar.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ixkggmji.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2sznvzfmz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2puaeqadf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2hdfvqjrj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2oadxrytl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ebugnlru.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2oebalwsh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2aysahcsj.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ebmpdatr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2einxpqmg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2rijnmend.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ehkbbqhx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ucwsoykj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2esdbunhm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2oiigsuwd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2iekhmhno.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lusowjqd.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2itgllgoq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2xvmafezy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2dbjuvdgw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2uvrewplb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2najuuwgy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2mvbprkyb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2tlgcfnei.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2dmfiedfj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2qqlooozq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2rhiaeqfj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2wpcgoxbd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2zyrujozu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qvosjrvo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bmgfybuu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rabyasyw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2homukzwu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2otorldnq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2xsuyxiou.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2sbgoilkz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2qdkurchw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2kyojkkgd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvcymmev.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kkcpdwte.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjnupaud.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2xecfcclf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2knrzxibv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrrsnuvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjhnelek.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2zeifkzyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyalvjrp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iabvwrgu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wgquunlc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mbcgruum.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gdegcppd.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2nvxbgpik.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2cbrjphyc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2kcoxptje.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2hvasaact.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2illrryym.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2axsxmsfh.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rgzzsvci.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zlyiicij.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kyvnfsyq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngwkcmoc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hblqxmgy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2flxzzikn.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2otqsswfn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2fxfxfmbs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2gmbsyjru.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gndqdonj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2eddlptjc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oejpdmll.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xmzhbkja.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xuaitxbo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2emiehtyy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uqfgkmvs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2fhyuuwka.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2dqrwqidh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2eabkqnqu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2jdrdjqev.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rdnjagdw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xhstqxxd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sptqudps.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ralkivwc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ermaginq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2iwmdlkfr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2wgulzjhv.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sidcjaad.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2jksnlyez.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oggohvmc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iwcsrfjt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2vtqnypyy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2kbtmxezq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2mnfquhdj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2jcxafsfv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2jjclpgcd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mrxumjoe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2bucxbyvi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zvqaqhct.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gpkyiede.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2fsiupgwd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ofajyflv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zcolxqdn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wconjoxr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2xerjxbii.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mjosbucv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2gjdmdobf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jjlgolgc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lsnvdeeh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2adjtxgsg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2zbbdtwlo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2yjtmybnm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ptrgtgpp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ulfdpgoi.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ismdyfnd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2boetxhwj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wrqjzodo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tzwxjgys.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hgreileq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2hlwyxvmh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2viwejgxv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pcmbmzio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryacockm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2yskqxirp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdohwpxx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vztinhdo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jlwanooc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2iskihshh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2upenered.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qznnqqmj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2cskxvjef.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2qqtlojdr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ilrnhadt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2rztltaoh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qaklepqm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ixjhaolm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2fvcdosqt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ethqwbmn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dfmayoof.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xcffiihv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ldeyzgja.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2hvhfdffa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qurcdrci.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ymcttpde.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hjxhmbxd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qscqwsde.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vazoiieh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2blozjqaf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2emupbewl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vqtcgudc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hrgmievr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jhrrrbaz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hfkktrpw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zfsuygmj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2milpcdgh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zwzgxgct.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2welxrrwp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2acfzxxhn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2exwynqtj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bdryjvqv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2jplilkkr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2nduppyzi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tmzfqnag.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2mzuoxqdu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bmvnbapf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tqpcshij.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ijcqzmat.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jvhcnnoi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2aoptaxkd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rgvvalzp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2lrdjmmji.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zzfzunjt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2unksbgvl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bbjxmzxc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bwxvdfgj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpnwbmp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ldzvlqbg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2pdaizxrq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qmbofgtt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wojdajsl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lluhxygh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2habeowkl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hqiikmrv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2sveakird.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2xudmvapo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2iytigtno.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nlmoefsg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2srugfkow.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vnsjemzy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uoldpxjz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2nskngyvv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2drmkouva.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fpcbhiaq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zzvymjns.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2iniahuzd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hybqssuo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lxqccofv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iebzrvcy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2joqxyoif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewmlfvqp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2skcrfjvf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qsxsusdl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2emtqofzf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pfflopfy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehlidcmq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gzirzcmi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tbcnccpc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ececbabw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bwlmeseh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kmhtfqgx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yjwnqrta.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ctslalek.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pbqltgeg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ohfpucsl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rnasqymm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vtdrvhha.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kfhrdnlj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2peixpbpt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bjzfhrdd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzuwtml.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xckvryjx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oxgohsul.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xwzddrhf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vulsxgex.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ijbgwetv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2uzrwufau.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2thshaamd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zqdpfrhv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wotyfqgy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lqudsjuo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hypbsnha.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bvoqtifb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fqxsshcq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2axsixemu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ojgvqvhq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2oymaazsv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ykrmnwzf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bujvwxry.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zzrjdmdw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gfzrvlft.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xazmzzxc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctxrssub.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ldqhoslf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2erjrxiwx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2gxezrecb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cjtednyy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2odeexjnc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mfmfsllg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ccchayjx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2osvdapbq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2lmmguxky.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2diqakzfv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kxdqxrao.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2cabutkwf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2xxtsvksk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vrqsfcra.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2bmftpare.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ebrtzzie.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gqffpggd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2acrotknu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ktjrmuac.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fkrhtopj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mghisuvd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lueqanze.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2fnbcimdg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ytndedpl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nijbzphr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dfqxtxba.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2aeyqrmxu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tuvqtmrg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fahgogvm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ovezsmxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggxzdudu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2anlrytpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jviibsvq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nostjrxa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2asbnnwox.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hdfvases.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fpqdoyhw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xejfmfyl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ofbszngb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zpcnngjc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2lubvckjm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzbdubkp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2usivsvax.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cbpxhfnk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2blqlswmz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xtrnrjpd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oxxqkagr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2nwekbonz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kiogmycr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dferasra.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yxudymkw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2szltdqki.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ippjuryw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qpwhmhyz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uztioiti.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dtsfakfs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jkhaxyyj.html


<!-- 参考信息 -->