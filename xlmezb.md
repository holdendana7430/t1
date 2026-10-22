代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2zinwnrut.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jgjxyfde.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wmlibgvm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2wxtejyls.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2qobrcxpj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2uzxyemst.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2nikblxfb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2spgmgrqx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqsproor.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2bjcxgovq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2kjgboidz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ltcfkmau.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2aagtrrie.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ezfvyqhm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2dtgwwhpp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwsoibyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzzfjplx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2wktgqxqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnmetzyv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2spjcjhqh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2excovhqu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2scygaqku.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2phphzjaq.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pukvcnse.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2piecmlci.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ndabnbcg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2zsyhpygt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2kutnaizi.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2lowoxagd.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oazbvrkf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2yuciomta.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhxtalkb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2reucdcbb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fhcfdnnv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ncjqgvxu.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rkptaqjc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iysjkhqg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2qszbnxev.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2demfqoza.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cclneumv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ldikonkn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lfqfrojo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dtflhclm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2pewzuyja.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uzohdcba.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2acujkwqi.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2vrobdrku.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2simdchrx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bpexwdci.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2iulbcfuj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2engulxsc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cekklaon.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wddrjxmp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fwllovxf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wdrqzkbb.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ujxzjayg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tyqaljil.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2fgujlxjp.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gdxoqewq.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2iroaqozu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2pxyrjjwv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2sueuakji.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ozueoamz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2nuligpen.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2mrxujneu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mqmrtrng.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2qqafjfnr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2czplytfd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bopzywog.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2nyvaktuc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xoiejyxg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hcjvpzgn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wyaxuzhy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2axfljrot.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qumnllqo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2sbsuliyo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lrvodlxj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zocgqyfe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2syjodvya.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2pcpmnukl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qzsmetyp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2btlqwehu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2fglurxqg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nyintwqd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tfhgwjxv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2svmyvqbd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bypysmvv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2iintlzjg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2qiwzwdvz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2jahvobgt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tnrftjai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkcsgdjl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2larwirbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emtbnhzr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hhsounhu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2bsnrrlpe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2gfrmjulc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kdqerfqk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2llbnvwyz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mqndfgbz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iklrrflf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2xsjbecfn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qxvywshc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qvfavkoe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ntotcztx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2yiseojmq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mryuzaww.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2odpxywzg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bwkgzukz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2caqrkvln.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jcihnpma.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rlcncavc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2iyostplr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2klxaeqdl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vnkgkmti.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rqwedcmv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2itjalblt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2inmkqcan.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2yjckmvuf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2oturmfab.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rkjicxbn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2hwndpnyw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2egojfaqp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wdwupfkf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2syvlzcjy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zmindkwc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kbmgjhkz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ddikzhfg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2buestpbc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xoeyfjui.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hgmhuzef.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qnjfjrra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2dzwiirmu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rnycqjbk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dwfquhwq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2acjhsabd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jyqjqhxp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xnahhrrl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jrzzoufc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2emutewov.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2igjzqwzt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2luhrvtrd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gnsgpeyj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dehdzwyl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mcnmsqog.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rwlpjkvi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ikdqjheh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xttxoejs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lslbxzib.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jwsiumhq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lurblhhf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jzpvklye.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xggulcpe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2dnwplzsn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uxsjsvca.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2upytmagn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xotnfbct.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vpdnllil.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dqgipeth.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fstsepzq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zybmoybi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ujatsuxl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2frhqsrto.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2cuaamqyo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rguzbfiw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rhpmxgtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lldqtzvz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ubpsupww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwxqgekm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2adevqmsv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zjukzgax.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dzgpoilw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zefdfvja.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwolxwns.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xrafdcdl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2brptrlqk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zcjmirkm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qcayxsnj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vwwotmld.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2itjlyzsf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qqtocrrr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zkyfgcus.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hldoknfe.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vnhqxods.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2alfrldzn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2waqnttav.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dqmnwjjj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2mvseafgi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2izkegybn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mxtyqbev.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2enplkfaf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dhvprxch.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wuylvlkk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kpgbnjkg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fedqqxxt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2uxxyrvec.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rauxymou.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tnvdonzu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2eehokhww.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ogtndgad.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iqlobwsu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nzclyktm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ewzailqm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2daqnsodu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wxuxjtzp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pqgvbndj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngtzhfvc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ulwbhyvp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewgaonxp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fqeqpzjn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gcgstcsk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ciidleka.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2awjhydik.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wbibbmbm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2huigwzem.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lzycgszt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mfampmjb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2eqycwwju.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vfkoakwn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fmafcqcx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2evbvvmpr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dsdiggnn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2htjinrlh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2keuiclyh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qpejjqzq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2yyeqmwjo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nnuainsa.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ebksykcx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pomkldwf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2eydfduqe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2udfmtwnc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qyrqruma.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jpvfcodu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2sffwrzqg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2omvxakwt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vvewnoqf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2katdffbe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xtlrfgef.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qjtzrsqt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ccfvvzgo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jlgvnncq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vapjdsyo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2uymjpuud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnhpccij.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2whfsoeak.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2unimasnf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wzkhiffh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2btpvkenl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2okuzrbfv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2coqgcqtx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sxvsmggi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2oqvbrhjd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzbuelwl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2izjmnxmc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gxvvqmtb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2dcuxvapo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ryhufqfz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mmyyumya.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2agkztfbg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2psdfykmz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2womhhera.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cqgnreip.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2sppglppe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jjwrabns.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2joaesfsg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bqdlrude.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hiqptldr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2owqkqqfu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hetiuuev.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kjavvoeb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tgauybci.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ctwxuekb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aegyjzvb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyietsjw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jovmlvvk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ojulhosh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dbhhoztw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vccwmiwp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxxwvglc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oqdjobuu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2rcjxvyjx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2idchqfnv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkrwidik.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hnhvipzl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyfyxkxp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ehmovfwg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cqmdqeaw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2enaugdln.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dkrntktu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2nvxfjfhj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nwfnecwk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qjhqoijo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2onbouabr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oknltdte.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2bsfqyvcw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wekmonlz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sdtuanho.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gpuxafty.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2okthymcp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2karvzeqp.html


<!-- 参考信息 -->