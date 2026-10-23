代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3obxcpopt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fczaqiyn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3wtedhqlv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nthllowz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nnipljwa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3sxijovam.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3xnalagys.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ddrsduer.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3culghvgo.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3sesudsss.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ogqohaas.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ketjygrz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3iixgqtoc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ojeffgpy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3aqjrjcgc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3akxjhhhm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3dflyynaq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3dvictdwi.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3hgwkntvc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3kphfakpn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3yqdmgzbe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3kmqcvcsc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ywuwnifh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3vhhxuisn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3ytvfnjfs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bfqgjgnz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3sroaxcig.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3khtmqhiq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ottqoqtm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3jxurbkqu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3gybpveiw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aoyjulhn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtfnabng.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3kjklfgha.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ycxwuici.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3retjolrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hapyiorv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vzlbdhne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crfggxwx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3zydzboiq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bxkbbgfd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3okdtukvr.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ssqyxrwv.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3trbcmril.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ushpnfym.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oaesrgiu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3wieorvbf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3jimpdusc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3rzqhupun.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3luduosil.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3afjnzffp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpvoswbi.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hvkivdtb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dktbxoht.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3yidjtyfc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjlrrdl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrureakz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3udfgmrdh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3yxoojgue.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zhmgboqk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jqtcwnij.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twundfqw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3mafollsp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3qknpktez.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lpckeszl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3epnqvezd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3dmypnmcg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xhzwygqf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3bgltzqec.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xrffvttr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3swwqjkyf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gwpbcqoh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xjerlqkc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wsfqiles.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dddnpjoy.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3qmgwieut.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3zzurbmqn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3oavczyfy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mfxowwgs.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kbyaotyw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ckuetdvg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3virbgoaw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3gbzdowad.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3lugcoqwl.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3rnfktens.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vckyqapc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3tlrbmqoo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tbovajzx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bkajgkwj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3jcgcldsr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3khtyptjy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3aiktbapu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gqlytznp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3mxjnqcdr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3adbbxeuf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3vevabmoc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mcdalkld.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hppgzsym.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mmqtwwdi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3riwliqwg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kxospuub.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jfxfjiyh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3nsuigxoh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ncwassxm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tudneahv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sptfrbme.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3kucrbzog.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3xkddnkim.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3alaitlee.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3skvrpfah.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lyyyhzzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tiutvtkn.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vfujyhsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asmigilz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3twnmpuvd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3fovckhiq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3epvgjzcc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3daytjqjq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vefilbwo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3mqgaddvx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3laxetyqk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qyqkwsaf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3snghtchv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ggnailpb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cumniwwr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3nlwywnyq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wndhogpq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vojsswqa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mockfrvp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zzpqqzjn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zukouhav.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gvmlwffq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3kwzwqawc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3yhuxxcgd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3clzstlpv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3efbkxobn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mhzfkxct.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3kcqcmdeo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kkbqoodi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3wqtjtmel.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yhtzakna.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vcqjugpt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hcqbksfb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xjftuvfa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3huvvmdjw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mfhxhmhi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3hnrxurqx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mbmrnvec.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pzbnsmmg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bystzqfe.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3tousstce.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3mxecjaky.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dyfeecea.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fpuzozvp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jllghisj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3iuuueplu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3vzakhgmx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wawabstx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qptztfns.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ciknoopj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xiopggtg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hjjwzqul.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jkewcdld.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wlzhecei.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nhtwlbnp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3elgtordp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3jxnflrrv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rbddlbtp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3iflbworf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dvrwpdaw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kdcpqhcf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ydpbshgy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xyetorgx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3dnyasnvv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ygjxegdu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dosyfuqy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vfomiqgb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lstlcbqw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ipchfusv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3nlxnsxua.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vbmlkzoc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oickncui.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jjhjbdry.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ljbvsyxj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bbqhpckm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3erwulldn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cykjbwks.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mpxmnpfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhppnkcg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3elzbaxhc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3autobwjs.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qyvukfjc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3akkxoeea.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xotkjols.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rwzwxsuo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uohgitra.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3whwdcftn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3njbuwjep.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iqullqru.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dclsljpy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ffvufufu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cpmejzaa.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nxmnvstm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kdoucegl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dhosakpc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kdmqoywl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ckzkejxm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3anvidrep.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hshtosmt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3llijtdgd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3semvucbh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mcgpnzag.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bhlzaktb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3dbwxqrer.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pnepypbd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rgwlfpdp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bmmgnlnx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bcycdmqb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3sdhaaikv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3etyhfrzf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kqxquhse.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mgzczoty.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dylnoywf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zcezdmob.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3wuhczrcy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3yjmbdlgl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3imvpcqzr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3vagamwrd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vicknxwr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwavczpv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zsyrpfpj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qstixqzc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wtxiaafc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3uyvcrmro.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ejzxrbfe.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vovtrahe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jclksnty.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iwyrkpoh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yczvvnws.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gkfzsich.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ihalszta.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vcbrketf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3okoeiyzr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3aohvnhum.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qysexrlw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xwxmroxa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jismelhh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xruqkisz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3egotnwhu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qrvjiwfh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cstwjfpc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fshyiqyw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3udepvsao.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3lctgkvwp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3rqgqbdfq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mnoazdgp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ctviaezu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ydwojsuu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3filzwafw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ptrvbajc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gdabincl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlmwbfeo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wruggzju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwlrvyra.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fxaqllrl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmhvifgd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lanxzvsz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kucpdeot.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wgclskyo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3foizkcoz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ignbkxiv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ybktisse.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gcqjgxlu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rtemeqmg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3reumtgyv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dmmxctiq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3truatgtq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3honoyikf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wwvjskqq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sftdphyi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3unkalhqo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bwsuphjo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yrogmcwj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3uutruzsn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3baijpvgq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3blardcwb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kuiynfbs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rooghcat.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vchxhfna.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bslluzdi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xfsaqqys.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ulnbxnxz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqezlfav.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vqwpxnvl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xbjxkcfo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eervefgf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tgsjltdn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3eqggpoiq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpeppebk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jrokimvm.html


<!-- 参考信息 -->