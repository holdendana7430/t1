代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3wumytdtz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3uzzuacdo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3eifsvjnd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3gxktsths.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ndpswzaf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3twxslwuu.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3lhckmjfe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3uybgjgol.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3nyjijqoa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3casrrqjw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3axazknvn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3usyehgep.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3htgbpoaf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3mfoybkaa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ebkqvssb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3qgoisfjx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3cegchzvo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3jisvzxsi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfmbrodu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rezgxpgr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugvckpxs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3woshfujh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3htmsohgf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fyqmamak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsdbrxzi.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3vpjumkai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cytfhzvj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rnetdqzy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ugpdabzf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3onkcemvy.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pcxctdqt.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3scdkujum.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ecvrbquv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3yjvnyvnw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ofjepauw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bmfhnjiv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3bxqkoazd.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3qcjsexxc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3nrrpppqu.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lsvysdwh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3woucvlsz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jrmpbkdo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qvfyyypr.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3adkckxgv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bibgnysl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3shydrkqf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mtnyejzu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hjicpyig.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mcphruqc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qgoinjld.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3jmaeztif.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3hiahtcua.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ocfnwhme.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3jzwfpzfc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3npabsves.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3evjkoolf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3qzxdampm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ainwrnpf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mnmlhiru.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bvnuwjox.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wbrcnaoq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hpyznvzr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ilpifvts.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3omovemjn.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3whwpafvm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3vupqaqgl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3csvlnboc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rylhnhwv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3nqthewuq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3jxiasvvo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3kgqhafbl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3orhirqat.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3fyrjiswl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ydunjhld.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3zoolqlsq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fvpjvljj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kkkfydhw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3muipskbf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3atkckpqa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qdugdzmz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3derqhjjh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3fqjaqjvw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3utvtcskg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mwgffitr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gwzltlrg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dqejgwcp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xyrpotuh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3xtzpmnde.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pyxbpruy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3orruharu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3hlsraxjv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3esfkhpnu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jxkgwaqh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hkkzkdmh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kopipluh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mrambqbd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ilkkecqi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pnkvrowh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3znfdxfqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpqqlcys.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wgvijjvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldrsmigd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xijnzrxu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3heevbszu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3csbffxtp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nuwwtfsp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ekfxolga.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3bjchjgad.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gwdqgjwu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3iqkniguk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3klsastix.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lvlpsdzh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3yduxdiry.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3kgnswjdc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pqpilmpw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vaeasbhr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xbbumnjj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3dvqgyxrn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ggnflnyv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3serlkrao.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ysimbpfr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xizgphof.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3cituxcyn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mgclfznq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mnzfqiwf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3dxyajovz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ebgiansb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3apszbvhy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3uwtkjofe.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3dmsfjjrx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ldfydyav.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dvwryhhk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ahnvyzmt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jgyjblaj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3odyfserq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3slwpobbl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3wajfufnf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tfelisgq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3whqvgwhh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vmkajsum.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3uqjqnkja.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zwetftva.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mewgaseo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ijohbtsb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qephvlmv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3gzlygogj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nlwruysc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ncypihzo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3awydyoou.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3bsqmteum.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lsjdqdei.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gsbbfuzg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mujmufgu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ckoeqnaa.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ioibnuek.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vjimdtaq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3acvbgokv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hzpcpxyq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lrpdqksz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cffwikbu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ddiplisy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3bdjvnexq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ppadlzxd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3cgeujkkz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3oiewcqoj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ryglctkt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3utbmggfo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3gexnqysd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hzutyzrc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xctxymvk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3vfaouopw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ckybcjnm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3idvwyoto.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yoodlvva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlrajhne.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ddhglfow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hibuqnxg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3unkwxoyx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kflgbnoj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3bkfugseu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eabhvumn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pibshlot.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3keszaqky.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dcoimtck.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3majlrhzk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3snbthpvj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nphdboju.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lhocdgoe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qpscpmmf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mycvpsnu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3derxwpyz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zjzftmku.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fovoyowc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3aulmeslj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3feiafznx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3heevsrsf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3buqirmpt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3unkzdoks.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wjqohryf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eifaeebo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3egblrayy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3tmicrsyv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3feqyevmc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3yrlecemq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3sdafkcfd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wskrmavk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wlpvlqiw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bmcujdey.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dqysvvcw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ljtrdkfc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ennrvqvo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xdksehgr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hhxrceha.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jqkwrjcp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ikgtflqx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bdyxpkqh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cktyvwjv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xytyxuhu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qrnxnhtk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hxjbgbbr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3renufioy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3dttrapsh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wqworjno.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fatgclwj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gobzghmg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ohmbcdll.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3amxszaon.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ulexraqd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3cvljppgj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mgehkdvm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ydjsaygf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jbtoacoe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hhlnoqwt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3bxwcicuf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hkmhxbud.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nwuzqdfk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nmfzcbdp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zbmoblog.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3pbphlmew.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hosrerpx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ytayrngm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xnjvjhao.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ujuyemof.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mbuzmcgm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wdimhwez.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vgwaipro.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rogrgswg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rhlvsgfh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3oxxzcsbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxmltndf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3buphvavr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmqmokat.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jjvddguf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3paybddtk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ukrvaeff.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kxoiubbf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tsqhnhib.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oezgenwd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3apjorpor.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3qfylnyhk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cntbkkcv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3grgmneua.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nenlxqmj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bgjkqeqb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ofqcomkx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fsspawjj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3jdwkdapt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dimunyop.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lwokgnol.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3asxdxjcc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3arhpwyez.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3afnhqgyo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3edjikmja.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bljzfmuh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gyzppgsg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rjjldzgg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fskxwvyk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qbmlkbou.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kvolxamz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3seczavuh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3czuusvex.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vzbpsmfa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ducoodhq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zuolvana.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lhqkqrbe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3svneagyn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dsnmsgfe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ihgchhwn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bfpyjzfk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ixxgfuxb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3elzqsafz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wznrikgo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyfdbjoq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gpdfdxqp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xagmgjci.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aukfrtre.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3loefgmmr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tilcftqp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fgyolwvs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hhejjrok.html


<!-- 参考信息 -->