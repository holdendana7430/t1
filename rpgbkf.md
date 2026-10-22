代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2hhfnedrj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2wgfsaxlf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fsaxmman.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2wovgdzfb.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2iuamtjjr.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2nofimhae.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2euaarayu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2cdbrlksr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zeurgrtf.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2isuozsqg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2uvipcaur.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2qjlgenpt.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2rrzqvemm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2iwdgevxk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2nniqvkyl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2flmkjsek.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2etlariwy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2fflxzglj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqqsvpls.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rssnefld.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2uzydwlaz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2agdgkoqb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2bkwyleeu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2vrjcztia.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2czdxckqh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2zbvaschx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2hgvqlqie.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2duoilkbt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2btzqycvx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2pmrqgjlz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2vdmfcdon.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2iycwefrr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2wpufpdaa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2wifdgcvu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xrnlqhqq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bgfwtqpf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2yyhjazmr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2qpqfbwvn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2zrfuirlc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2omoyvhgi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ayctlytn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2kjehymrj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2biptzzbd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cvnmhehc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2pfrnshwq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2aezpcmbb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ebbjdpxl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2rqeroykt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvbrdlel.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2wvlpxtug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcanahyw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dzxacrjv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gaiticxf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zqlsihvq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dvvzxlzl.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ouanwzpa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2jkvfaaoz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2xjjrtngx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2xqataxhj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dpegfvbg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2hawfofvj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ktzxdpzg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ddmwlksk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bebwuhrr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fmqflheg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uagekjbi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jnvjfnju.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jpisuqes.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2dodborai.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2omdwsavv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zikyztvm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hhlegdwg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wchdhzwr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2iyqfafwa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zvdxcyrf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2rfhkwctg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2fuuywdfc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2sbfytfkx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2euncodao.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2pqkqwucr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ejdhzdck.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2txbcfzms.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tjqlfpmx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ftkbvlir.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2tfofvgyp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zdbogibp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rxgjnfci.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2dqhnzajp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2kmoycxjt.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wfirejta.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ihphqodh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fcgsnnrs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2tkcnkfxi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2mfrloadp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2yekbrisy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2onveuqta.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2gtvpkxpx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fncgqszf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hcfpiwdx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ghqupaon.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hozrvvoy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2nghskyal.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gjtzmpfd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mylltiab.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xfhlfcdv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2golvrdgw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lfsdhajp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2mwfaltho.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2psuiuibn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lebrkgtw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2asoajekn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zlftnypo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2rbrwayau.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2koamywsv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ipwwrhwb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2renhkora.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hlnprbit.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2japcydmz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ttelyaed.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2djwvqwro.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2gughfxnj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2vmqqlbaf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gqetzbyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovygplig.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dlgudlix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilwmuvee.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2rracoqct.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2qrtvyoun.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2acfczhsd.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jmtcekze.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bqshriex.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2cpjswnmg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2kyamtqfm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2jxmzwecl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vygigpco.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mrlqmyfg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2sgghmqmn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lvyovzja.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lszbxzke.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2llwniyxf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zirmndph.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2okmhdxpa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2pmwwrans.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jnqrvpew.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2dyshmxry.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2znsbnbeg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yvxpucmn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xghdoedb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hqgmximc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cyimuuzr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lkizzzsr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2slaasxdx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qupjfrqc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2npqqfwqr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2qsekiexk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2sghsckor.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xthbfvrm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2eckizebf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eeswcqff.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2phmystze.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2rsmcnwrw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ogqyseql.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ezplagbf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qlsbybjh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hrsnhtju.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cnxihtup.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2eflkkdeg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nbvfyvmd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2fgvhouio.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xffbqtmy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uradkhnn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2eedpgswh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hwzzaceq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lcwhgsnx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pxccfhyu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2idnwxcdo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gktvcrww.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2relsvjzg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2rwgnlipf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hxgnbmow.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dxykuyxr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2slpqwcve.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2snwtynmi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hbtellyd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hraigbvk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2lmiremuo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wsixbhhf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2wfspipux.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xtrqegox.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lnbilmus.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ckawereg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2yypyexev.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ilscrsur.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2myngxmor.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ouktalms.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ortpjwaz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nthpjdse.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2drupgnzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhrglypn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2qhvflnkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzglaaeq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tcftzclf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ifsozzai.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2npqqatwu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hcemmysd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vjnhuluv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gjujdiir.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uochsdty.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2odvtmyww.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2igqdntzg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ztuatyvp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qzqvvnxv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fmxcesbw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2alsbgovk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kvvlbquo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zwstpmbp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ffkkqacq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2osrosqrr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2udkzpcjc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2widfqqea.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gjtjcohb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2oqllbcek.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kzsakdtq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dczenbxa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2twsptdpp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2denrlbbo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ttdulrru.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2qeseualz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2prlfhdbl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tzwdnfyd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zjnexlnw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wzugpydj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lwdctpsd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jrtmnuep.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iljbwxnd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dlgvrdcj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2sonxramj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2iydrthbx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipuuccsm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2kkwcipak.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hpecbymt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2obbyslyo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkxajyua.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ameoradz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2bkimlpmk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hqenomjh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lxzziyno.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2shdzryxe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2artbxzsw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2oziyxoof.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ugdhlbwt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xaorrodk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mbgriuvz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2tgrituty.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tktjsrlc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dtrlsxwq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ussqvkvl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gxcarmyw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pqmloqbj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nbxrizef.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ejejzjfk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xobpwsob.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qiwaafbu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2usomsdkb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kbqegbvp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2pdogolsk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jfntggdp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zulneiro.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2viezdlrf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2oqwmtpwn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2gejftkjn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tmqeeuhz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cxipwhqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfzerlwn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2szkigsrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnlpvnlb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tyecnika.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2osemhdqh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vkynxrje.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iniqlewm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fopdjklc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nvibellg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dqxzrwjb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hpzxzjyz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrsrwthc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bvpfdwro.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bqfcmcpg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yebqeapr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eomnhkxf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jbafhqsq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jdyawwor.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lynrqktt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2atzcylth.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hftrutvg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2iqurhykq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gepvgrns.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gopndpvw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jrpdvrws.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rsjwfpvm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mqqbfmue.html


<!-- 参考信息 -->