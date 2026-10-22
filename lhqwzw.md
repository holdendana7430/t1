代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ebbvwikz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2qezubkhe.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2msbqczsp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2jwuhurxj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2dauodznz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tnetegnd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2rcssdyvh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2eelrmpic.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2iokmjbof.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2rkvikeir.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2usunrzzd.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2debhfqmo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxvalpzn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2giecflsj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2irhyvtjl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2oktomvve.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2lunqdjsu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2qofgdhcn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vlaugvmm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zwxpmpsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfnqrozi.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2sofmgtfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jccaubuc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xhghggxg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jisxqpnb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cjmfylld.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kzbiunwc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2koxplpoq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2sdtiumkg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2dcgkuaos.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2leqyvycv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jpxoukde.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2oschzhsa.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2eyjdgwtc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2dbdgtcsm.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ctkmdjew.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hpeindpd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sowlaqfc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwicddc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lcchcjvv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ropdkplo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ydjgfvrh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2hpxkrgna.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tjcznrql.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kdawexxu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vheimujw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ewntkfil.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2cmnveosk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2fytyejrf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2aemfeust.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2naizzveq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2igwioqbf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2djjiclrx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gnxaqgzp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kcxlhbpn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rifchytq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2zwqqfoip.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hkeglmrs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ocprusfk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mkxlrbdd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2laypauya.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2cgyiatnp.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdzzxtym.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zkufkhiq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2gmwgkmvj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2bmjlarlv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hpafnril.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2mcbzhfkz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2smqskxsu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jdswrdxs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ribmebhy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cegqamly.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hfkumqet.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dmabktoz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zybdqkcg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zafxtqad.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mjvpbmmu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yggxxhml.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vssfvcyg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2zgaspcdk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wcvswxuw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oupiupic.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kkjwekal.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2frfbhdib.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wcjudfby.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sfqfkwgj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2bcmkasnz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2limabsgl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2fwzemhwc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vdyxrmkz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xiwvzapd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2agiiucss.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2gupbpcuq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ltnvtkqb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hrxmshrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uivtiqnl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2fmwrlksl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvilgeua.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zaoixjgg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xuyqzoco.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2cpypgiuj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2gspiwebn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lzcfrome.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2qgaotsjn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2spkqyimu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2poomgrxm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2tdrhlqvz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fkwoylfa.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2cihoffld.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2suzzghwc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pxjrbxtd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jhiuwdhb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2uwkfoklp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2kufbvrus.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2aarwxzpx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2igmolvlr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2hujpevhy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qtoudnku.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2emfwovqg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2unsgpwsx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nhdhuoln.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2gvrpqxma.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nvixllkf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2apbsvphr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2iinofpeq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2uqgdmcnp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2eutfjheo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ofofzzwq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lbcqaxps.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lbtxfphf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nrwejdza.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ndkxpbtn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wslheman.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2lktgvvds.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2cjhmqxgk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nbqzisfy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wzwepmmv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mfqsfudn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2chtizxfe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rppkfosw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zwwhhmqc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qwvqfqqi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tkfvimtw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2uiwydkkz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2osjundam.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vricmebp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oxdlxtte.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rtirwdtw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yucrsdac.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ltimaklj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2insvxmey.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2dlnmbpnb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rzlgxrxz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2sjpmhgcn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2cblusopg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wjgbsjse.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mstmchfc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2qmyiamjy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2otztfuwx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2epsaklph.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2sfeyjynr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wsjivfxw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wleschgf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qivfosyi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2opefknjb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kguhprhi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2feakdrdn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lwgynwef.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sxahjali.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2thxaestx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htwhwcza.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2lhnegpgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htqzsmnt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2beizfhoz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ccvcmlrz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2soqxyhhj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqwhfnpr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tqgojbga.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2npabsvfd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lsoombys.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xmvdqddt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nofjjbqu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2avdtflmr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fdupyuzc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rhosrsnb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2chevpkqz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bnuvvsbg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xabttnom.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wimspldf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lmagvncq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nbprsmou.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dzqqlksk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ypxjedkb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2nzfmbgof.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2imjfnzaz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2giatbbiq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2cbqxyuze.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xlstgmlz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jetufvie.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mozxaout.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jcfowkph.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bsnwxlvl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nlhpsntf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vfshvxha.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nsdczzwj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2vppzkehp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rnvabbei.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2lcffisyq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2fapdmduu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2glbhuums.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dquevejg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nbatpiff.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eefsuake.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wfyifkrx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pjeragtk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jmktrvml.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rbdoazjh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2yormbpit.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bccnpwez.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rwlhuava.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2krrqojoe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2onamalld.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jatefgfp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eyfhhtjw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2tmglztdr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qynxubca.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2hzndezsa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2stzgwluo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2siilzztz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2iewvvflp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hqvkwhxg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2iaiabsfv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ofvhkksy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ffobvwgh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2cztdquos.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ezaxgqdq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2anjtyxki.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2fbocfblq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nfknwmja.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eeyesxtt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dftwqsbd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2lbllxlqk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2sywxhmwo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qemkxczl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jupcphbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2daquaxcb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2grnotzha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vltpupyv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eoyfujkh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozulwqks.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gkshydfn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lozsjxuk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kufrmvhe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xiqrirtj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yldjqkwa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hkwdimxv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2retfzmhj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lpgtwqun.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lomerece.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ngiyzras.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bplwsbpq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bvcekbsr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hgusnyvn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bklkebhe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gdrgqrmv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wncalsds.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2eteaamtg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ibfbrixg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vggskneg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2agrzfbsl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gknrrwfp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ytqylkam.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jmjtmwog.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fmxocxzx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qlutygqk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2fyykfwps.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uciwaxhu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtkmzwby.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bolkgilb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zjebhjnv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zajiewiy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ryyandcp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pqykijcp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gyjjcubc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2oksonifs.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ajxxehkt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieobttbi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2skldhbpx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2geykmbwc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lqdchppf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dfezdggh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zlpyobdj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2okdzezuv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mydohtfo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kjfjfjbp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kkrfgvnn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hsbfwvou.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ztaiydaq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2trzvgrzr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rkyyjrnx.html


<!-- 参考信息 -->