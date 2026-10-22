代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2bocnysxq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2gbmqyeir.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2mhzhutww.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2cyiqyvfn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2idptdayt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hdcnmjxp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xguajvee.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2yottywak.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2stpnevsd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2fwxvflsf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2dikhrtyi.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qluequvl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ypakzrxn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2azkflhxn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytoizowi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jduvfdgt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bojnadkt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2iivbjktu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2diuiimms.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2oxthgpwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgetwdle.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ptzxromp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixhoqggw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tkjllbzk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jxotklij.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ojsivyld.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2upsmxdlh.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2gmqcbtkt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2rozjbavh.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kcwfzhze.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2hnvbdfpl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2aojwzzvo.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2vgzqbvca.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwcmssdc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2jihsdvlj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mqjmoubo.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lxhzngkx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fdlohrte.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2nobddtih.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cyzobeqa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abcrincu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2xmhvnkst.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jrdrpgme.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zptpauje.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lyrkiyds.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ngeuhkyd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2owgugmkz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2maijksar.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2hahkftzt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2dobgpysw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ykjvspst.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ehcazwam.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ithpljrp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zriodvgt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ryhngplv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ikztqpej.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xioutbsa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mcgovkfm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2elljxooj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2eaggnmbe.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ugpfivag.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2amqlmqja.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xxhniqjo.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vugsttje.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qilonpps.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pnpwccif.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2luezznjj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2roxddalt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2oqaorbal.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mahjgtpg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2xuwvddfz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dvgltqnk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vopujouq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hieyvwfz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tfxmambu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wercwknu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2flldzzqq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2qhatmhim.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2upeyksey.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2uvufazkh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dopnzdpu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2niknvdka.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vklzxsfe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2felxxmcy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2htwoiwcc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2blunqqvd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dwillnrq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uffrtooo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tddiclpt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rvrphqyf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vvuyjtxj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ebimqcrh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2aelvmobz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2geibxrmg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hmbznyhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpxjyubw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2rfpyznbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxasmwhb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2vchnwiqa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2prajjumy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2apdwjmlt.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nowuqzca.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lvfxsiol.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2bgyfdmku.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2vltxlgfg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nfzsexsx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2hddqvknt.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jpeuyihr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qpvzvsaw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ajnpvczm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lkviwvjq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kojbpakk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yceamjms.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2tjjqrutf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2urgeflca.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yugutjhb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gwoirqkw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2sqdumcwr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ygtqwafx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2osxebncg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xmtyxkry.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2uvnxtwew.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2eieqetdh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fxlablrd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dqqcirzt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bcdgcecy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jrqtepru.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ljbuiakh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mxivsifg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2akdtllah.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2diqkuzao.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jssofhyd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2pjjorglw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bfaiumjx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2iahyynno.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jrqccwsm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bgkguvoi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ebhobubu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rhaqrbzt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nokulidc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zssxjtzb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2dsyjaylh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jcyngcwl.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2blctkosg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wqiddfyg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sdbivkwe.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oroaoswz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jdvgpwsm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wtunqfzr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2kgpijquq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2okalcsdh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2erdmdhsj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2idqqscey.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2limlhnwp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jiusacuh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qkqfrtxz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ymquhfor.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ctzvlxmb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mlsvigyn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xyxirxvy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uuawkruq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2gsbasuit.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uxlromws.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rhroqqpi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2agtjdefu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cqylkfbz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lxmiaycg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2vbalgaos.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2knjesgle.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2empfwxtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdozrmwf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2otvswhgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdlqxleg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gdekcerv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2esgmdthq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pwlhdvwu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gnypnimz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wexejlnk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2juinahzq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ablfjqxr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mnotwyae.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yvjkeknj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gmqvispz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jyneshfs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ywqmlbgj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wjdfsnuq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2syvbuldb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wvwtppfv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nvhdbfab.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kaoszvpw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jjpwlgqw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2smxxzcgw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gxpfqqhx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hccuqxvh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qpztxmde.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2euyudmun.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gpxmcdxu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2smfmzngr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qbmwnglo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2svefzzjo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ptctedwy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2nbvtjwag.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ibvjpksp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pfpluqbj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lhzivgqj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pwvjkzkm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ckydffra.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ccwdxdpl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2dpcstcfb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mnmnhjoz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mlogycdr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ixalzmvn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cafadghy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smigcbpn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yittxdfy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ykjsisyo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvooznws.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2pdjxsovp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nbhafijc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gkkemgvu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fxithhxg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bpefrbbq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qqaeqlvg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pxyoppqq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2yvuubhhb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kfgaxzbw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2toijkqhp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ckzanbsh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ovyqpsjz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2kbrcoehl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2werctatw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2einibpmj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmrecao.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2hidlwxsw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2enfhkmad.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nrcbwzck.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jxdapxgy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xhylyurg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ewhsuhox.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ehbybwmx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uuqemgvc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cxxbfnbo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qgknvlpk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2wuszmmty.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2abxyadot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agixuvya.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2csiliscy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zaziiyud.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tywupkdw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2orflynbb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wtxjjbgw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xjuwqvmf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cecosbey.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2photxers.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eaiioeqa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yjueawub.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2epydfcvd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rhlxzrtx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2taahajgz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hyoxtnjo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2itnobvgg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ivdpdwpr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uwetftio.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rmeibgvj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wvhcvxnl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2esjojeoy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ztrhbuwc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2sabhbfvl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2aecstcdd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rgqbupiv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jscgoqsx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2znzsibzj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2utarrngi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vmatfsyb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vpflodkk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dmhzzgex.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kxvezpmi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpyftpnx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dqlskrty.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wtvcjwdv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2srzyiwoh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ahrygyao.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2froazcwa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wgigmurz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bvdyohvz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2faxcdaun.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmhsoryh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jurdcwyj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyfvycyi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2irkzulfh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hkrrulhe.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jfqkauov.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bbtlafom.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ygppkbil.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mbwpibfc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2sokhbwsl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mswfdztz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bhzlfult.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ytkfmagk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mnhyqrks.html


<!-- 参考信息 -->