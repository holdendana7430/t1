代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3dmwxrvbi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3prusemol.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfojnjkl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hyxrvlyv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ccinmizq.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3mwldkcth.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3aczljeyy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3pmyygseg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3xzqbqtqo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3joqxxnqt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3kdhugxxm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3vbllvilu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3dmsapxag.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3gadhecgz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3mxbjkxmu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3gcmdcprj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3yqcpwrvs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tazczdtm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tkmngscz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3xegxtuym.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3iivnmflx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3xnbdgkeg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3spvffjsc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ganyvdle.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ermfdzxi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3akyguwzd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbuvcbgo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3trfitaff.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iokpmtoh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3hpikqxhb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3oyjsjhbl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3bhkieeja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utfautwx.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3xibrknro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntwyhcbz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3zenmnfgp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vxkllild.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3cssdjbsd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zckpyqtt.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wfiydjcc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3lfkwfnmd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3xezmbwye.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3uukcvmwp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3olyjootu.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jvpyjtmq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3eqhxsehb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3figscjeh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hupjetjl.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3loyapvdt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hzlqymha.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wwasluwd.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lzuokaca.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ikpqzeld.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xcqovyhx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hrgbzfnm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ctlukqpe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3rwosrvuc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jkixoiej.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3evdpoxxf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3jsmoiibf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rbwkprbu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3zkumagst.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tfyvqcxj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3pcvmlyyg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3rkrunglc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3lftiraqh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mdnwfrhr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnzswxa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3emzptyco.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cbzsejdz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kylyngfo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3fjskooqz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3uuqhblmd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nuigtqmf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3srjsjmzo.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ccmxihyy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3wrrulevv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3fqclhzbk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tiuyvomn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vjwhlfoi.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ltfjkzjr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3yrnumhvg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3nqfsuygw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3atlistta.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nctcyuui.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tiuokflq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rtacgtya.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vwlrrggd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dzmdxirz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3fuvejmxz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ibkavnqq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3yhfegtzq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yuhqsqsr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ykfbvoyp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3thmmbjqd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ksuljdaz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3uqmchlxo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3moajxqpn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3oudvaigx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3znhikzjd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xwusarhf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qaqfxdfo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3idpvoorv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3angftvpe.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ufltmacq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ogufbnpk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3evslxokw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvqctlzw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3uimprflh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbpyxvkn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3axwjwatw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3yqeblwmy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ezhzdquy.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3azxljeqy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xqcnoxth.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3mweytljl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vmfygtip.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3opkdljvr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xswajphn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aewiuhen.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3slndhyrb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tumkdfkg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3scwgodlq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3frslhozi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3pgwjdsix.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3wzaumfwu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ivsyimwq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ulbedjun.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fhrzotjc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3uwiaytji.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3clmzdvbk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uqbcapeh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3acdwdrcs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xgsvbmxt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fabynvyu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3otjjwklv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dvexfdkn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3xgjnkbtx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fbqwzjch.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3iqzgcubd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yprlmyma.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rpcnbmfs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3cclfswgt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3iwvrhdxo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pylowsdu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3rwqrxnws.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3isbayzql.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3dzcdjwra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3cjyialqf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fkqnklgh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wsvqmgqz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3psajagge.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3esvavtjk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nxknuaug.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3edufuicn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kpsjxxmk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nokdbtfq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nxmmsulh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wzfjeato.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3afavbmmx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bqzwctbn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ewyhjtpx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3kbaqbwaw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3eyjbcolu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hfprhsxx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3luekjvtx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3brymmcoa.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3crykdjju.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bnwbxfph.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ziitaedu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ryhsmhey.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3fmdpmfse.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pnsybkzk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3upiebypa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3buojhqhe.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ruhufxkk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bimyqcny.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3npxgajgs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3uvnwhhua.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bhegzgeo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3manrktgr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3icumbhpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxycbpjl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3pdoohojd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgtrscei.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3onbulwjh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nehclxqr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dhckbqdx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3raeapdjk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mbjhlimv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3doqmcwpd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ajcitwvd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ksqomagy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dxbflydd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3joveqwhk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wqcpjuif.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ohsooons.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3iyicqloi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xypaefxx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tvciyicu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nbfyxmwh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3raapjxba.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iwfqzmmj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lgfepbsv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rygknzke.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3rnoxbdcu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aizituwq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gdrxmztf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fioetlef.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lgyitgue.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ekebeaig.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3iswcdkfz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qvckghdm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gaokvxeq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ailmhswg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mrrnnetj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dhlszekm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3uoapozro.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wacsonlg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ciubqldg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3axrqippc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3habpsuip.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uwqmodaa.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tymmhgxt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fyfmnrwt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pwsqfksv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tgoobexl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iccakxeu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nubvnokv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fuyiisfe.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3fmnlbxht.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bdhawqdg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sewxoosl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3smmiictw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bkqzawxa.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ovzlxihi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3oawjwgzt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3heminjad.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jmozpfve.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3tzgisngi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3pmfdaayv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3glzwmtth.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ajvrytoy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bttxhhzz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3oqdkxtjh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zgzglduv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kbuesfsk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3akfqncgw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3avzauleu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qokctgjr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3bhuxmlkh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3epewxnzt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3obanqhuo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xfxuwomd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mibqmsrb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3puvtprcn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3wynyblim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpviaspr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3izliexbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izvpxgww.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tjvfhjlw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zcdogwrc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wiwrckfi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3edvjmyva.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3odxobcdr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwmwzjps.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xnaczhdr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3bufxgeoy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vpjdqsgi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3bednusqx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mzlcwcsm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ysdwslpu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3svycrrqu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3whookqys.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qegdrimi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pjsjbtoy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3liypnjki.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3czyzimyu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3cpwdwdvt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xwpqelbz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vgvsddmp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vqqmqzik.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ruaattlz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3avazeucy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ofvjtmnb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3trtwkunc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3guhwthqx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rstlmplp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pimktwwb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzgjlxmp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ztwcuwzv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xiuyiwcz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3uohmbgkb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3rtadkbeb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3edkomyrv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ytpfvbce.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kedwzjxp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gmyggzdi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pimdekdv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpfyglrx.html


<!-- 参考信息 -->