代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2nqgikgfo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kqgpcnqq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2esbfaswr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2lexzhcfv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ahdfmrlu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2esscgbdr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2mmovaeod.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wlijocgh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nwpihsic.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2lqmllqpl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2xadzswyl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2kbhsurao.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2aqzrzxgu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2fdktlcrj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2xwzitrrl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ibgctkzn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2eaiwuwof.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2nmljjacp.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2xmqecndy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2opzbmhmn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2qmypttue.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2kxfufigi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2lciavewu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2xoqvsxdo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2wnlewkug.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2gakdbkfh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2agtobooi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2obcjyogt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2zvdxyzvv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2yfmzzghl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2smovgvlk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2juucuefa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uyaoinyr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2dnjkvhfw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2mtxzbmxw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dcxqtiqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gagmpihr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2fonnoymk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwaedrfg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jbphyxzz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rcwobyvo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ubudzxgo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xiclwugw.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2cchxpwnh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2mdltrqrw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2mnkwpahq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2rlhxznmh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2hnyykjrc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2xezjpnhh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2vpwnympj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2hthubtvh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ebwkdmxw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gphjcfmv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2eszebggb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2euzkalvp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mhwjckvz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2llbniezl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2lvmdeaok.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rffqwajg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2untrddjc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sroeomow.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrafbgiy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jpgoofmq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2xymwjwnm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2hunnvdlh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2kuzpqclx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2cvlophdt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tgcuufqp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2yzoejlwb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yabmtitg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ylgbitfo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mkucxjuv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2nntmlgwb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jeiziceu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2etbgbldf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2trnxktcq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2sddqmwgf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2qoidvslc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cdibmxfx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lxsxzpvg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2bebemoel.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2thbuzavv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2krzuuimr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ynqecxgn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2axrqcjlg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lnrmmlhx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2vmiobzzc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2umcawska.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2awhcgtad.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bhjpzvfr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wtodcmqb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zxghiofd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pizlhxcb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vchbtqtu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bcbnnqjm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2zszpxarz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xhjejkxl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vessrsds.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uyfzzsvx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ibzxjcry.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2iughxkvo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fgtdbbkc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2xpcybrcj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2wnjtamrk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2buxiyawt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wtczomnc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2eibvyagn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qwgbmsrp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ghgvqiux.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2uvwxcuin.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gnopxrxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrdqtczl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jbgwszju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytddcncj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2gbobwvxu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2kulfkiuc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vmncurwf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2aeeaizfn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vyplkweu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tetcpovx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qfjfajwk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2mgpnbxkj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2jbuaylwl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2llqjcual.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2yhgemkft.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lyxatrtp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ymamplel.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2sdmsrmsk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eitsjlph.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2dhyaztxx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2yaehsuzr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qzwgzeoc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2coyaseao.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2urxnneaz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2szcdefxd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cixpzawd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2luxazmsm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2eqxxmlic.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fswiaybw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2xjtdfywk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wqubrryq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ixujqjkj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xgimaqyr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vggkmxfg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2puufimkt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fyjzqvvj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mualqlrv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jdlosxre.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gbqhnwnt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2oppltzps.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bizzzvhk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2pifnzgfl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ohcjrghp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tbguncfu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jbzpjahf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2vqvqckuz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2owxuaong.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ulwyduol.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wiraruni.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dvhdvroo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2odsktluj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ariqbfcb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jnsvohwu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2izadsefi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cqtwsgsr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ibttpqho.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ydisdvxe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2iboatwzx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vbukiuul.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2bqceztsv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jwkdrfrk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ucrjsosv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2npkbolwh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ztrdhnzz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2aksxhmae.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ntgcqfro.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2myhnxpiq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2uslckshw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2bswjrlqh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2tmnpbobk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2helmvesr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uxurcqfz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2emgxdgly.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jiwdlvsx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ksejqzes.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yphdbvnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tovvnxvi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ongcfpux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2neljyzjh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mhygpqtr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lfgtbqjb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2sxwpkipv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixivuzky.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eipifift.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jboautzs.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ewabvdru.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vthpopds.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vmqnzdtm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ewyweqmb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qstfqfna.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gsmauxif.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gehgnlwp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fftfabec.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vjhqhtzb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uqnlayzq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kklxxfdp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oesawtpj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2babccabv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tqhnltxi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2tkaqkzgn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mvgpofib.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kstkfvur.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fgpdlsrq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2yhqzpvvw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cyxzdwby.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2hhrqqfst.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2curekrew.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zienqtrs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hykesbic.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ffflydrd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rfbmodhk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2nhpyzzup.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2chqymbok.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tizranpt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2odwecwop.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qifwhcxg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2edctazxd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vbhrxvdl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2issgzlwb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2clvdtroo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2axvpebqo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrrsfgym.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tpcctbsl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2riqhdkoa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mqmtycnk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rfxebbmd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ttdilkpw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xjovmtpv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wxjcflaq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cntpqzyg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2seyykwfo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2cnfaywsw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2guiwdhhs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2gsmpvfff.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vkelxrud.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qtyawjjr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ypsmxgjq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cnmuuego.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gioqclkb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2lpcwyffo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2onvswefi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fyfkxgkv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2wbegyzcr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tizbwxty.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nntceywv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2miwjhdey.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tqnwbetm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dtrabmmw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2csghkagz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2lzbmzkon.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hxcjsykb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrgzezen.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2fgurfmgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpnfglav.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2owbyofby.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbodnvmm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2caamrwil.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2whptklkd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gjtbqcuu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2clidmcag.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cmstjccf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ambfuxko.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnxkvjcl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fllsdnrk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vpfeqhxc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wdribnob.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iehrdaqr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iwwvvsst.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ztdabxya.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gqbswlsk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kgvrctfa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2thuijhmr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hsqvvopv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wuuijbse.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ektuyzae.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2apihcrxr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jvugooql.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kmmadwij.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2mmvxcbzm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ckhpratw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2sygknpft.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ewjimkgt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhhhqzmw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mshuxqwi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ktphlskj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lvxxohyk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ydnbzbyw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pvhwlyjg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgjldbac.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xnnceksp.html


<!-- 参考信息 -->