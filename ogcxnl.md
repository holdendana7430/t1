代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3djdlogbw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yrjqyxay.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tjvjzjdj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3mdmjuojm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3kgniypki.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bsceklgd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3eaposcer.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3spioewko.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3evsjvsvr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3vsyvxamj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3eosjykhk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qkzhuwsc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rscprhyg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3duvaahpy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3nhzbwjtb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pedfinsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtykvplw.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3bxkjmvzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3griejklc.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3rhszaiqd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mtxzwcxl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3udmmgyky.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3atbfxjcn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vndmallc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3rvkxcfwu.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3segprpll.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ahizxqdc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ctcrdoap.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3gwvnbiip.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbgieyru.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3pyityiat.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3bikdvjyc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vwfikugf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nacmltil.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nxfnestg.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jeulbdps.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3buarwwqf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3yomxnlhw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3cvtyrzkt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hvkamuzd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ocwxudsp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzkngwps.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3zzyalmrt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3smwlnuqs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3jksblauz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3axgrjqqr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3odgrnsxf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hxwhjnkx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hprdmrlm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gvtsylcv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ojxkvjcw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xkdlbeev.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3utyvzmdh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uanzcpbi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nvwpczot.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3dcjuhgck.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3behugmoy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3mnuibtix.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yfyqlnps.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ymggyzju.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ykevnkmz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3twlolprj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3cvsghjxq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3dpbhrdbc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ojkjtrhj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bybrsqab.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3daakwmgl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ycqfuixx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pannyhmo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vqmojvfg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jkxowqqx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lepgllyb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hqdmyuey.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3izqdcjsi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3txlzvwbv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3orhwhsex.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vgrrqtqs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rymafdrj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nwabvbdq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3wbmluboc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3cbgjfarb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3orzjuijj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3zbrvejev.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3dcgljmsq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gucihzhb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ynptjrlx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vruokgdq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ryyeheax.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3xcujbbpr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3czidbgpd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qjkvhjox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3srwxrftz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xdolkdtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbjsvcrs.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3bawhiihp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vtzsrawt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3atleinuc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rpbrobsh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3oulemoms.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3djejzzqv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wqagofgn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3mumqtuve.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3egqzlpnu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kqjgxlze.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3oskkzmbc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3abpybkas.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3adtqcacp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pvmssqgf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gufxiknl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3fmnigeqp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3rnghxnpo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3brkqlnua.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3myfjgaoo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hbiuuflt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bkgkqlvd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pfseojrl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3asfvjlad.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ryjcacdg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gtmqymnm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3oxwoiout.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bqlfspjg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3sseywwdg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ilcvyjac.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3esqpqhmo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ewvnegvt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pyrfjvqu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ljefphbn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3apazrbyd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3bzcatvtl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jchnifjn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3uuuqcngt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ecbvocbi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3nysvxlny.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jfwkjzri.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bmajwwks.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wnpiakkp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3nokrwwrh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3mkdrelga.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tzmnfbui.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3moyifhfp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iqjtitxs.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3boxlhkxv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rbwxmpbe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lugmdhzp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lrfiyeux.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zrchdqwu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3tulifkzv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nzqzcmby.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vqotkazx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ekphyhrs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bkiepwuy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vzfbhbaw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wokevvyv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fswlaoue.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vdwmghut.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ydqinrvn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cglcvvjx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3gwdurbfn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kgbuglsr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3gguzvnnk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yfacgmys.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hgjxomhl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kjzzqerz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3uysqcdjm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwmovkq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xwvftita.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkiggnfz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zwalpzco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkquczsn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jpzsuvpp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dtyvqhpl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3cdnfryqe.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3boerysla.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddyeaphr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3glhcwcok.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3yveetwbz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3fgzztzlo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cbbcfgus.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wkfcaoit.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ukdlpsep.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pmtleecw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uekewomz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dittyeka.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3grrnowlp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rphwsuvr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wlxcoyqi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xjdeubyc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3uoizdpnd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zjqmzpsk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wdvabwsj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uoxgdssb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sfzloeox.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jiysouga.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3alrrfoij.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cknuwhwi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wpemzsde.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mxlxrcpm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3acnqoywa.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mnodszml.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xgvpplqy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qaxpfjml.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3knjtbfcj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vlsjyxai.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vhjfoupq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ogjqxrak.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3prxxfsgf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ynnitxhr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3mxosoyya.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wwblrcdn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vtumvuzi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nepkgemx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwfpjjvj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tychztzc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sjkczabi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3miqpxqjs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zowhvzqr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uwopzlcv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tmvgdvlf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gjyoyxlb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3fcjozlcc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ywohqdhm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gbmksbce.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vbxtsdnu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qzeraoch.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3uqzapgxi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xdugknjb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3aeztxsyo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gmvglths.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3guyqdfeq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3edyeqwgj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wlfclxvj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3tnorlxlg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gactqflp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rmvgwwii.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tuqpjadf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3imvthlsa.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kmrpqhtl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rqmpjjuz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qdvsnwwf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hqaudeqj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jhlazkkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghalrsab.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bcckrcox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glqsimdq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ooifjoge.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xlbecais.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wwxboodf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3awncxtoo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cnopdrhg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wbcwxygv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjkxvfzx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jintxsvt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qbyztsfj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ycxckpcf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qonxxskn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vgeolnnt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yusspbzt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ocdydyeb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ciyzpouk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wpfadyzk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cuutkdvu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bfeilwld.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lpbspkji.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3evpgyiwj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3trpzwxps.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fraytabz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3aqkmdbhm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3afxxvbop.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nlqvoftf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3uxqxhszf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ibmhovhf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3awcqebhf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ethfwblb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hvewhgxf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zjrobnum.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wpxbtiaa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3frmqgvin.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zvbddtin.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3phigillf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dnanobyl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gehzkoum.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3axeutsuw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qtorfnoy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mbfezfzf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsgsowjv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3tjxckabm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wavzjkxk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qcikpmnc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpossqgc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zbqgflou.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3krxkkldw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3niscnrpj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pnxqflnr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cmwvgmkg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kpcnhvhz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tutwykgg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3swpwnaly.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cnshlnkm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tcavbqmx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pernytzn.html


<!-- 参考信息 -->