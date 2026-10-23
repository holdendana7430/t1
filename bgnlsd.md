代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3nhclvqbu.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3qoxwkoju.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3gylykmio.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3jjqvrbvi.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wiovatqg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3csvafucn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3jiflprxl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3vpzesxih.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3lmvddyft.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3dhiexkmk.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3thaatgzr.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3txgeymqy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3zlkcysey.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rhzsduvp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3kkenxfcl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ixtkdiuq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3qipnfpet.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3sxzumwou.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3szrqiwkc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lzswlwae.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3quhudruw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3bogwuwnc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3zhviynjm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3kqsoykwy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3oyrbqvpt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3mhkrpbhj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3oprlhiga.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3aengybyb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3voddrpgy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ytshvzvr.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3rpibxfoz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3uefkqqhu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3czpvwtmj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bqghqmhh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3bvnwgaqk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3toykhzdh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3isrbxpln.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3nnxtzysv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3aeknnnmp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3dyjqzuri.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3shinikik.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3pvvbsnoy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3osyjnjwv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3godemtbh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nynmyowd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3evgbgdoh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3fqqrtbbb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxnvvwjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylbpgcxo.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3itpjrbgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvdjweds.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3fbszikty.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hjguiige.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qjhsjshn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uwzwllew.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3klwwfhci.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3fzrfrwwj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gvljqaxr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3myvhqtgu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ofeolbwh.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3izibnkce.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3hbwjusvo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ctzfgdud.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ocuofmuu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xecqclmv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yastmlls.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3neidqbfh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3poiducre.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lfxdevgg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3rmnerxcd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3iirddpod.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gacyytpc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pezksaie.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqgduvob.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3lvwtakyx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3rbuadoyr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3bpzqtnct.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ixkbdniv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3wrmzbyft.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3adxqwjed.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3fzhurdtx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mwzzhobx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3eousxhtt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3quahcioy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3seakxiqx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tozqbdnf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3emtamfvr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3hqsvfzrj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cktmywri.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3qzxmiztw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lbrvayxg.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hgddminm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ejauynpy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3xmccgkiq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uokdgxxw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ftbqzpfe.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ebpsafiz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ighdrwst.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3cxocqurk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xnzfdwog.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wbxkxxtg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rmqaqfco.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kmxbxepx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3athmizdl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3znhcjixg.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3cqbnkcmz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oepejuis.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3yvjgdvmq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3veqlmfzk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rfuplygy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nrrhmpcx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ygncedrf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3suykxggg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sogwmfrr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3qvcacjwz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3jyttzkrd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rqpvorkg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xnoeznhe.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zwajpddm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3adrxktpm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3qutchcdz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bmbtjsae.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vpqfydvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcoevugg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3jnxsyriw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cymxecns.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3edzmwwca.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3depuucyf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3jdhocjzw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bbfdiwvf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3eaefyczt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3qcyzlcam.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rsspnnme.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3inpmnyid.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jwxcovli.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qqthyyky.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ffrhgajf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3lslqoofj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3linthbfl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uxgrjuhy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vvjspbrv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3dvbkxcyr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jnwxwozy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3tsmqmags.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3gkpiruvt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3awuekrpi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3udugbsde.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vmdbkizb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fhqvvymb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ftsiyecz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rvmmsebd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ulvmaubo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mcphukch.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3iywzuieu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zycfzxsl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vycdbfrx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ndkxcvqw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ezbyizqu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qvmlzndj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3vltbyxiv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tnhbelmd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lhqdfpcq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kleugetu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3mccqahps.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3smgsmjyr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cnawaftw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ekkefxpn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3gmwampmh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gbnhrlnb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bqajrtle.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pshpqacn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rkdfmmra.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ivhkqguo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ojmngkxz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wagmwpxj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pxvjnkak.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zpgwqujd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gzhufjsg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qxpzwnsp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3deoorkjg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3aqsnwwmz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3nsferxqm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jdjaeklq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yeiedlri.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3atszjziq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gusttybx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uvbghqvx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ztkdxtsi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ckjltrvy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3nkpavgak.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vadudxvn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vnblznqg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xyjtkynz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mfccqgee.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3rxmusquo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mkzgnhcs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ijlzqorz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3emwrhsyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdgmcdyg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3crpkxmut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czrkjvgw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ilnpzqjb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3potsvfxb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hfanwjsh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tmnwekqz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ufsqniqq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pemhzvej.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bfxyctta.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3etyjepmv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uokzmdww.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3opytflzq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mrsvvftg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nwuypkox.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3beckhuyb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3eoxnwobh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qyupwvwf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rlxforsu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3gilgedhc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sxtznbhp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lnohzxhy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pvokmlbr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3dcrkdteo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lbdavvtq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ssbskntc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3onsmfqgq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3deeonwsb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qhsmubnh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dfyhmble.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3warexblh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ouxubcqj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hpqegzfz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uwuytwzt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jjefbjor.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cqsvkawy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zkdjitjv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fjpgfuqi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gmvrflaz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tufyuyoq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zwjmzthz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tpzzmyus.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xhnrluvl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zlyahnkz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwrtiec.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aoseafnm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zgzkdunb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nqgpphkt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gkqpwijd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3aokvdxrv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3oomukolk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ldxrugjm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gutujmvq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pmdggrtl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xomlciqq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jxwehlpy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pderxzoz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3filivbdj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pherrrqx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hvbteptw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hmuqbnhq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bdmmptzv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3newpgjxr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dhterzfh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qrdaxfsp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ilxqirmp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3szfqwghv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qbexnbqy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3jkkpdifr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qshtejje.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dgcrkqnf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3cfsamash.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ywyjbpmy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bkqewgqg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mzqqvgfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdseipsu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mxyzkdve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbskvpfi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3muixxots.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wnaozfue.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ejziqvvw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ddnovmfl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fvrggsda.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rabyuuha.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3geubysog.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3evsucnag.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jtoqcctv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kmvlpjhv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tnulugix.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pzkoghoa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3itkfvmeq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ehrkmjfx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdqqatn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hefrwhbd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3njehhwmh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3inoeaszs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yfwrjizs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3dyacsage.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3oafvwxej.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jywcgejk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tncwumrv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3plllynod.html


<!-- 参考信息 -->