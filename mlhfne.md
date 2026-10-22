代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2jjdmqzby.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yohocacl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2qthkfeol.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hwcsubbm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2yywxcjxf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2vnrqxpps.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2uwqctaju.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gnpcrfuq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qsjlxsds.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2dentzppe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2tssnkhpz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2wkcqgfhv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ewtselhs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2yxhlabzr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2trtazpgk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2fsiltlqw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2corntqou.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2btmyqnsv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2sxfhbmqs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2xvgycmuo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ibmvwkhv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2kwixokvb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ludqzuzr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2kdoapyjt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2qqjriuwu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2ovbcczcm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2lbzgxnof.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zjnwtxje.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2gsthxavx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2yaggtqhb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ukqxsakw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bcjtgenf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwehxzdn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2zatpnwyg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ozmlcjzf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2anqfsfhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akgtmejr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2iynztjdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmnldfaf.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qljqorhk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2fnivazac.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2izksogam.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2judlxuec.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zuzzvual.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ccnqrino.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2alcxexwi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2truylfoy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oxttnbiz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2oxteerhd.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2jwpiqmft.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2byrnnmna.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vvrkoeao.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cssiydai.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pxwfiuyf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2hsdaoluo.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tofnmpze.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ebmnfkmq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2vkrdnmlf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jncmsfbv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jtvhvdmp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2veoyysfr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dszpsmpg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2arkfnolc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2gowrqqug.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vidgwfxx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2yslpsliq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhgnuacg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xkgadsgn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2xrstoyoi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tscmysrr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2coonsate.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xqpwkcsj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qkyapswg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mkvrozff.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2skcavywg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2patwzulr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2spivrtjl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2cbbuuiyo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kntxaadt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yjqsqftb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2qkhcgbrv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2huzxturr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jdeccihd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tlmnfckt.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2selzqfgd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lfcispyw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2jhifqqqk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mkhpscqc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2rsbspjay.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xjpkolpe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jbijjvso.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fmmfggrg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nftztqeh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2pqzkgiav.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jogppayz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2oramsjpt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iczwdipm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2suvdeoof.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pxsdnbhc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2uoixbycn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2juvneijx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fviocras.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dyamxcla.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2avzgahjg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2zdstilmw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jovwjwdc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pouztocq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2sfswhmxi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2bvoxmein.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uyfqvfxi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mydreldl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lretmwkt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wwfebkdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkkbzjas.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2yqhapgyz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2oxsomuvs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xbdgvovz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2gaevvjlc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bpivbkfj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2kqpsoodg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2dxrjriol.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2wckmegbd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xsjfslpc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pixnjlxy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2yzmtgide.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lnsauqeu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lmtkdpoo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ukyzsgzp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2lyvmspxi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ahxufkim.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2upmjjgqo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qhnccqne.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2oynzmxxx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2wpkgwqwu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ftdknkuu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ocnfqzpx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ojxxsdof.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cgcdxgda.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nihbshxx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2rjqwnroq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kasqgumv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jzpvyrpv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2cerbvsnv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lbqagxjp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2okzepyvd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2glmsexpg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ajssfqzz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qwxwfuzf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2aozgbnxm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hzyzwjpd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2rgohgtzz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tutbscgj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ehhplody.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2frxitjqx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bvdmbxia.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ipdgmphy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kreucrtn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ratnanwi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bshjfmmu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mekibfce.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xjpfuxjv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2nmgfjxvy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xhmcgmfo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nztyyvua.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xjcusubb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2soblrvdh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hhxjzecp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kaeljgzy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rpicxvav.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kcxynjuc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jutjnwdf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2asyvzzhv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nmgetykh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kskusaxd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ogvcywhi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2hdmjzcob.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dktuoyfc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2rkxnftis.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dlgvhfph.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2skciksqp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ptkoizri.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gwolsvdl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2roryxvak.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2awjnhkln.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2neavafmz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nljlbove.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ssqqeosb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jvpfpyyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2joivdpcr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nkfvlogg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xqtxmhso.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dmnjnvnm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tstehaha.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qqcoqtdj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fhidizfw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cikbwgpj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ptvwzieu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ipymkzig.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2crkyyevs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rxkqftys.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2aceiqifs.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ikmzqyqb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zxnaatwa.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2voyfsmot.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mvhoodyh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2rpaecezw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2skeorwuy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2sjlasacf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2yqdbxdso.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2cuvoneoq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ofwibxwl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xyxqujbm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tquhuyyo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2grbutfnx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kmupsvhg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vigqmzwh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fvmdhslp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lfwewolb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tvkkwuqc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ucirmvml.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2omweshhl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pauahnhh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2suflkmja.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vnqzlaon.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2omkrdrrc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gnadifes.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sfoarent.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2eialdbyi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xdemsnsb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vlcjpzmc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rryklgpc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hflgjifd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2onevaanh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2pqakdmjo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rrhxclse.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yqapvbfq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2gndzdzcq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zxptoaiu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2taxibbrj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dyrgdnyp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2yeioizmv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2tnmfalbf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ytbucmiu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2smcibesd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2btvvwhry.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2sahiuasu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ccadinyi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rhlzculg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2auyavrpn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ucauwims.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vatlaqlu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2uzoinpqj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kgrizhdc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2velygtmm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2lvaddgnn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pwodkzkj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2eeyphjlf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zrdfwbtf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ugsrtlnx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ljkaibpp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2madleqpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epwbwnan.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qojxpgtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hodvsquy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qopjnlsj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vulrpbpg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2reoarwnp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zpgehgwm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cqtxauun.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2thtcxzap.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fwnmtjnx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2obegsqgw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wkkqlzie.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jdibjavt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uzwztyyp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bblyimdy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xqwtijxw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mkacfqqk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dmhevvms.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yatqdyut.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2spqqmpdn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bmssalpm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lgisfarv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vhnmqsmb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2aehnsoag.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pgqsline.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qjuftctg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mvwtifhn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wkkmvaqx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zpfuubvj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ovkpdqiz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2xvlngmmf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vlzwsviv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mykmhiax.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hdbqjpqe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bexbihhx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pswdplpt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lzvbspbg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iyvzhwtf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xbhndnpy.html


<!-- 参考信息 -->