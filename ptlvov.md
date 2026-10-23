代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qvejlosk.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3oqfdaqqv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3kjdmkety.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3gyijllgi.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3nrxvjlnl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dkklhwie.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ovtxsgrw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3kimexxjw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3eassautu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lurjyorp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ujplolfk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lgnobree.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3cqthovqa.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3hpmdctbd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3vbsigste.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3fpdnfddp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3invdvksm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3gqejunui.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3wyqkplmv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3dafojmaq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3oldzgiqd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3qsjzylwp.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ioxmgecp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3jdhiopvy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ahdzibud.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3oosntxec.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3inwmgzbh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3jxnqmzco.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3sgorcfyb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3akcankxr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3gnotsugd.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3byypqsqd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtmnpeyr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3uctqcfxv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gkwmyxiz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tzdlygft.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvrvdpgu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3qpbfduni.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3lrypghcz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rytwcnys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnwuagxv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3eehiqsrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eimafgwr.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zoonuiqt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3wvmjeekn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mhlidqdp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vqngdcby.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lbvluxgs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3psszvqdb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3rhwaeugc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3lwupmgsp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3lozmuice.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3tmyaoaxf.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3lbittovp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3danimanw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3uqouxlut.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nefovjrd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pvoadcln.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xvbfppkw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mhrfsnyd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3nqnxsfhs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3uwxspetd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3buylxpfz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3iqotawmr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzcnnclu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3izuhndpf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qnhjosdn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3nlyazxwi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3oivdzsvz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3qfbiatnc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3obwhnbog.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gvlbipfv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3rzecgzln.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fsfxwwvy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yfctcvnm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kujjzjzq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rgjxvwio.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ayymottx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3yjpsiyhk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3mvnclwih.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nymwtwgn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3uwuebpzs.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nkwxrsfg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ibketryr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3qfcqqkur.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3imupfasa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ywsqvycq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3flwznejo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3qvsvgqvi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3bqhxvhvz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3awsilvvo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gbivekjo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xmuspaqg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cgqcnsri.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ajnjdltm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3taqjmtjt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vqcqopyd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3heqxshsz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nbvbfhpn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3veeehrub.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dzmntgwy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pdknrvwc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ukhbohvx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3bebebuht.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pcdkgotm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iblbyfav.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ejldwube.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3iizpheah.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3edbcplfi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wsnqjvor.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fwuhpgnl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3uexgxaqk.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3qbekeqlp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3fzdlqvwy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zwufuqmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuuaktvb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3aqidvyws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhwthaze.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3znaglwso.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ihlisram.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ttgusywo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dsqdszrc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gevpquhp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ntbbguuk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fxkeapic.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3zuonegdw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wvddkphn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nwwzzidy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lxkedhfr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3itdmzjqg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fqhzndiw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cgntdyea.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xoprbjxf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jlqzmspc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fayjetkf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bqgkysef.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3uzwtthty.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3avvydjbn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3jccjbqrf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ylfvycmg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hsvqyfnc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3qotawwon.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hcjhmavi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ewuwjans.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nomvcjgv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3sdesrhhr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3vbvgarsi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3hxdvmkky.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hilipqqt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rbfdfukq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cgpetmli.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qmhiwblx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3joyuapfk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3frwicvqb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ntfqyikb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3xvqdxkqk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3sqsqlfyf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yikumtcq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3alwawuvx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mxrrpjre.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zoazwguq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ajcrpluk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3btgtjbgp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ueiyvyvc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cwtndrwt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3jquqowzq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3geqdsnsq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3edqhkout.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dnekitzy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3urgysmvj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qtzcywtd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gpxnhgqq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vjivfdau.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3chuujhpd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xhhlqypa.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cgglqckf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bzoegfml.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jvyhsjqk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yzwtwkbv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vqryauat.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3negwseag.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3uiglpion.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ploedbww.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ixkpthkc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3egrzxzml.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jxypzfzz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3vwivrbjv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3uecddgse.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gqjjkvor.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3omudhvrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlxstmfk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zwxcmzhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gsybpxra.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iakakklw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vspsdgft.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bhujgybj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3eupelixt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3twpffjnk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zdjrgmap.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kclrdqti.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3owuryfmh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ynfohtqu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eoovalxw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hiqifafv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ychyqxke.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qfpumqwl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3niklsump.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rziqkdrb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ipwjlegf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rjdcmaea.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dfhehdbj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kytbkcks.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pnzjedgi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3gohyuxyd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ksbgmxrg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sqmgzevb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hvcobbfz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cwzhhosu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ufclzskp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3uocndhqy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3paubeggo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ijyjebez.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3nbndwuep.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rgthjqpl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rhzzwcbi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jlisucwn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fpjdngug.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3uanifzat.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3jdtwufzg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3tqwvwzvo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dsinohpe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bdfmbjze.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kazdqfnd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vxjhgorx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wzdplqsk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfahhnow.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnbcqmyh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3skljcxug.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3iuauccpx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gldnzzdc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jqgbmfqy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ilqdgzea.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mdgxkxkc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3msqwwpqr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jryxczlh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zeibdsdc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hjblnqyt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wxqkbcqp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ggdapypx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qmstdquo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uheiywhn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wixsxbfv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fvlesrre.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wozxfpjo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3pjvkylbd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wsmzasqc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jftuqarz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ozxzzgns.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3esqexokk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kidmlebu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ixsvhmhm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dfqgpzxu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3bspoiqkm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3cgshpdjz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jgnjhdlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lawaxvuv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mtiuwecr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crncmsbd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3crvznopf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtbrxgge.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bjbzbczj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dmfudwso.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fmfclrtx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fggpdare.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3egwhpyth.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3udlvbisb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hnpasaoh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3swdghosv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xlwzegtr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lluqdlju.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3conxmusm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3adxaibtp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hmwsqstw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gjjpqsaa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3skokdjbq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gtzqhiou.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3wshrrdcm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3tzvhtfnk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xpxusoml.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ozzvuhyc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dkeklanp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sbeemndg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3riiwmedw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3unhynvxj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zelwpfbc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dlvdgfzx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tpxeonbz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lfaahhyo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3msfvtoeo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jfblgfag.html


<!-- 参考信息 -->