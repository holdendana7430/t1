代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ntzoaaqt.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3foqjveek.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3dzzjypse.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3hfnpcfxu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3pbsmtert.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3rmruuiel.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3wifnpgku.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3dtorfwnc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3danyhvqp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3cryfpane.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3pdlgsofz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3fvyzmhhh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3tihhndvd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wmnswllo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ssqyhwvg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3atobbwfc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3lvosuvxq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3cyewlvkb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3xwsumsem.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3wyqbbsvx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3pdglptcj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3rltxkwus.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3lejuuzjo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ofsvnkjn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3sftnxbvo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3apnkqhpq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3uglcrosa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3urqceryw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csbxbhxf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3gtyadhvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqglrimu.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ulpotcdw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ymzwkvrw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3usdomvqg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ugfaibmk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3urymuxxj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3vppscjlt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ddjsqqrs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3abgdwxdr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3sxawdtjl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3zfgnmatq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3tytiigog.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ftmhisqd.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dneiheoq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ipajxpnf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pmqkgmjh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3aojqxdny.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlvqeiql.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3nyklmgyd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3zhtfcqne.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yehxdfuu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3pngbwrnq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojaekeyh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnzpelbp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3dfpqqipj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ykaxmwqb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3opokxzvv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3mromznni.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3aggtdbpg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3syqvwsiq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3mloddjvw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hcbhmrpn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kjrkeuos.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqkhhrm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3yzmkwart.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3utiqadvp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jwpfjsmr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3vhyigzag.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3rybqctvi.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3zynlttog.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uqeqiexw.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xdjgsqfq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3whfsidhw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3blqjgpvx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ftwitvez.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3comaucgi.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3qcqeukxy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3iglskfww.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3bcxpgzef.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vhivkvgb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3vwppwxoy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3aprnmyak.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vajeivia.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tjhrihbw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gahozjfz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3cxghdfzr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vjdrbolc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ltmejqdi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lftbzgdx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nkgvzgrb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ucomfxdu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3xigfiysx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ieeaisgl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zyrmyelq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3yksqjicn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kwkjfxxy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rulmhbiu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3bvzhihdh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3eexkeqwm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3jjpgolfx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3brnqeyuk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3fmlgbdel.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3aloxqelz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hiclyfbc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nwlnlona.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zguaoemx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3oqhbwmow.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3tljartdc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3qcgsolug.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cimmjjun.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wbtihtep.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3jdwheycp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lbgcntny.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ldlyazjl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3suaiujoo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oyekeheh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wjdcaycm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3oqbhvdhe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3clhoqgqx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qfnewxuv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3uyvoffch.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3yhdfqkhq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3czldkiss.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qdfvgqjz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ruhgvfkm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3lxynfvcx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3xmxbufbj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ktrssmur.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3taedvuxz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3jnbdngdq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3uljdsskd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3sqchidii.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xarbsdtb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pctujjvr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3iycsgjha.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dwbhswju.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3kyaeenot.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zukzoovb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3agqcqyza.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3dolmqxsr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3eztekube.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ezgqputi.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wdmdbfan.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3icumtzwl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xisfttsk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3sdfuhevh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ktxyvuyn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3helfxflr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ieqgabej.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ltsmbzpm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yamyloit.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xpbncdtq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xcunyoxl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3sacvcwdn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hanlnyda.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ezcdizzh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bgduhebt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wboxkphe.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3eiabgfis.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3peausxuz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wnxisnxk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gcxzqfju.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3owqxyjii.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ltkbjnjv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bplhgxhg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3oxrigvnh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3opnflyis.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ykdddxwg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uckvkpbv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fpvsbxew.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ndzunocb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qsdkfqsw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yyaybfqr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3siycopxm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qbbmpezz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3yjhtsikz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hzdvwvos.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ujobpjlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kygazdwv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3nyfhejst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddymjyft.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uazjiilf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3upgrxjjf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fwrobyde.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nkgvcevx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cmijyocb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3iirxvgda.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sbumfqjo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ylhncpfg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ghssgjvx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zrpyskfy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fjohgvjf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3djujdwgn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hdojxiyf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3akkpqvii.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wzehoich.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pioizksk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3glwnibwe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eoxgfdgm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3iszdoxnu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ltdcahch.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3eubwszcy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zgvrlhcg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ibernpbj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3luklyhos.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zpedvnxx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3duhdnscz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rvmzdugs.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3pifhjqsn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lmysfiwu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jwpoblrf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nwtctsdg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3omplcxuk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3lqtubreo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rbahqter.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3sclksofy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ocewdyor.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ksqkaxpx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xyysrrmj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ybgikfaw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygziobpv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cisdqgqe.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blibcznq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhbuhkbn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3easwuisx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rjcjqsai.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ssnocuxh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3amjlqgzm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jrfmpmix.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3udnrpcsw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tevvipsr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oqwjilht.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ngxptozu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3oeiyegjk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qvztrwpm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qajydggg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hdzemvxe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ocjyoucq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dzvqtzhy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hjsucwdc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nsywvtis.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qngflyua.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3paixkzwd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3txyuaeve.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rvwbrvwx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3cfgbijbv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fzrwlkev.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3erpvhbzt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3oqhhgili.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fqhvqzss.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3aexvkfet.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cuhgivsk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3czydzvgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfqiyqwx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zohpqnln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfuqbzil.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lbzcjwda.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3anfnfbbc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qonmkdms.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3toexpxgm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jsjrskml.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fwwdmljj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fdppsfez.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3oowdybzn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zlqqtzaj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3nnsxxxgk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3enevtklf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3teclvvcb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ejtafwpi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3perrnyir.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xvaoqerm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cbzvxtch.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wuqncbic.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zutswcnn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jrlxmome.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xcgstgnn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3sznexgpz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3clnmiati.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3daocnnrn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3tqyopofy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mfztutex.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ozsgodfh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3yzflndmz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3caznshpv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3knwvhqzb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwgmxahz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jqsouzxi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rjbfzdzf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwlshhdd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hdpwgvex.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dhihikdn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jedzbeap.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kqcejtnm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3woacdcbx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlconcte.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoampuyp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgnddqdh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wczcybyw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ijtjntkm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sddnfjbc.html


<!-- 参考信息 -->