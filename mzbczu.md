代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2unwqqywe.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ergpdnwd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2oacsdgpy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2kdrividq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xszsmhnl.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2awfipivb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2kokwhmwe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2zsjmipyw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lqbkazqz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2stsmrofx.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2jkagjxji.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2nqfprimt.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2hnvxrrwt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pxlllkjh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vnuzphww.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wavmwqky.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2pvywzowk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2deokxicz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2yutrrsvs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2sdcobyia.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pfvxccmx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2pvovjvzj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2rnkgtfxh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2hurwjgwf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2geaekfmh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2hiazvnpd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ovdeezen.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2rszsfflc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2mlyjcwzk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2qdtmiakf.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2fpzyvias.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2giujhovg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ddyysbpo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2navqcasj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2myozvaez.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2onsrazto.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2vekmzmge.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2twmhegnf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2xnyxybps.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qrbwsdmz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2bictcwqy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2hbjnhqbp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtbibecn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cehbuoxv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2uyohlmva.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2doiozyxs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2kptwcpye.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2rgyinfvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzrkkgij.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2eolevewj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmsfvxxb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yrdycwfv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jimocnoe.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2cubumfzx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2mipfjbgs.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fnjjjqoi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2pvwuiuii.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rbplcjrf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2pcadourk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2llepdpzr.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2gpmqgazq.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zaetpwxq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2xxrtdwmn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zwmiswil.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ubulqxir.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2idpwfnfl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ptoccgpj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ttdhfgzm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2vbhavwar.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ruftynhj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wgeztjvz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qpuwdaum.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cigxgcbb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pnvokbda.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2wveswovo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2byhfmngd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fwbdoylo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2rzbynkvd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2bdiirtyx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2wtbqhhis.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ujlyguur.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hedbkyzl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwesjsga.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hctiauha.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2apgatnuk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zbaaoily.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2nwxinags.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2tsqyrckc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2jzmahnjr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hxgzowme.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2axmtihhc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yulstisq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ubmjcntn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2vzjufose.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xlbeinyc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2rwwlzskk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2pzkymlzy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xflnehdu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ofrgxiin.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dzynvczx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nhqlmsor.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gdbfpsan.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ddxkdctk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xjoyqsor.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2klsqxhro.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2gajusyxx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fkasmryw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ybgdhnch.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bliekxmu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jrjnpfhu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ddvufcju.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nbtuueyk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qzxcmizg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rycoeaud.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2vxzweddh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ydwdqbvm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xaupporc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2pyecfuqm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2icmllzvc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2oqtkvhnt.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dllyyzjo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qyqyyqbm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ppbcdogm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duizerjo.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2wnxbwaci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkpwtjhd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2estiqklu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2knrpxbex.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mgsoxdhd.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cammxoqk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ytksnhoy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2rbcfsero.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2yeizexnm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2tdjqeuys.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uimkxzmj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bmropheq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2poekhdpa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2dogxuokj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ushzexcv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bmvsugwx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ccnfmcaq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2vecfroge.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2txptmqgy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2krvfythg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ggpfmeni.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vnrjxvyp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2itzesxba.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nspnvuge.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2prwraciy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2krwokttv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2aadsjaax.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2dvgvubeh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rfxttmqo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2mdcnppwr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2nwomgeuv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2fknuniko.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xuhgrhwo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rvrmvpcp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cexallka.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ufiosmmu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2lijozyfv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zvepvzyp.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ssiebbqq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nksejdnn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bfqquvek.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zbfqblve.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2usovmllz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qnwezsgm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2axmndhwe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2rubtqevr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2anujhwgs.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qccxqbbx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zmbrqayr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qnpiarmb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zszrlfcf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yeoqwvpw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wcmncnuq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2yfxjhepg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2llxsbmdz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2udeyrvtf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2boyrwvuc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2vpeqszku.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ubqudaxv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lxfszakf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zurngged.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ampbekhf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2agiyqyua.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2lpioixcv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yxjxixhc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jihpgcrx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wexxrokp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2blfmjzbf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pauwlome.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iujeumxa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2grulpesp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2oqonhfoq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uhssbask.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2llptfqmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exauifod.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dlfznuje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfpwnytp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bvbstdnj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2gwjamolv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lmrndxkv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcnqcxwz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlkjthph.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zmadrmuf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dqyqendo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2anhvbbbn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ffufgikr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2oxeunrns.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pvzgdfwq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ngapzyda.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2aphsnlwb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dlptsbfe.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ggnrhkng.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nuhtavsv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qhfaixgm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zccmvpla.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xioutoan.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2elopcpcf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cioedwth.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bupghodt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2arhgdhuv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2sdfjwykm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2daktqyxh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2atuhtiwy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2uwzsvhky.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2tlkvalda.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2edpqfmvp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2shldpwxk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qcodwera.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pfknjoyr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hmyugmvr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ehtvfqpo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xleblmmr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kdrljpjz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2sindmaep.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2taupwraq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iccbnfnr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ysaqfohr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lprcckwo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2npyejczv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbncctnm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2aizbtvfu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2sgymzfem.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gbfefrec.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hdziqjhj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2alvwdknt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uzybknct.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gcfushub.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fbbbjnez.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ljiabhfh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kalpkeym.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2natmtare.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2iskqhdjj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2oibmuheo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xbbsbbqu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gzltnjtm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xpejrjsm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2erritxxz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2umfmdbdp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2tsubukbi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2yvqqpbpa.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2veselqor.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2fujlphvm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fpbnazko.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ficmtvgl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cquesgrw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tzemhigm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2iymxymni.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2yhkweeyx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bfakyhke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dazdvusp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jjtaegpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bodupvhi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2lsswwjpy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qpvksrjt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mcovdbme.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ksovtsun.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lqshtrtq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fpfdgwbs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dckvolwn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zigtoeij.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eckdnuqj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2oqxfmwnu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ylonvnir.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2djjuzwoe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pnswrxza.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2refffwtw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2oywexvlz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mqxejbwg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2udpdnsdk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uueaogdd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qvdqhdkv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gqdzmqlj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2pmtcsico.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ygwhwlxx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jovgkqkk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qfdrxbza.html


<!-- 参考信息 -->