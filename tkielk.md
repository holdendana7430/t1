代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3qtivbgym.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3bnfqssfa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3eufjwwbn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3dujhjiyb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3nhcqqsvj.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3bvgubflo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3gjfnvgfe.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3iktdkbxz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3byselbiv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3rdhclxup.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3mwexnjhb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3bculjatf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3zogkzhdt.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3gfwdnszm.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3qnlyehbl.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3lrgzdfak.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3mjsbnxkj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ufowzngo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3qeosyjdj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zyvznalh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3eryiiqdr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3rvytzlkr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3bdzqfbgk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ayuvzisn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rtygbcen.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3hvsjmtvb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3uuaoehtp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3twomwhzf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ycxogcza.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3qntlqjfw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3fgbapkaw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3wwpygydz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3cdzsogir.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3dzrmbmsw.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3adqogqcz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3jmhjairl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3mcrsmbjf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3oomzvywe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ymtdkdui.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3aaogxkkp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3stfqwyyg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3jbipsyxh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3uqmrgqyg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3yhlbkwae.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3oqfdxpww.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3thccamzu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3mjljpdfd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vlvhpgfi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aurhhgrp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3jecqioww.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ndjhxkjv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zchtyssq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnzzunex.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3hdxsntmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmcvinnn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wiogicme.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hxtxdcbr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bphmplxg.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3deqfcach.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oohroomp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ihbaeluj.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3izjpmcry.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3xvumdvmg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3uygbjvho.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ihthpjev.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3mwpeydjf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qwzpallz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dkadxzwh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hmgynncd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cwewuzzy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3mobkfzxf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gheevucs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jdqkxncj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3werkxiyh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3lxvojwqg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bfvxnkav.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cysvwhkq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dyqdudwr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ohpxzljb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3khwkjyix.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cobpzfdx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rowbspyp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ppiziwbi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3optqtyxb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3nweujizh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3tmuwpesi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gxvxmewp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kjaahynb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wggtbwae.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gwtvroug.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3btqzpphx.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3jztgfjuc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3vgcmqdma.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3pppzbvmb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cczsxroc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xuulbnua.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3eheiuxgg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3hrdflfjm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xpqclapx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3hrhyrmjw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3wyzdidsk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kqjaypmq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3sscghdbf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3izulnbgu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fqiyjzvx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ondrblkd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ksjegbkt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3selqeskm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vpmgmaha.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ryaotayj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3otzovydb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3xdaufqev.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xwdlxwdo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hlhbjzjs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sajqdqkx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3adxacxey.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ylcknocr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pyomrozj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ofmajhsj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uhdgrkxm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3qrwvfney.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kcwwdjot.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3seezrdjv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3wcdfabui.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3nmqixglc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ozuzdfen.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yypqfnmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpwskbhf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3pieieqfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gsjzhwmq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3bsnvvtnw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xdmyeyxv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kpacxzhu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3eroqzawv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uhvazomt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3leadwxfw.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3qfvnszmh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3kunxxwil.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3mqnycovr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yuksgmle.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sgoqygsv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3lrspwexq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ypkhqwnl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qnbostni.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3thdngrvw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3rgmhaswb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fvvqzalm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3xyusufmw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dyihzvdl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3gbjkvyme.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3kugnxcqm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vqecbzgz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ffunuhig.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3wecjncyi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lcghgtbu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nletgotw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ktylpwec.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3kdmaepul.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3smsekdvn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zddqcnwb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zaeqcroi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wszdfbks.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3anaykstf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3unnzjtgt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3vcjoeosn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3mikrcnro.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3eziywgqb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3amlgnvcf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3rzjccymz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3youhkday.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3crjtjaaw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3nhdashtd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3eafcytox.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3fymrmeno.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lqsvzrsc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ackwdhkx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3itjlbypm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sykmqzqx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jrnfxxdo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yoslnmqf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yhbbdxtu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ivvuzbic.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3htjwmpll.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3aihdnadd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kythawfz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qimpqrxa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wxluwbqy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xuukiebw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ufaommgt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mcczviwz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3arlqmvqq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xsqsguua.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vigeckic.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vwoizpdx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ejamppfu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3yyechxza.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eyanvcdq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qvepdoyw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3zkhdeejc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3tsmjkrtt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3petvuymq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hqzejouw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovsprdgx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ueyajwfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgsbwdam.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3igdeudbb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ydazvvgt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ktjriaao.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xuwgssiu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pzcejunq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wragdkzk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cleeamsb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cbsyrrax.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kqfushrc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vcxmkdrx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3spjurjxq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ypkxzyyx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ccorolqe.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ezpubrkm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jmftizbr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fthtxqzp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3guhkdgrm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vstoseep.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3awuggywd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vzzrngwh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ttmqeeqv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ijwqdqss.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sflfqlbp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ovcwbjyp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vxqukjya.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gjxzelhu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mdtkihvg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3twttfosk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gwgemimx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bafjptkd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cgjkbzxr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rtpxwocn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3utzbnbfn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vvpndyik.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ofbckelr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qucmvicv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3auajpfoq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rebcwumf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rxfwtqiv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3myddnsdb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sctocmwp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfznqwsn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kuwnuoiq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mjvqanuy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ioxlyadw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bnxxioud.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3khgmesnk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lqwcfxfd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pzxdxpaf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sgbazglz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3paqzklzw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3holapaci.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rnvliaur.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lvqslxht.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zersuojq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xbnckifr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cavwocfi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xtfhdlyh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ptbnvgib.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cskzprgh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jejpfqhv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gtqmucqb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3sxegbuxm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zktuyhnr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3gsufohdn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lhlbuhzv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gzponkdg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jyggradl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tjhgcstu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3oawptaij.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3lhkxnsfi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3csimwrrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozaneuoz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jsibayrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsecnzja.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jibxgmzj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wmzuxviu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qakjjhbk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ornynsqa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xporqcyk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqedmvdj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oklqbdml.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3lzymcyww.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ehgbyveq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3phnmhdpd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kkcszhqv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jjphcqkg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dvvmujdo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zraoakgx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rmuutguq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vhhetaqs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gnfpvidl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3spedowmv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bjwafybs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3swmdaefm.html


<!-- 参考信息 -->