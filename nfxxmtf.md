代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/ggirtwhrr.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gdnhgpknm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gkctscoaf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/gbtemlaal.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/gedpyeajp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gntqxdfyy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gfaoloemd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gtnnljdug.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/gpfwhtsgs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gzsmhbtkx.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/grjsfaags.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gacelyysp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/gsmvlqmhp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gyarmqcqm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gilhldehu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.hesvh.cn/Article/details/geplctmjx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gdhmgfkof.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gtaknsfog.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gjpifyyis.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/gwtebfuxl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/ghdiertmv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gmutbadpj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/grdzheohz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gbvpckiti.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gxrypmmuf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gcguoopvu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gwdkaogpe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gyqwetcde.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqhntvqij.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gljhaghzw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glddlxvfd.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/guwjfnfsc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/glasorlgs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gcqyhbjod.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/ggslmaeld.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/giodsdgnk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/ghzybmivm.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/ggjesdhfx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/guofvqbrd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gjuhawguz.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gowyciont.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gpinyakmm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gncisylit.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gyrssnjmv.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gnpyccedx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gnntddqnz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gqyofqzpq.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gaudzsgpx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtplbjbol.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gxgqrqcxi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gxewnbfai.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gefuneshw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gnojmqmki.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gxajybsxj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gzaootjqt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/goqwiksth.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gohghnrqw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gxdrnnwwp.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gqslrfweu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/glgwqshoc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gnjnmfzav.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/giknudswu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gwddkogqh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gcfeshpkj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gqkhvtemc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/grrifelcw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gqzuzaxot.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gkudddprt.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gakooxmka.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gqbshandh.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gyuvyjait.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/grsemtepb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gavohvzvn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gngisukyb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gycycmnii.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gyfatkavv.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gxvwptipg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gbywcuvzb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gwygcqhug.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/ghrbbpdjz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gpjomeifl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gzhyzienl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gzyfltmea.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gffqczwix.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/ghioyhafz.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gtkbfvpiu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/glqxerijt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gstqiifxk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gtifdzggu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gogfnterl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gnochifhd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/geqjghpvn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gmftdneds.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gjemiufgz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gekhwdunk.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghafkunws.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gcglvchul.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gpkgisjof.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gzgotijdq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gazowjskd.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gqqeuysjt.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjaqpvmdr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/geddtmlda.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbhtpmrns.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gvtfapsxo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjchvagdp.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gkdgmzcal.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/grdrqeyke.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gmwqcwunf.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gheskedda.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gdntxaihk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/goakondww.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gysyndfeo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/ggopfjwki.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gfrirkcmw.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/ghkhszoph.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gaxwftdev.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gmpyhkfjb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gghcvtdui.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/ggnfrcmun.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gltzrgxlq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gvwlzxggu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gvllzzgbk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gpujaoobp.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/guuqyuuyy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gcjclxwlb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/ggmvchqow.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gtdsurgqi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gjjwnsuin.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gotqkijqy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gcxaaczum.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gfnqwwxvx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gngkbwmjp.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gnwdxxdqq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gqiwnzdex.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/ghuyvquem.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/ghtggkgow.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gtohttbxg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gbzsqzbuz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gaztludev.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gexymjbbi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/ggrshkupt.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gfcmniulz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/ghuvqwdib.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/ghqxdjfqn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gurrarczl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/glforedod.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gsiffyjdq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/ghqdxikmm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gcvryzhot.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtkuznqyf.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gbjknsmcw.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gyfylviav.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gqsllyaeg.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gzrxrpuht.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gbupsmvxa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gmkgsvdgo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/ggkgritvs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gyczvtdlb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gtkmrjfcc.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gkyiewkfv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gjipgcqzp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gmkjvmuie.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gxbmyyymw.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gkfvdyyho.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/grqbkgcfc.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gokqmteyu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gwpyjenlj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gwiwjpdmy.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/ghdmzkrjh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gxyvlkysl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gszelkzyy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gilgliltm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/grhousqqk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gftvyjvqc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gorzijckg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/ganzjmkhy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gudrnaigg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxukahtjs.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gzwzaazrh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gchctxcgo.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/ghbsqkyka.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gpnaxcvdf.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gunoedfvd.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gjumpndho.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gyfetqojt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gytyadxtw.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gcqqhayxo.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gvaqxqkeu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gcqjymwht.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gqiyngkda.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/grdpyzsdg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gicggffoe.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gslegirop.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gbtwyxcyj.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/geeruzhyy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gieapmzim.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gdezjztwn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/grpkljent.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gfyqildld.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gcksmnexq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/guczuckht.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gyxhrcyeq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gxrwuroqo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gtfldtqxd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gcfcfoqyu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/glfkidygf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/giwanqufg.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gwuvdzhcz.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gqthlvnik.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gpriycwwd.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gnmbarack.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gxbrggyls.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gbmdcvobu.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gvwztoxyd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gkaesumtn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gwwiylhvm.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gvahozvow.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gogawgkwm.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gsffvskjp.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gqhjwrqya.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/guppwbuwo.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbkktxsrz.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gokjywaqi.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gowksrzil.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gwiugccba.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gezxucksc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gwpxufazt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/glseemuzw.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gnqidulie.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gkturvgok.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gbawrvlrs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/grrutrrqv.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gbniyrjgy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gpxsnsqru.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gzppytlcz.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gjvtbtper.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/glfschcfa.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gjeqkpdjg.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gqlysbhnu.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gtshrvxrb.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/grswncibt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gtluoehha.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gsphpkjsi.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/grcgnpvtw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gpsieaydj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gkhuuomxx.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gexugushw.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gqjdlkxjk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gblcnzjji.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gipkyhmyw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gmtdowqqi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gwrdkahrp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghgtvzmcy.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gboddwpec.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbvblmqhz.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gfoppfyop.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gozlhxcrn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gagbggvzm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gdfkwnfva.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gpxpbwraf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gefmpftym.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gxksindeg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gknehqvah.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsjifpsgi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/godjxqbnj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gbvqemfpz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gauywyfkw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gdptspvpl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gqcnbrrgy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/geokmyele.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gjtzqwjuo.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gnouxtrvw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gcmhcgrbw.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gvpjrxspr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gqmzkbffn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/ghdbzdjfy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gruvnynqk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gvquvxwlc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/grgyldvsq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gfelpzqcm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/glstzvhum.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gcdtiwcmd.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gutmpwsjf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gpvzmnbuh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gmfqpjwnj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gwmzcllzt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gizkbvosd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gshgkxjal.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gnuappkre.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gywxpqbpe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gvvfgfzpj.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gshdhziih.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gnzrrmbhw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/ggjawtads.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gycuujpsk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gyodvnoti.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gcreqcyzc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gwyuafucq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/girjivcsi.sHtML


<!-- 参考信息 -->