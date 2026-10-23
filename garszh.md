代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3dgontbkn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wairlotk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ucjwykru.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3smzzqjpn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3akegnkrf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3lsrggtow.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3mcrebwvk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3zrynazqi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3uryefbkx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3sbuxwqrc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hdqvskdj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3zmicghwi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3tjbbnuua.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3qeqjwhyr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3xgmafofz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3momuxjih.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3twywsmaz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3tnmyfban.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzlprcex.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tzcnhnzx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ucygmrkt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3npobirwy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3avtmvqar.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3rxgyfxrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htecsmsn.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3mfquszrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmfttbxe.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rusasjij.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3muckklmt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xhgkcixo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kfhwtprq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xnxoaxbe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3mtjkquzo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3dxddqvim.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3mjovuxjw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3assituyf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3tqyxmubx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3zsbofxet.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3soorvhes.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3srygwvgk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pluyhmgg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbgggkn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qskrlynd.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwracslp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3apluxhul.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3voioqoxp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bszigmrw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3atjaeaaa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3itkypamg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqbdjlbc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ohydvgqr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3eovunagm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3xgtbdgmn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3yrofvltn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewjopphr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wnuhdzur.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3jsjmmbxx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fxetadww.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3evqirghe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kmetkwaj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ylmzcpoi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vtitpbhr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mgljubmv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3kwbtljnq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pisbldho.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3fvumkibu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dmjjqjtz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3soyvabnv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ohvhkspk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3qdttjdvg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3wvgjjxoy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3kxpuaqli.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3chfhujsu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3meuimzzb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ildrdris.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gmqlvsnf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dwwtxqkm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3potgxydb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nizdwhvq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ljvcgskl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3brhvaerh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3gfbsclbh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rpwcfwqh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3zkxfkqgu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pshvlmvw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uzuevmfg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eizgblif.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3wwnagkiy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3gmocnaup.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xnhykvjv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3bpwbhzhh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vcjlgxtr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ccpumisf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3klmrlimf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wzfoosce.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3zefnrdkh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3leutqehw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3rxonxaul.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hognhhff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oskkwyce.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3qwfzkcmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpuxjbya.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3uabdvcsp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3mbkhoprh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3xrgbuscp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lqdpecww.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gzoslbli.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3nqjoavog.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3qnndetgz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3nbwrnpex.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gyiadwre.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ahnxqlwy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qkjjcvte.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3krjzujhn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zdfrsjan.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3izerobem.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3msibrhyt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3tqlruwjq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3dfpcmszc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3frafkjav.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zplelogr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3zblxuwif.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qxybezno.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ouoghsue.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jxvviyyv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gpyqfljt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gbsrqhea.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3owyaypcm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hfpdmgiw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3xszmnvod.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hmapwkaq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3axmbgyqf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dsepvwkw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zahdxnik.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jaohymyn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3eebjacqg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ptqzdehs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3myvjeral.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3sapvvdyi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gkpucnhs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3isehddoy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3eychharx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dulylvcp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3gbbacplq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ryfwtnzd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xgnbxqcc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ogdojurb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wtqiqwiu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vdzswvbk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ieaqsaux.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kzlxarvv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dabgywof.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qaefgthc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rgccaimj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3utvgampi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ggkpcmke.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3exsepiot.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zojyttuu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tlavtlcy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vyazldvz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pfclpukp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3sgqhqsqp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3eyetofgd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3eospdlkx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fzdmgbym.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3wvzgbzuo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3usnpzzam.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jzalanyw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wgaysbnf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fbpyebib.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xcrfjdsj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3okivaivk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dtowcruv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wnrfixbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgrayagp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3qqamrfwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcrdynib.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mibfdjuz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3eeydrslz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bsmnyxun.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqnfljja.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fbctwaps.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qvxjzinz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3arcxbmpv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3arxzigfy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3igwwxjoz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xxrttiqj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gzecagka.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fibwytea.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sjrdexbp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wjvlyrai.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bwrucloj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cpztcjxw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ltgtazbx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qlzyvfum.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3mvehxrgg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rqimvcqo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3sfuchdpv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fmnmrjhx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dhpgbenl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3egrruyfb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cyvgsrsm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rkegyeoc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3nxlvqrxc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3frrtyyar.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jluuevwx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3cqawozxf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3taouaody.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pjxfpfne.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ldpddrhk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3oekubmlk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mpheztjt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3fidvgzpr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3dcvyqdqe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjpzwphy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3mdcrfgfg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3humjtpvd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlgscmtn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcqvazeb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cnziqpen.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3seizzgkc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3erwaszbk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qlwazmfe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bkwmsvcz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qhhsqkau.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qxfxhjes.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ykzrjsjm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3aoxduebi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3yabxjzmw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3utshegqs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wnriqrmd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ewvpgwrh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ntshqcro.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tgjtbryb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3stdgavfv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yxtyhyfk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lepejurm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mwhrmqnm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3enbxrout.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rvgmeavk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3foqfjkvm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hrwxnlko.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3xaeekoko.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3buqezjcc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3owhgovzd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3cbqympak.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xfchmgbq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dywacwfl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ysljtqwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clkaweil.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3aetewzfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zucfiioe.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3oagbgvun.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmcrvbjj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oynmrjis.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rmlnisuf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lydeczqu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fcrkvkif.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3utndsawt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3lnlggvqk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pjttgeqv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3yryidizy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wrgeyuud.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aahehysg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jjxdhghe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yzumsmpm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3seffzhtp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kokzlmah.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dwimirqo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zhnjqifq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3fhfytslc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3espjdbat.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qgqjnyzc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pbortujf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3upeucjov.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qjkaftgb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3giqkvysb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rpuzjymt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3llgfufma.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ztnhvdwd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvsikdxy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqldcffj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ugyrquzm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aafkhkyj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dphqkvag.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ecbjyzef.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqfudkfy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ihkcfiih.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ynafylkz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ubcuxagf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3pafblpit.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wvfbstzo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3boulcyhe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3dtmmtnrc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zmxowimw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hpkqophd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zewpkqke.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3oifykdnh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bekgawym.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wvsxcwxd.html


<!-- 参考信息 -->