代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fckqfcpi.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2mzvtustw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ymgbzxcb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2vedopbrr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2enobitmo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ijrphpcx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2bdaekpay.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ebxxshue.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2mibjpjzc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2obusphtb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2sddnjwez.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2jnfgzrkm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2zvqimahg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2vzyezjxz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2oshabtvg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2imwtlmxz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2bkledtfx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2bflchwlf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ctrioipc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2djuqhbkp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2avgvolge.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2mbqrgoec.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iledrvih.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jemrcxlq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dafpefss.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2eifpsfpc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2jszgezti.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2xbjxyhjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xaqvsbdc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2nprptsfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csearnkx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2dafovasw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dvapktwf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jmgstngb.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lcddhjze.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iysyjzxl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2kirasasd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2nphhkeia.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2kpuhlinj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ncasdjkz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2pnhhbcfx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2mwuvnegz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2nyxxqqgj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2upchupdw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fsaeezve.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2talzdjah.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dsxmkhze.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nyzfsqec.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2iuwcwyma.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2hpadkmuq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ruuehcte.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2gcmrprkq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynjrzabf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cocqzprr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nyhifwlo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2wargnzst.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2crpgicav.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2zdnfavix.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2kcbpcjyi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ocioaxha.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2hgibjphi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2fgaosvkm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yyifluim.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zaacovir.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hgoafsix.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fyhniqag.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mbmzsmyp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2zvacyehr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2chhyrdei.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2eddaijke.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fsplhwww.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wxrchdbh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2kuisqbnb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gtnepfyf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vwutikmz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ipqirepm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2mubejuku.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2txotdrnr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ezqnsakr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cfsqjmsb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2csctcweh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pnrhpkvw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cftxahut.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jxjbsrqp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pdziaqev.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tpuxmzko.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xqctncwo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2hulpdlcv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pqxbvefj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mjxuqgwj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lmtufvgh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2byzdzveq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ufbmxirq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vxvwuopi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2houasqvx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vmapdfmh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xnncqpoj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jmbhywod.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wzisxhmu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2czxcdtdd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2epjitnia.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mpapmvil.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xyoxtyjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyvcngud.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jtxldssv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rduuxbsh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ykdiwcgx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2dxynhiof.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2edglnxgy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cqtrxznn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jzeedxaz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2shobrnig.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2sdwzpome.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2bjokkgvp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2whnyagee.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ingugvhy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ifagufsn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2objqmwht.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cmbwfvcn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nekgznfs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2srrcqvqy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jqnyyvrp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fyzyxlkc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iztxcjoi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xlknkrvp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xxztxahd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fihuwsiv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lzwzoqrb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fhssysib.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2doqcgpaz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ikgzyvrp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2mmtrnqkt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hbcyiplk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2wnepnzno.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xhgkqvdb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sadzclak.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2okeavthk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wvhaxncr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2gtsmjqpu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zeueswsq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2rhlhnbvl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pddvseav.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2udtphfhf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2swpsucwn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rfxabesy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2klrwfuav.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gddqxkpy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2unjethjf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wqyncnky.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2dxoarrzo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cgwsstci.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2itoegmvs.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mlvebuzi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2tqadadpj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ifuiblmf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qpbiaenl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nrmemzcx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qnkbkqns.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ehwbbntg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2chhqcrhe.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xrhioxlt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rsbvytfd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gkcpozsg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2auogzrcc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tzsagdzb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jdmayisp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yzpjisrc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2llmlapmq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zpuvmrnp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2tjtxmziv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vxmrnhkf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2fdolkdbl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eexqjyuc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xxqekycd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2pmfohofr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2cuihtqss.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2grynrwjw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ftxrswdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsdvucow.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xhqofkrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxdsaptc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wnqxjbda.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2osngnqlx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vnsgaasw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2sgojewxm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vqcrxtlu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mcaevqap.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2hueqhtfi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jhtoghat.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2oywdwlwa.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zgkvmzyw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lbbgfjch.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ofvmkfka.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ywojuadn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bwsuanjm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uwqvuccx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tmdpqtgh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2plgbivri.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2egvzzyux.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tfmxqgdx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2plhahmoy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jowmxoel.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2idzmpwji.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qwnjsliu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rajfyidy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2khkkpzxp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hivpmymu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2lbhnpswo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2chghabst.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tjfmyojg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2wnemwnqz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rajibjqz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zwkfcroc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2kkeminmo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qrfdjcop.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2yjkurofw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nfopflps.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tjmnbdgm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2amlfktbk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2idwdbxpg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfftzmxe.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ulnwynke.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2evdeqiul.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ecvklzqo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxizynub.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fvbpydkz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2rzwaczst.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qyfvwknd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2izglheqz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lksiqrws.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wyuywjea.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rytnornp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jkwtvmdm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2aecbwrkq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cwohidgp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ougzehze.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2dtjsxjxz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ccgiaqsf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rguzaebf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jicvbcky.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2npgjxgdu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hdytxumr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2duyqwytn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2madrnfkf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2qlifamhn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qouqpvjk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mmcwzgms.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nhqnnlul.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2roaqycco.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rkfuhxne.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2sxeyhvep.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wqgxkyno.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2lsyxasyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osjhlqyo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qsojyras.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdukgwyn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gijjlpou.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dphysoyw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vqrduiwx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xecvumie.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rvsjwpaf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mpgilzrp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nmstairg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xbprymss.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eqbbuxtw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rnmemubi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jjkdsudj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sjtvmpxu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vskcfkyt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ibusqgxj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qvojqmbg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnrzsyfz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ylvkelhd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tyiaulqk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ekavphak.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2buqnesac.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ceqnhsso.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kjucazjz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jhzzqoge.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2lqyapvru.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dmcjulzk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tkeyutgi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ukrsvfag.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wanswxqu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jhgmytvx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvevlhal.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fmkutajv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gweaennj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zqzmoyua.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rxjxllsj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bdmopqnd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2igfzipjy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mcfnzfki.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jkqcdxuf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkrsqcyt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wiczhmdc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hhsvdcrs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2dhavpukh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mrlvxckc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2awxwinzg.html


<!-- 参考信息 -->