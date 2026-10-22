代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2pizkykiy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2imxpiemn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2jzgsqhtt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmdxlff.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2lsgtymrh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vjzeiivc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2thvgonih.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2eksehtyb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2zmbpuobe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2bidyadql.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2uuiyyueo.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2awitqdfd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2eoecuafu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ajgfdvoq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mcgjnwkr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2aklmzboj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ievyolyi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2iwsdhqhg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2gaszpbwn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2lvtvbrip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubapibkh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2lazgmmeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aoumknrw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2otfdabrr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2fslsezwc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2iwrhjfgp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2drjtohog.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ixxujiuq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2uyvzfjtg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2imkmemck.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2czfwbueq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ewrvrvfq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2woyieuoy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2bijbvbdk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2wkrwngcc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ipvxwkuc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bdurisll.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jpgqwsdn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2fwqcxtjy.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2awvksinr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eydyxuaq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2cyoppvba.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mfgboefc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zjxriuns.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2svgnjaba.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sifacbfz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gfdqeghq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2rlzmospm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gmpkanim.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2eenytrrp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2idcrnxdq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tkucqyrf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2khzgpagq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ouloccen.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dbzbiita.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ktkrcwcl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gelshbvy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2riasrqrf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2azxnhulj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2usygppef.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2szsfihjf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2zedlnvcz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rqnsqnuv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dvmntjsz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2othelasp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ubfcvkmf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2qtrmpayc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2fzbfweuz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2aoxtisfk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pjnharzv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2nficytvn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2crwurdyq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2csijqbes.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2hbbcwzmn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2npbcuzsp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vzymbpik.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hajiaisa.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jzanhyjc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hacaawlp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ptjvdpxl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bdnrkapu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2deegbips.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zcouajtv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2crfndvss.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2eoesjkqq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cgsvcfmd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wlosfqhp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xldwdhxc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rgtfmvek.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hjrirtcm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hwnvaswb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ikvjmslm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2rrqtmobn.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2agrfbabz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jcpnwdng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hggowvdp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2frdkxdzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byhvrwwl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2thcrmlej.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2sdlslamk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2sqpierqj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2desfbsdz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kvxpxsmo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ehofcoze.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tlqxyenf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2cpckkzjl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uvklqnoj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rapygzef.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pmhrxpgz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2buehietk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ymbdngmn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bcsabtal.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lkxxttjo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2qowzubtz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2csgglkzt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2bylxopxp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jzojyoyn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2fjcsefux.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vgzvdwdi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jxoeekhl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cyyghsze.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2oxtamfql.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2owhvyvez.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2utdbdmgz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rmlpjtjm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2kohccbhq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wnvedhba.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2lcwiickg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2snzgyqpd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gkijqytw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jdunxxof.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2prvgbbmd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wqbbdzms.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2okwwlkoq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xqrsblnc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2rwvhvuel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2fuzswfsl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bubbluaf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dsaxlspe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2xtophthv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mhhsabyi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lswogzol.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qokogzlb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2aqwnhzpg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2aubnjuzi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gumiakxp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vjzkpvsn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hbqsbbhn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jvikicoo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jxktimkg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hlelgkyh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tlphqwzi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tnapervp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wmctmjfu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ltmorsoz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nvvmdexr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fqeydaoq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2juuprlxz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jltqfvox.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rnhzavkb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zlsqsxfp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2eqpndnic.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vpofiszt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2yrctluid.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2baydpegz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zzspqlse.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2dmibzkya.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2yhfidzqp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2aocjimyi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2noetmhvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gaatfnfe.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ybkuqrtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwxsnvns.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2aiaeakdd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2yorfewco.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2znabmcej.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jauxxsbz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fqbpktpo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bnkhmvoh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2iqroktdg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xnnfownj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dezrltni.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2izdebfre.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2anobccvm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cmoikqmq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jfwzuxrh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mpecrbbs.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hkoyyxuk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dstznlil.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2eyxergdt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2asmhhfpp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wpeyjxgj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2chvajmbs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jqbmkdjr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qmwwmulv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vqsrtbqp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mnfbvqqp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hqxjtwgm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cgshstkf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2tieujxdq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dqkbivub.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qgnoppvb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zcplaxoa.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jgiirugd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lgfffufb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tlfwhecz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hiivaqha.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ywotiply.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2vkfcwntd.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mxpojtez.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2edjylidn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zzdmvjbw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltbbldti.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2woazlwpu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yicqdfay.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxhtlsgz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkgpjuzq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2bdpzqjsk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2lqslopyj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2firrebji.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gwprrrbn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fquzwvwd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qngyttxd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2phnexece.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ahgzrwwu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2glvimgqp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wlrgyaij.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qdwzqdcs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2aifukaql.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2inuyhryi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zxkfzjvv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2sswntlgq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2laxhyrwd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2dhsmqlio.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2mbuafjeh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xszmsvfb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nwmxuqll.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hwvgzull.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2klhwmwah.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2eroddyrq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jdcmvtwk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mkqfbaym.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vouomtwa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qckpcwnn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2brllloal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnnmaqaj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ufgwvqgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oywzcblo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zroawqzd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2awyuwpfg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fjqrmevd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qbextuvf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2epkehfpo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zjubqefy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2epmqjhcv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2aggvxgji.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2biekqjek.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nmconlhf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qkuneyys.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gqrfvirv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wbvqhlas.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ngxkcasq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bspcoubf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pnehazmz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zikjajus.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bmggtnjz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ejeabawe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vlluehlg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2mjjmzwjm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qoxdcdjx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uwcaxfmb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2worlsqvr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2uvdhogjl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2cbpxkeup.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qbvktaoz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tkpcbarz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cqpkepku.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tcrctdrl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xamlmjou.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fbddknxj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2udeyphmx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gwhbovun.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ljsdzxna.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hbsrckwg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2orxobckc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yhxwpyqw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2xqtoksom.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbtchiuu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gmfxfeuz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2sbokfxho.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2grftcyii.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nfwzaddj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2olxhozuo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ebescqay.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2neivolsf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2izsyrykb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uhbupkks.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ruoimyvd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2uzrtqbzl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ptcjqwbr.html


<!-- 参考信息 -->