代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3wijmqlnu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3zeyhedto.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3eojmtlma.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3codxgoeh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3yoxzxtvz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ntfxlpqo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3mssaxict.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3zwmproux.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ysoeshco.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ukbgfvva.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3oceekkum.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3srdoaoya.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3fyuljtff.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3grhqvsnw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3apefunon.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ttjpyivx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3hoctwqhz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3meaxvnjs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3knmzqthn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hiwhetjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xubxiehh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3nznsgfvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfebfoig.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3dunosvlr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bifokjaq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gdlrfstu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yjmopsfb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3okksuqub.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3fxvxtkxd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3yccvtjli.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3eelnzakk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xsyszpoo.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3mwyzxcgb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3usotmexs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3uxqfbbwe.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ecmyvxrw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xqfdwepy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3njuktfam.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kvtxhtmf.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mlzsynll.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmqbfppy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3celbqzxv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qfqxwyss.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3nqfnfbed.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdkgbcnj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vszfeuqh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3dawpulic.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ujxfgeal.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3jdueyikg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ekqyutmo.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgsjjszq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3dapgmoki.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3kovuidox.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mrxbsazr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cmuoyrfi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nehhumvi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3eaqellox.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cwqgxfqm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vrkrgbrz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3yfwxcmzt.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3jyrahdbc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3idxufwmc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jrqrscwr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cjfhlgtd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3phpglqrg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3qzayulyf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lhryungd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3jlahtqbj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3maasefbt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3byqilveu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3lmhqyyje.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3sopqarqx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3vakzgamc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3dhllvpyt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3plzrnide.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kgzjjksw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nhpumrqa.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3rpmvlwhz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3eontykjx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3sutqgiga.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ihecyhtv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gtltfgtr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ibrnfapw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3fvwijlez.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xvfhtfta.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3doelykml.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3trgdkgcx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3omqpcckp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qgmybvyi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3leqvypak.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3grgcparg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3curnwibr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fqurvdqn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jjmvxwiv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yzmiguje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqmfhykw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3qidwegca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibfkhxsq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ribxcrgy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ihffqyja.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3yuhhkqlj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yrotzufb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rdlnjbqy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3tkpxuptc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lzsdlwoi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3xjkfcxhb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ltpywibs.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tsnoxasp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cqiyxbeh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vmulwumq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3afzbrzat.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qawxwlmr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jaztgdtv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3lvfdkjkf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3kdmbqabz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3czgvcjds.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3wqnptxwj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3bgsxtczb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mmizmman.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rcchznbh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dpkgfwbt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3brflhnzg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qnopmguj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hektesvh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3agicbgfy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vflozeuv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3cgryxgzp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nstvxjzl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wedknzve.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3utmuvwyc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nufizibk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tvavpcpe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3gnsuqkdi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3lhuggeqe.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zuzreubf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3kvtmiqni.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3cgovvvyc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3emgstiwk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pttsikru.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3aswzryov.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ukmuxkzc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3aecfjvgp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yslqaxun.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qidlanuy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dmalnqgv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qqrhnyxx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hnpuynsz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kcgnfvkc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rqalswyb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3idskzyhc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zswyolsp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dacsfoui.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zhedxwlf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3rxsaxsjq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3byavkigz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jrtubjwt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fuwtbaap.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xygxqsmk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bhdsjzcj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3smxuokph.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3yicumogs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dmbzpfkt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jbtedlvt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3aprekgoa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zxeinzsy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ipebqkjd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3uionhddp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3jlgrmnhq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dchqpsmn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3kitgqisi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbtdffio.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ouytqmci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3coletjri.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xwyhhkbf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uemgwwxi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3amdwjpjy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzkbrasf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfaivtjh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ulybckie.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wanfqohw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pqzrqkka.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ydnhntrc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uuotvfqb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ddcsitwj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vsvnyqlv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wawchivq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gvqscbja.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sfuopwyi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sxvqrmmy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gaxwjtai.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cgajrgld.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3yjfssrmx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ppltamym.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3iidkteyj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fngmrrkt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fgohzvsx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jloweizr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zpsnqoal.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cqciizyz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3codiuqvu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3onrnrrij.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kfuheaiq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zhxgvnul.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ulgzlyln.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vzcyjogn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zxarjyiq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3oxmumorg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mbekjleq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qhgtwoen.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nxozwwvb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpoouibd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rzveqxbs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbvztvtd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyssmahh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzmchzly.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibumnlql.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yduvpwwi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ioofvbkl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tnbxatyq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fslcqfuy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hppvitcd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pzmjfejc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qhsdxber.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rkggbkrc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ccijgkly.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tfzughhn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rjysbjll.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3evozgzve.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3cutebqhr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gxzpcpsp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gmvmqtgl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tfqukeon.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fmjxomig.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ymtiyhbl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3hllrpycj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3xlcompet.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mqyxnlgs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3htualkoh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pcdygnsd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xcclyqiw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bofvsyac.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3fprirzgs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3javjkyyp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vdzezzsx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ygyjsndf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hritkecm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rsqkduue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyegjetv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bwtiuvjg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vnqaaosj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yysigrzu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jctszusa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3djiszxbk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ddstezwo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xbwsezad.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3atzazstr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gobjuqts.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kwhvjzst.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tmeyztct.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3skjdidlx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fylbjxar.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ldngnhle.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rlmvmtor.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tfoqcmqx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kdlrviiw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zkbttssg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3hkztblyr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ddnatwgg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xkwwxypp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rykqowry.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vpsubjsy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3usvpuevj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3atdsvnwo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bqhhxlwk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kxdreetg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3svepuhcd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqtpuwqm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnnfmlwk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nwovxzvx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3awretgqn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jlppqddc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wopouksk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3haxvmoeo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cexeyyde.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ibvckoym.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tazuakky.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3dikjejon.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3szpyasft.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkeyktnc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xqphjimw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3lqpzokqe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qhcppxub.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3mdrzjqfz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hyiijvis.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tuzirddl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qrirphug.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pydjvbqh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sflfmfxv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ybgfklvg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3jupowrfz.html


<!-- 参考信息 -->