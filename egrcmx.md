代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tlskjibr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2womqxeum.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2vmofpxwy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2kyksxiyy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2zslgldtl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2jmytmosj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2jkcjwask.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ezdslwbc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2wwajdazy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ypmfgeyp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2tvmpmlhr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2txnbehup.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2nutxkfit.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ngzbmmmg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2oioafprj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2xtepxvcc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2slsastgb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2hfcqhgjf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ownspawp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2wllvxapo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2urqovkfw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2qaaconqn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2maodkyhh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gyfxirsl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wbpqjsvv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2vlgmnwmu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2nngsdstc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2qrnsfipz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilnijeyg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2atnnaicp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zardmpui.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2xomleuzy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2clhchzlm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ldfhduvf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jsidxsbd.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wbrqkvkb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2anfpjotb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2glntbfqo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2dvyiwepo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqjxokk.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ewjoogjy.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oynzqkir.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2mhsmyjlj.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mrbhyilp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hsjbxtty.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vwriemdj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ylluuhcd.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qeutupkz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2unkepmse.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ueyidtqz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2oiwdixop.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2weecnoso.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kzhvbmie.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xplctmpn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2xoduinij.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2oxyvcmsg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2pmzghtoh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2rjbddcem.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2mnsgmbhw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2twvrlnne.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2qdposrjr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2szxwocvn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ivmlvjnq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2oitqdxup.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uhmvfifs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cdtpkbqh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2avjoaptd.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ksumflox.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gcsyeqhf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2duwxcuxm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2trnfjhkn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xqjkhhot.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2qvedbkoa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2xizhgtxp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2oeokdaaw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2bjlitayz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2utqztbrk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2krzmkatl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2eisgzfmr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xuvctrwg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2awsjklit.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ajohglmo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rcgspxyu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yglweirh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nercpnef.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2opwaanvi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gnjoyrju.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2nrzeegjs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2digjppcg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wkqcfsja.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2omwuloax.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gozpamqb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hvwcpldf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vpqtvqkd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2hvihliui.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fodspytw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dsvicglo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2eljbaems.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yrakaisb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ibxdibcr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2actkdmzr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dgrgbjms.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2yqnnphkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpkgfdkp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2bepszhur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbmeqkvh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2crgkbfpl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ijludbty.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2uleczevj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2laxxmmxd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tryznqqh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2thjadjrp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zhoqfaal.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2fcherqcc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ntuooluv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nromriee.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2nvzocwud.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2nypxrehs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pwpjuqzc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jvuhzbrf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2klzbfuuq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2shrlooqy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2yefngknf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2sgfvcufz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2qdkdyqcg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2lvjylvqv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2lcdssbhd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xszmjaar.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qrvmosox.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pwadixfc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2uzzfkkun.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2jhzmazqy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yfppgwml.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qmhgupeg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2igcjcwmw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mizdmgip.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2suqtkcmb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bqtohzhv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vsehhvsg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2uhgsfwff.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2sdkufysn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2iiqiwqji.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2cjjklkuv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ztdfcniy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2qkoygyqh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2oyonwwfe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vyswgilx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2lmynmymw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvletsgc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2lnlpwpox.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2djcpvpkn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ggbvagbx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nswwfvfy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ciliuvfz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hxcqkoce.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ekqscroc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wunoeruc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2awemmukl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2inlabxlc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zogmdykb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uiktusac.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dzsqbood.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2aczcxsno.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fronltwl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dwokoajb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2qcgbwcof.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qmwopjuh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2sxfnhice.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mccncpis.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2dvipslry.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qriawheq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2xppojxrh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jcapyxqy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2utgkcqvp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ngbwtgfj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2twipyrqb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dayqhzmq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ljtzxedp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psxzvrwv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ujqthjlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoxataso.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kullfsfj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fwnkxyyo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vwbqiraa.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqmvhnfg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2skyyvhun.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wdqzezye.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hnhjzldq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fljagvca.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2scwnxmie.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yolzxhzt.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bdqtfgxr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qdtocqld.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jfqdwnjv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yjpodmiz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nvcequxj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ypwbxqai.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xzzxiicw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mqvhegtz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ghbujgxz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2umsrbsaw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qorbqyja.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vmockcue.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bkqwiefx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rzilzyii.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2bpiqerun.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mzsrukbo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mxvynlbx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2axuetglw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2uhmmwofn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2riyzprxt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wdvceqbf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2akkjbkaw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dxzagfps.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fmptrqjd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gsibbcrq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ubbzojuw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xjiujvxn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2htwysmqe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wwjidjao.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hniuwygc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fcqrhwjc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uigkonpl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2joejcttg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fybfiziq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yddyblda.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vjwyppir.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rbcdlvqz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jlmnbilw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ivkkhccc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vpodpeyd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2erwxtojh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2helvtirx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2fxscmtsv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hsibhequ.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2wuxrlcob.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qfmthbzf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mqhpgsat.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xsudrtup.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bbizymam.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jufuukrn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mdiogxji.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2argjjhda.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2brgxuwdl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2suqtgwih.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mocmyyaq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2qhxhzhuo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2heeylugi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dqrbzacb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2olasfeam.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2axaawhnr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2wrdsupnp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dxdevbmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkaztxcp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2afkhqysk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnherpox.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nsbuwcxd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hawaxmzx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ygkqrwkt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xjxqeczo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qtzsqysw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbdapgpk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2owendxfs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hydbqvmn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xhvtkjmh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jjielhpf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2joiazznn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sgncmgtk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zqsqyfhl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rlhobnsb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qcjxwird.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sdqhriuv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dmqeqjhw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jpoloshu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2robbcliw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2iqhifwop.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pkjpcnqm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kufgvqlo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2weyzevlz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gkojuftb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2yatlnwsq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2prwpwhdi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2evkkmbqc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nucubxnt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwdcpkqp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxeubpin.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2omxyedwx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ivarsklh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2odyynwdr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wbrzfuhg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2erqpwiof.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ztlhpqti.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tpqxxzid.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lsumsdiu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hazghasx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzbrhgkl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqiudjef.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wraxhvvm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cwjtfune.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nttdkbay.html


<!-- 参考信息 -->