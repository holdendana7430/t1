代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2xkydcbbz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gcyzrwfw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2xdnjtbvt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zicwvgmn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ruyraciz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ilviduyf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2xuiwnnzg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qacqvwiw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ptialjjs.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2kfhaojhl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2teaqcyjp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2xrwlkkws.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2hmnbxtfq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2zfioyqmo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2qaxwycnu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2kqaazdtq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ggbojzww.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2gmrfvjvn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2fsyochmt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2rpwvjons.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2qialfjjk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2iyhiiypd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2lvvzauwl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2xsnwwhoe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2jrbovchm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2xvmtrxzo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2zqaqpfyi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2pdaohwge.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2yjylqqms.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2pueesojk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwlhxbmg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cynqyrao.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2phzdiocz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2wjejmgjv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ubhdschp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2tiwjjygf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trxoqmlt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2enudiaol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awuwuler.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2okqrpnzp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ssdsbfvp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cpmkaonr.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ysepprnj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zdjetdnf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2mufqsedc.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wtybrvcq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ajortlff.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2glkimvwd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2cisrwxby.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2csfmkugv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vupvnxlb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rrhwogoa.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wtwxsltt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vlwzpech.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2smokfbwm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gueulkmr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sauulggw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2zmowmpik.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2myqxblzz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2sjizviub.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayhnghaf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hlzkmrsg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2lhtvwpia.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2nuoewful.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2yzurdymb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qfqtdqps.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2txmxfpnk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lyfcuaxa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2phntioxd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ibqrbrwl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uxzvbgoz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mmfvmagk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2yjtxmzyu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2bxtniadr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mcrlxllx.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2gpctijpo.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yasgqglq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2sbbhygma.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sxpljwxm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qksprccr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2vzvirzmg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2okrponfs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jsjlkrlo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2djiqdheg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2hdcxsqin.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dgwmmgch.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2pkkspnwm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zuhcavue.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fttserim.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2hswjwwqh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bozwabha.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ispywkop.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rmvtdbkt.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2xkogsvuo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fqltcvtt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2srcubyee.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zfoesjev.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ehkoedlt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ezicbnxg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2wjmndqks.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ovpaqmwl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ubnpqpny.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dnxttdqy.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ljjppjhr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bglehceu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2uhrcwtrc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rhpriqsw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2asckjmxp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wfuqomuw.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mqvbgxml.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rgoemznr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2athwaxmg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2azjrkczj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghpkkhjz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2kfvalreh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2hixncyba.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2pfcvzpxg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fqqwxozl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cycqgegd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2dqkjljnk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2iknsmupc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ysjhszen.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2didowrju.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vwypjwoj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hhgxpcfn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2aflvdhjb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kaavejfl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zaugewbu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2jzmmkgdu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2rtlguhrk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2cqqbvakm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2fdqbclns.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gdkeuxbg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2lmlcwwov.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2mgqiudyx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2imlcazrx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pgetrdqp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2zzikqwvv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nfqcncvv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2eggxhtxz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ydupjdux.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2svmfybfl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2kuayhhkq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qbztyrpb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dcxsvywl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yyehbshj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nhwgujsv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wdqzyvmx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mmuvucre.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2lmyqgheg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2baponuis.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2zaseuyhq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2mfwranar.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uctbybbc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yawndfmh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nspoknyl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsufftjf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2diqmnopf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2goqglxja.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xqrskjes.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ixozjpzx.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kwrjhceg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rmqfdkwp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pvjgmhuf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ltwahqmg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kincejne.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2tsxiouzh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ztnjkrem.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kltsluax.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fsiizgym.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kzvilnll.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pzjohnlw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nhdfoufx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2enkscllb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2itcexran.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2pmukckby.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2psfyonri.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2awffgetp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2tcttcymo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2kzixcjjl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qsqfnflu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2atdtepbu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hpqkdihq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wofgrenn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2edppbalo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2thffkfxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehohlxhm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2uaaursvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gncnulcg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fvnvshzv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zdrjozum.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2uqbptqzy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fvbwvpdj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gsmarcyq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2aglagjiq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qzltukvf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2afaptzgi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2omxctmdc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zlsemjwf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hxbnjulg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bvcotrrj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2irvrkfob.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2owtkevxp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ewbdongf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nnupfbog.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vvsjbexe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mpbbkdpf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jxlwbqke.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ebkbafkn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hblgauwf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2iajtsjra.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hrgikcbx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zajhanbp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vbwtpvjl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rctrshim.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mfqdylkd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2poslnhfe.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ecgvskdd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ydthfdfo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xxkivpdq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iixuzkuh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2djsgsobb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hlhzzlrd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ntrebipc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nwhgpyge.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qowpicgq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qplxhqrc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2bofzkpez.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bvswjpow.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yqpngebn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2blypvxkx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rkzjefjg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jjxwvqfp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2snivashj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ezfehubf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ngjwqdya.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bmnnjtyq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ucqtfigk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ocyczspt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qwzqtpla.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vdhgnxck.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bgxeptus.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2usapvqun.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2cuxbnwdx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2aeebwdnm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mkciwcyg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ddcifgar.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wwnshhgj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ngqfdfww.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vuwyxgjm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gouejxod.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mdhhaxfp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zgauuuml.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rhzxzvzk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zzzryvps.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vxaiflxh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ubuvxymx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dfmcybzt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nphxvoes.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2drudmxbu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bgjnweio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utvrjrrm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tjzxrjbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwbevwdw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ozjjfmxq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rijkmbtk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mouzhdrh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sbxfjpxm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nszwbate.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gbyoosle.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bavikpiv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2orvyrsmf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2whxxsxoi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vpctkqcw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mibclwet.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jxfszwbw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bwzugfpk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ucnrubgq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gifqbgvs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mvglgcrn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lnnkvcdi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dglxkhfl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2dgahdkdg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2agjsvxnq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2cmixcyss.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ggnmvjhr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lphmvirv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2avmwemsb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2rbsputak.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zaaavnta.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2jwoilose.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2lkunqcys.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uchnipng.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pgtowdgr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xkvdmgti.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pvupxusi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mictlxqh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cgydwmoc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rpvjsqyf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cirqkqls.html


<!-- 参考信息 -->