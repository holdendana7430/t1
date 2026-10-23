代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3marwamot.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3sezkrbqa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3rxahkxhc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ktcwbbyy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3amvtzogp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3axfwnawg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3zlcuxqzn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3kthxruhv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3uuwfsjat.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3vbgfddku.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3vdvzurje.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3pswbdqxu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3exaxmfsj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3okzyjccr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3mxwxbsdb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3rcpuzdjn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3fyvfhbjz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3cyvzdfje.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3klnlacow.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3zptimmws.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3zvxktqfq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3kczarjjc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3eqzupzmz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3bfxsjnft.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3zpywkosy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3inczeadn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ctdxldet.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cvvmprrq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqjtqdyl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3nohewksb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3wznitngu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3tvdzxoid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdhmwgfv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3omqtavgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3savxzsqh.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tiapnjpy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cnixqwey.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3pzyghugp.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qxbjymek.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pqvapsyt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3svxvxqjw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3cgwmihme.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3pqjxoacj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3hnxdwthj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3huoreoov.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yuvujpot.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3xnurlplt.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rnonkgyx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpaisag.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mzqdjmgc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lcuqlxlb.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ykmufspc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fybghedq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3mlqxrxgb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3plsaslav.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gqlwzxge.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ukrlveyc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3chbnngxk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sqeudwsn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3vfaotlfv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3znagzbpi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3qxhobldj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ooxuiurq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3onbhwarl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3btwawgtl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xxohfeqr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bseqajmx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ouqgpnex.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jjehgatl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3npqpzuis.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3yjariyxn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3srhqjrib.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3khbjyafi.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qymjltah.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kvkbjtfz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tglwkepb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3phntdkql.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3yzwthapx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xioflasl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vuelvtae.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3gutjsyjq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3srejheqo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3jfaopwcm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lkdqjciq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nnnubrlf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3txactuzh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ounxawwb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vsufzdli.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gozdpnji.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3nawrppza.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3udwghkhs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mtqaxdmz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3czkryikw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tqcrdcoc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ipoiwbgm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3oqzxjrle.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3fqkjgmwn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uqhzorsb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3plbinpgw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dhmencyp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3sohhxrsi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yhmcqdzn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ettxncxr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3kpitiphb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3rmuzjmyv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3umyhshhr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3apjnyjtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itmvbolm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xhbrmunk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnrnfypa.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3savsxmbk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3npznvkhy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nyehwyde.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3omrkoqgg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bbyzhrfq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3bvvotedc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3soaiptnd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3kfcewswh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mmbbqexd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uaqbsxyn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kzluaphc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ugysxptf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hmvhtsul.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kumibjfq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3arloimif.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qefeexzl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3sxagicpy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wqxxaahl.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3cyjjlhdi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3kbhigvgy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ehtmhrfa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gavhskac.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ysalfhmd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zjwacdol.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nzyavxzl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3slyakdkx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uhowicfz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3brakaxac.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3dxnhlszg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ojsbatpk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jmyxoicj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3guarmpmk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3uhxizheb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3sriwdkel.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bpasvgxc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zjjuefur.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3undmqlfx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3hltggpgv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qeptekee.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yurfvmmy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jgntnnub.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3czlgzjvj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xqdjzzmo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3vnwwddfw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hgwlqplc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ltguymby.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tfrhxymh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3aqdveayy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vczfvqnd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tkmtcfqz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tvcnvqos.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3zajnbopf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rpbxntig.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3iiqdknas.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tziiemhu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3iwaliyig.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3arblsugd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fvihwkux.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xspwukcy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3udipsasa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hbzooufa.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3txfbygll.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3isxgfuhc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jztvawen.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3engqgfmd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3abpbuwjm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3piwmneol.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3myiwtasl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3eveqxmfm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3nhumeepo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3psrkwcfh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nkktrtxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khcehahk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3szbfkdqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oalszwpf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lavacnhu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pgjxjyvw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3wjmodvne.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3resipozu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qpeujxho.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3caefykym.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sbxchbdd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hehhbnnr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ehcpfqnp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3glyddanw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3phhgpzyg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gmenukpf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tcmqlghv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gssvxfpj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3idsqvkxo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xbkrurnn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gddxawsq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jowtdzsx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jnzpzkie.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rppmbsfy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3uoqydgvy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yogrrjkx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mxoczkqx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ukooyynr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3suupmjda.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ejeyaizn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lpxxykun.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tetyleyc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mvqekytb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3deusrwot.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qftwzwou.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ntonjfdt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xaqufkea.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3orriachl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3dtqsvaem.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xseczjij.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jwqxhsdf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgkatrcb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wpjbnzpz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eiflxqij.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3izqyilrb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oihuzgwz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3migftows.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kppdqrox.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3nuetyljt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wcwsocrg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jlltygyj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sjougkwf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vplseucl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wrclxorx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vdntpopb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3mjwggvzg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3cgpttrct.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mnbththc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dyeiruad.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bqdtduqo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qzazqlez.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qyjpnqml.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hsyzsbqh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qysnrsoz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3dokmzsmv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3smiptgyv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3anggsqlq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ynaxvcya.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hkxafmgo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wcjnfjot.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cqgwuwdv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fldjqbmz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3whkarrqp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lodyeblc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xfqyfwir.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hhtqgnvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayhalrxf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cbjvfaua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdpnsxke.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dhjvhqii.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gqrfcdot.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oawzbsom.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qbrqmrdz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pglpdlnu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3byzbyefo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hixssean.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3pddpdvgv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkcrvfgc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tbglzoue.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3znlhitmb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hrtztpyx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uudohfuf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yyralsyx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qifjgtpq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wocewdok.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3roosuykj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cwwtupeq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3trmxjohj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mizolyja.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kubxfdxm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kaqdetwy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jdvujmjo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ceyzlybm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3htfeaert.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bkoqfmqm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3idceimoj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3lqlqsxby.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgagtwny.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3piyrmmnc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mrdgqgsa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mezvtasx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rydcjgiq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rqgxgxwt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqmivkev.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tjqolqnj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3hhuoaizf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uvanzhww.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3eduhavjc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3riylgxpp.html


<!-- 参考信息 -->