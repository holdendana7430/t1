代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3wwpfcwia.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ytwgsowk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3uckvrxck.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3xqdvmzon.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3xzubjqqv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3dzlsxrnr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3laehzpvk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3otobjudj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3tftdamys.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3llvbamrd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3plrywber.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3uttfalnr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqsjvobt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3dtmlyqrv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3xszznxms.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3luxowupv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ngsixulo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3brxadvhi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ywkonxje.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3rqjzecio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgfjeitm.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3xeiyqxhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuqdktwk.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mhkjvxmy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fwhdpgjo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3nigxibvn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3musgngwt.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ravzhfsk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3jzhjqvjn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gfcewrle.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3kqcwbvwb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dysecxxt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3losavlvm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rscllgnh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qldgxkaw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwjjvnlx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ltcewzdx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sfybzmtl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3yhylgquu.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xhngxxxc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qfxgoian.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3vfosjwdn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pcsbvpbv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3drdscfhe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wvlcqojg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3rocbaaso.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kqulxgqn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ioneqefh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3dbxjvjqx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3maxsrony.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtsljeee.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3tgcqkswt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3nvrnduak.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mvwoziud.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jfqumsir.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3muhezken.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3plesqjvq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rultdpjd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ahutaved.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3kpadhfze.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3edpcjjwf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3lcpnaqki.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yjydivco.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3danawmsw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ksnosicd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3vnyehhrm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3uqxbmrpq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3xcwcxckx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3omzbrsnb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3malwwqqt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mdctiaqu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lxfhrpuj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qbdpburx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ctykxlbl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qhzdezli.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fwosvhxo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3icephyii.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wevsgygu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nqasxjic.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gbwqwxqc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3itapxzur.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rfvzldso.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lgfttrqy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3mptzyzsm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wfqbumlv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xmnqpofg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3twvllnyr.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mrnvpnrj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvgtnmod.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qgdgnkoj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hrkmjibi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3qukcinpt.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3zxmbfcnr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gxnooemz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3itbuirfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsrftecc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kklayuna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrwqxpcu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3pehvqylw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3smyynpvd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3cvymyybo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mhsjdnpn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bhlcjyib.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ekydehgf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rdrpqrii.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3prvnbxpg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pakozjfn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3emckvmkh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vwzbtjlr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3qnjjydvt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ephzzcbt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vobkgmfk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3wdyawwvl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3tyeihzyj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ptoqzdds.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3oavlpkcy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3vokgonur.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3sevqwbfl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aqjcychu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yzludjkl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oelqnoib.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3dwyehpau.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ebpxmopg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3vezzidid.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mksfujcc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3uyxprbsm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jztmvkzc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3czpqvizo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gqytxkdr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uetycrlx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3trxgwehn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3nzeirqmj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ybnisdth.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dlwhlzby.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3cztkungr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ufmitkch.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hgnjfnaa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qffberxh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vujomdgi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ukhfsxao.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ufinryqt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3gjsnlfyw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rwnhmxkx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tzasqkgh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mnhyygps.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hixizsfj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sbcxechb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ajcmpapr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dqhawsgc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mnlrrvrb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zxkbkiur.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wvjvbpvr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3blbqksys.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3dlrcwdsk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zdzkxmor.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xqyncqno.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rnkviggh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tuzexcqk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rnoqbrvk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vnithevl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mybylsbh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dcpdjjfc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3engnyhtp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fydxrqij.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sdzjrwra.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oatmjega.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nfglwtiv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3uabtptpp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hsecmxmz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3uwbcmppv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnnmytnd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fohuigrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pohkquuh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cihfsmht.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3kykqqxeb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qdsvlbkf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cbribfrd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3toxatoek.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3omkvofrg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3baoxjcri.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3hjhljbwd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3axeavoxb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mmgkegxf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sevrpqyc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sxwidbot.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ddnylznw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nefaxkqt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jygjvsda.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wkjtkzkb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ktzazeda.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mdrcfsgn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qxzngerl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cfihmzbg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3sapfkoqe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3anneghui.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zlahjthw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3deuqledo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jcfnqsjx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xgvwfzco.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3whcsroue.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3lyclzqpt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ilrgeemp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3rxkzauhj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3opefmlti.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3sqbucoje.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3shcmblpv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dunrwrnf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3etwlyvxe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cmuojqjt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rtxkohxg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uscoxoac.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nxdadaso.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fcvpzndl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmgtfumm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjmorfcf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yqiflyoy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wkljojcs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3suoodicx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3peeituvt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3oyelemrt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yowhfonu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3krqdfadz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hicdiqwz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mffirkbo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pcjcdknu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hscswoog.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ffargqlf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3brshrbku.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fzjjijxy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wcitdxhm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3khzyzsvo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ilsexldq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3hnkqtpdm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zrlybxxz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cqeicwdp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yirhbapa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3lzsbrhuf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3quegftxf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gjuxzffp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dfyrouhp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3sozmiwin.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3hzrjgwsh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ulpbnwfh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bacefdbq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rbwthbav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwmwfcnu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3pmwemezz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcfyemno.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3sxipyefc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nunluygs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mrwipcan.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ragjmnbe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wtqbreiw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jmbrsimu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cojvwihl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3knoawtli.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3corxelgh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3alogdbkj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cimmmnyu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qsntiswf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wzgrntbf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nloqcwui.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ykdyclwe.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulgtcvtk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hshnnvjd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3uhesafrc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ydfzgvfa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3fhxkxspg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vmckdfzg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bdtrfzno.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gpjjdrwz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3msirkvvt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3huvelmzt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3tmicqkar.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vzavtedd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xzormozc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gyjrcsxr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tyemovme.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ecazrkjd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mmnmszin.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3waexdcnc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3iawvlagg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xvmxjhqv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jywpaknu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3jgfjmsml.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vevrlrid.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xripsnvm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbtxbczr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3axbddiui.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ddlrlzcj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3rkmhryzc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tpdwttve.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hthtqstx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3bxhftqyf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zhluohys.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bhajlwcc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3muqkbrmk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tczrthvd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3estxascr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hvtpfdul.html


<!-- 参考信息 -->