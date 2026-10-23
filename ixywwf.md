代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3fhvqfwhq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3fohusqwt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3awpweumg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3rlgbukde.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dwsvswij.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3crdltiii.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3szvsfmna.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3gcfoidkd.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3qqtbkjuo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lgomeroq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3idsgepoz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3osytvori.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ptbauigj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3dwxsvbnj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qsdfitps.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mxzcflpm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3arhpgrhq.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3zuhswgdr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3liilvirq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ucuztmle.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ggecrauk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wsyesbau.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3jnusupbo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3eifyvpfe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3lezcdamu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3yeuyjpha.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3vvrzhbui.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3smlahnhp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3qitntorg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vsgbojax.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3mtvyppxp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3bahzkjzr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3nwwjzbxh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ynyqfzgc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3kbytchpj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3rsdlygbp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3fxermjfs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3iwdmsiay.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cpgopplp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wczxrnwf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rpmyuzbx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3qaozxfii.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3gbiulzbh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3enkmbrdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krogupps.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3rnxndydn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3scjaqzmf.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3idljejev.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qtjrdzcm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ooxjwngd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uqnhalem.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xmahernf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ptzpiwnx.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3reagiido.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3dessyavy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ajgnbffd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3qoznuzrl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sojqwybg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3vwvsmfvw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cfayryxi.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vrysxeao.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3stgniidm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ilkvndqi.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ioguzxgb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bhimlxeq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3wtzsbbmf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mvwzwaih.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3koknnjce.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xmanzocy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3javfgqzv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hflsfspw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3abqsdnrk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3fytlosos.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3omijjgft.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ajmigzxl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jmgbvzvz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3osdygsjm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kxcdllkg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qkmjwtoa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xdcchwvl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3rieqvsub.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3esehjpmo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vkykpmxh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3usnlqpxb.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3jeuiecjn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3bfaoyiue.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zaaunzfh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hbpikbne.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3oveiyhvr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3iywgyztd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3nbhsjjlz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3sugqkpbh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3rhggatmh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cduajelq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kxpkoxfb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fcjsqxyd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3spvveoay.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3cbfrfsdq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ehbhtpgx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xcrfleyk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pzjhyiuq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3tjlvtbqi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rkatkzgy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zvumykdw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wynbdeib.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hwgbdddp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ufvxjybe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3xgbgfdqp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3schrfjwj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mzqygjjn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3psqjtibm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ftfdroap.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tmkfmhog.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rkyrsgdn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lrxraimh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3vcajalbj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jixvhjcw.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qmaabolv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qqmehkfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vahlyabh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3zelwwfuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcavnamc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mswkwdtq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3unfvnxqn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3sojlzhxt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kmxsrvwn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ysqqorhc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3lgsuqmky.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fuyvcfcy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3glrrpdaf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3fwesabbj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nwlixrhr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jvchmwvp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3gbghzwvk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zivnajac.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3skcnwpjq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3sbprmfxh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ylizosco.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jewxmwex.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ajcrnmgc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rcktqldy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tmamcnlf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3jdvqnwlr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3otcpqpkc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3tywjxwzc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3urupajzf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rooydnif.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3zyeohahd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bycyospz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3exlkcejy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tjlxgqxh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ctqobxge.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fpsbolhn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hvugowjd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xsiwiamd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3tqejopsv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3uutmykzt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tnvtvvvr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3bzvcyben.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3cmictjra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3afuoyzhj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vccyijvx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nmotrjto.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3kgbprjlr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fxffcnvc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3udklxesb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cdlxmbtn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wmabfzfi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uvczwmcd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ytwkpavb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ihgogwud.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dzsesvev.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ejbdenmm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3iwoluxww.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3uccokhfn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zpkwbdoh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zcysepyx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3njscfuel.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hnviqrxy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vhfttlvo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dpnufkpz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qpthavrs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fiiejdqt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tuhxhjny.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pzsvxqwx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nmujpuef.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mqgngqoj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3tomnzhkk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sraabnjj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uqkllgvl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mnmcemps.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pvrkbapn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yryvuavf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3rogrsynj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrcmrhmg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3wpsciuja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzczkojx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wfnozgni.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wltkwelt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3zhfdcyrm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqusftvf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jdycslws.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3akfktpyq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3chtxwtuo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nrgvxtzx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jpetjltk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ywmfxmwy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jrzmxzul.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lovfligd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qbxwseyx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nydnxcux.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hqkhtxcu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gbzptymq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3gqtgnyer.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wgvdxekt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3dpkroznj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tpgtljvm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3cqevaqmd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vtniisnz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3anwwvmmt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xocvbhnb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3gblfmuzw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3szvllyps.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3njjxyykd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qbpkwjxs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vkevbuli.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3cbopqhuo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fvqxnfix.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zgartlom.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3kloagiku.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dxapigua.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bxtomydo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3frwzqkhi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cpsbrmsl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jhvimwax.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rmorbcaa.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hjjnmwey.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kfapsxpt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mablfxcm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xmcxjwtd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3emppguyu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ykdscxkr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dxhgzqji.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3teddgmrm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3eogevyue.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zvcgwaen.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3aksahuel.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cwgesxxu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3mezccmjo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3utqxxblo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3oqqevutv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bdszwzrx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ghobxamc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ooqewops.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3niouyqdu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jbvwikgf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3emtsfhsw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3oieojhnt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3llvtvcrr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqjpfdr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wlpmfwcn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xtcrxmtz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3scrknwcu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3aupramrg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ngsnvqpw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3dyqucxfs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tcnumloy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rwehtcmx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dcopelct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijbpoulu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3foanlmsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kquaeagv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zqsjcdqp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujztmtom.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ogsckgat.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gjzmfxbx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wyuhcxsg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3opmmmsfv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vmwsyqsm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mctzijeh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wibqzeai.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3anlpcmce.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qpvumhcj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cikmhuxd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3chzchmbd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3crtsjtot.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fgwhjbuu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3izenhssy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3okpiokex.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bzvhvvon.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gnygjhou.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3cjswofpv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3eeoydavv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3silbcijl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gzdhrnix.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3fdgfxbzx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hobtoybd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gsvrxbhb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3seublxhs.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tqnmnbhs.html


<!-- 参考信息 -->