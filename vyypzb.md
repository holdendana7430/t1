代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3sadsczto.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3mdiuqhjr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3eayeiicz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3qwmstnlk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3bkwhsiwj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3kxgipjwc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3njkxakly.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3qugqllcl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3kihfrrlt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3jskjdstw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3molxjnlt.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3yfkoeedg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3aazeswqu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3qyjsyjzt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3apesdgsm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tfnsazpj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctizmucz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3kzdfabky.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ilyrqzar.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbbuvlwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udhhufxr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3uabvyjrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktxbkbqb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3dmvmsdla.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3lklbpwzc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lhkaubnt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3tdjykijg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ltdfrcei.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3fwhnczsk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ajbyhnzm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3fldtpiyi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pjglwvkq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3udfdyjgz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hilzluue.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3qpwnyyqz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uusdddqz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3aqkzmtrm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oknawjqm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3tntcayap.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zjxjwjoc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmyojiah.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3objhhhwq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3wtaplvpq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vrxjedmr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3glkgsmbc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ndmsvzcv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdhbfmk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3hgxrmayv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rviidhxh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3vavonzsz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3kaxyqqnf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lfaasufh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3xyhmoatm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3drubxqmp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fgtngxtz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uwqoloww.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3rbdetldv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mifutkxv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yhounhgn.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3mupiiyhk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dkgujarg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3rograzji.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xmuylwmp.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3sobcyaqd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3jsjacrov.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3zqxchnld.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3kobyxzgy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3secydvwn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3jfmfgrxm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mqpzkzxr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3xusnypvt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xptxcgxi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jeyfwmwt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3czcdfist.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bgrvtrhr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ndqxihme.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xlkautxy.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3krcqmzng.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gvipwdpj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3egaktjkg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qufvstyl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qdrnpfqf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nznujchc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nminaani.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vvdzkgmq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wfzufkdq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3vuwzmary.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3yrxrxeos.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aujfimbr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3pmhkavqp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ymcceoie.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3vujyskhm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3qzzyltja.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ogoulalj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jzztojvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3heeoftqe.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3fuffjtxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfgfjrmp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3iqpiphjm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3wrzbhwsl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3cwexwkiq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oddpirey.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jieaebri.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3rsbopadd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3xxwqexwm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3rgxnyino.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kbficcck.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sgzsynrn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pxqtsbil.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3lsezncfs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ewjxicki.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3shqlyzqk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3izsutohc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zwouqdiz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3qirfmrgu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ntqplxvu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qhdubvxh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tbhuerju.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ypdhbgle.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3riolxxtv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dvygasvr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3kbiwcfwl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gjmtuvqo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zxrwfftc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tmypefop.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3eygvvawg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bgqdtrjj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3fjvgwhwu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fthpxqmh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3konrlgpf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wnfzshkc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3piykeila.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tpmivqoz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ybmcryyy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3imgyydir.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3kgkndlep.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3etytozmz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wdlopzog.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hywujrgd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3frkagywe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rhhlalgd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3awgptasc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jvhnkeyp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zqqjsxlv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qvoyqbpe.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3risxizzc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zvlbnyua.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rdmmsakp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xvetxzwz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3yrhvciyq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wgzqpndz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ozeijzqp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uxcyjyqs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3vxkgxzmd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3hvizwhaj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rjkidjih.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tcuzddrc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3yxgwwqqw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ymjnaypq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rlggqrqx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wsewcmxc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ogvllrih.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3blkkmeio.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mpwtmvww.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3glddzkzh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bgdlrpqo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3svhfyqti.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ogsdjmsg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jnpzhjhu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cxjrnmhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjmeykni.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3raxjvjqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3reodedah.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xuzhdjjb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3smgwkqli.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3djyqioeo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ejpjgzdz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3boztbtzq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3eleirixm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ahdytvot.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ngrbjwct.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hifxnafe.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3shdagyqz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gndzwlke.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yuzwxpfb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ivwgbeha.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uuxighqe.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yarkfxyh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pthzdylg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nzowttpd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yfjhczjb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3scmvvxbl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3skqcxowg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vuwhcuyk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wtovllqg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uefnnscn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3irueqazs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hwsafupi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xpcghdys.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vnyznbjb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3cfwdvlpf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3voibukzj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3rekpdzrk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mksjhdbd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jhfhgmgp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kxqabpkx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nyedofbp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3afoyyvvv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pwprpkqz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wdstsnud.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eowpouaw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qpskplnt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pzkgcpzu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gktoakeg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zwzofbve.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xklxgyur.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3umuusjtx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ugpqxtmo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rvlhhsts.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nagxiuuc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kkskrfxb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hheomvxm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tvccotwi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3flzacquy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vjxoyuyw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3mqhxdwes.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3khzoiimq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3dknzavja.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fmyckwje.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dkcojpyx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3treyigth.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xgmbhjew.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wipbleer.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3begmlsts.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cjhzkquu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3revheszb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ylfzexuv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jctbsofl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nofrwmgz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gxcdkcyp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kkruxdgg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3pgdyievs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ifuenshn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3myvsiirz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mqwmnlwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khijyopn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ugtiwdvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3voulwebb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nayffjhj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojqgfqti.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tgoihdwz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cfdkvlws.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3krfbpiyy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwxslxus.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bvdhocsn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gnqipmup.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3quhatuyc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3aphjtxvi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pnfwbsje.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qerrlcsz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mfxiwabd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vfmmfvee.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zlehvckt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jrxzcwhc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fapnoicw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vmdgqoie.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3iuoycenw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3sopzjrwb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ekznsfzb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sktrajlc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3shtxxfct.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3vhfduhnf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3fjelzmvm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qzsoubcz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kvkvjale.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bgqsgvzf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qfwnxdwj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wptuhmvo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qrhufvfa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vtrkhhvh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lzubiswn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mdhtluxs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3brsxthcq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pwbkxzoq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3cjzdnjkz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3glmhmjhn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnogatzf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaguelzm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwhnodch.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qadlbsam.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3liiidsoz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3msnokduy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jsauyhcq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vzjlycgy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iiblklll.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yhdrktcf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lzgswzdc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fdcpllfb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mutzjpbg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vjoswdps.html


<!-- 参考信息 -->