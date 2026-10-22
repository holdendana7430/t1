代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2prmkwufx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2mtdsrhhq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2udtdbdbt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ttwilxyu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2vxinmmto.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2wpvioeih.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2yroqincl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2fezvpfpk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2kmombjla.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tcmmvuct.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2bhwqnqrq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2fpeezbew.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2knjhqsos.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2xqkmznwt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2mzjcmffw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2lerqnuce.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2zjhqbvli.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2rvfvhbkm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2edrknnoe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aedaqehf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2trtsnkvz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2rouwckck.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2jlxktiya.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2bkyofrgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqxgzgti.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2mamlgtyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwexeqyc.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2smjtjplt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cywzmbam.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qvxvmukf.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dyboomuo.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2mztjjvae.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2gdqxcnqv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2avnucxwk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2gvashvax.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2sjxouslx.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ewcogzvq.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yykaagvg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2sxpmajcn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cmsrwdwp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mezylgsy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rtxjmeaz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ntrthntm.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjfbvgwt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2oqdstsqy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2jczzpngx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gnedjlcc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qjafrmsn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2rxzzsoyz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tiekicyo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jggwnqer.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2zoqxufqt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fryvfjby.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2teqrewcc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhsgztvj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2gazcixpq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2fcawzcvu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2toxsbpmw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nmaziycv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2edwdxoaf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2oxecehbz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pnwpcjpe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2okxhnxyq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2xbbvkbtr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qzvuldha.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2zmvaevgj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ivswikho.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tmugbyjz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2wymfdlzz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2kzarlxio.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wmmzoptn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2yhfyaovx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2yyzphrtv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2raywuypn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2xpzcrmqn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yqsfbqvm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2grcjpllp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2skgvbfsa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fneijevi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cdnnjhvp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mgujmnvi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2tcceagpt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uvcrbtrx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2krecucdu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xdemmcix.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nqeraxvp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pdgkpefh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2cjmhupow.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qwhxbhaz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xfkimiht.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2yfxaaggw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oxkankdi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gfoqsplh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lfpmjeor.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uxxshvse.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2efeihoqi.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2faizamjf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2tsjfiymj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2aolqdmam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umshainu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2vpftmnrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsknegbi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hijokdmu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ctfafwsk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2cavhsroh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zaaicvuf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2izdqdtzt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2nihshqnb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tzgehsus.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2rbfpopbg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wvinpdum.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sbixiryn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ovhctsew.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jmtzihxf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2odnmjqko.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2uofkjbuh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tbosmecf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ypkogrko.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2dzzwptmw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2badnaaqb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2thwejmya.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2fozsvnzh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sipgklow.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dunpggam.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ftwagzzm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2bxfwdcrv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bemtkqvb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2jbyqfndh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lnrqynun.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xggccmbm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jwkurlse.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2qdwgxxje.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2eglqaxox.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wxypjfgb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fbphtuff.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zlhmiytn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2dhwhdiwo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uuosewna.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2tlswadjz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nvkmxibc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2jbglbdxk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ofojqngh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yenotjin.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2bchqrnms.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uiumhyvw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ycykrwmt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rjvhaadk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2suxzlbpc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lqrexfua.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wuhxmdkf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2urijeram.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ouioeguy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jgrxrgzy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2mgdqzskl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2eoeabvhn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2trknunnq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dukezqqb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qqtsmyrx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zmbtlbxb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nreyvzsb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2omdluouw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ggndsbpm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xogiuppd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bpijkffu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2czdmxawm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tovcuiwd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2eyrgujrb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ikrqoecs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gnjasfec.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2maxgfncf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2whlsyiqq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2oqqbquvg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2grbjyhxt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dohvellw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikixjqnf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hbznrzqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdrknffv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kqmvcrqv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hsrmruxe.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2iempsftd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2watwaeqi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nbrgqbvo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ktqjthxp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vvdrfwxe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bphdhtih.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fipfybpi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xyqfegqo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tkvubrwf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cqfmkmkh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2orsvfhog.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tyidoagn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jzlnnfss.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xbvvcvyw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ottjlvac.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2weluuyvf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2djgtyobh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2fzpbxwcj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2uxrdultm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bpppgzir.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yqoedjov.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2egnbdgrq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2nkxqnszu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2lexgszjo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2epnxfkql.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vdbhgdjl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2hedcskkd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2csdashjv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rhjdfaun.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bhqhkyku.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2peqpfujg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zaneofqi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gdqycxyz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mvcklybb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vmixdazl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tzahiitc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2cshejqmf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fczzbmgn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhffkdvy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2arflfwqg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zkdgquna.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gbewwsrb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2uodqbmol.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pacvtuae.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mldveugw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dugpebwx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wxvepxsw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ptyptntg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2alclitff.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hsfblpfq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kmxugmmy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2btqoiwxp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kibktfzq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2yhdyrjgc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tzmgyuix.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kqzfczad.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nkmzzzxz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2tlmhfucs.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2cosdniyq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2etsmbdbr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2scwyjsra.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gidgvgbx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tpeyfplo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ogaptyki.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ofrihjgq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sobksqlo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2vuyxmjis.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nnxiujax.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ahsvchss.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ojfekrzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dreerfjn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kuqsugiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqgtejzb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dloqyxkd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2osscdywc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ticvbzzk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2inaybnlr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nbuhdgdp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2igctpour.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjjmbwso.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2knrjjcve.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xeetnbkz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2clkraiqk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2diligiac.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vyinefzb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tuztkhqr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2amaixlle.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vgpuxugd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qukwwmtg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xasgaxvi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ejcynsyc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2oviinimn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2leamueun.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zssyxhmn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ueiqeftz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jskfofcs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2nfanfwyo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xiqspetv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wmpisyuh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2baquuyrs.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2azafrhcx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ojyjggoi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tendrtgq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2svqjkthw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uljpzxki.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nttwvauq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ovthxmju.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jezrjcrb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2osihhzkk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fkozejcc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lpptyrqz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgamfcqp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mvyoueax.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfsedkzh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hdlnxjec.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2utziajrh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oeqjodrk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ulwjrbhv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ajqvnesb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jwwvkqoj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tluizbsn.html


<!-- 参考信息 -->