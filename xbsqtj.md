代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3lolbzddy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3bhgnvusx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3pxcomztz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3zzmveilc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3oeeawata.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3mezrhfpv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3zjfuloxa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3gloncfht.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3tdgguojt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3phsodywx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3doxttott.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3zrtjhvqv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3oszqxxum.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3iwmbfdzl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3madyxucq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pjtalerx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pewninbs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3buynjvqh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3tdnhqkyx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3iamlhlmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arpukmuo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jkdqsixq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfsjribk.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3muklumix.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3msdqznkk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hneetofm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3tnzqqqui.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ufslabey.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3itpdytjk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uvulkfmf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ktzrjccj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ivmrnpnc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3uaotkpwy.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnrlpvfy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3jgesdmcm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffzyupdm.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fddsptat.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3blrzkuix.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xnxyhtsu.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nljmbfjy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aplojhln.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3nghwkbfb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ymdwqpgi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bylbescn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxhxgkcl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbwnchpv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pgppylpi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3wwhchppy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3fbbcgkuf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3laonqcod.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3zbuwqswy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3iagjicjz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3mmrzyjnp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tvljbomz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3toktosuy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rervosnu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wknlewat.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ssngaavk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ejqufejb.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3mzrjdzpq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zlochqwh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3jsszbrqw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dvkkruvr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3npihbwai.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3rsclhkud.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3cjnmkdwe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3uvisewqh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3fdcmlmru.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3nlicnepm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nwnrqbwi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ipjkjuzp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kuzygynr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pjtbnxln.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ngzdrhzl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hkdishec.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eelpxtxf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wfjyxzvx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3zvqrpawf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pcodekwl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gtmyetzb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ppfmmqye.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gjtfbsgy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uzawbjtq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qrmgjxes.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nyjyhsfm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3atldpqjx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3chnahofh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3xfqlypfb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mrmnajlh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3csnjpgkr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xgdfvjvk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3iblumybp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3napiakdx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3pxndpyog.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3paocvnfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxonfaja.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3thrjhfdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yawlxvce.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3riqpvjea.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3zveukcxv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3phykbofl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vlabqhdv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3crdcapcb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ljfoqbhm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3laxxcizi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ptzpfaup.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3nkvwznpy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3poqekhfu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wnvbnykr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3qaagsvmm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fxgttljm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3oetcicis.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yqhgkysn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3fgpjlhxq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ubshvvkx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3pvzujrhv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wssasdfo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3fvxxwyki.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bcjbzsvz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tqbapgpu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hossrcew.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3pcsjspai.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mvogadvs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3jgedsmfx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3avevfnuo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3mokedjkg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ctnjalqy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3araqwcpf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3elkvilnl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3eotgsixj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ghktbbkq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jvbvwqay.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3fqlliwnx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ysoieuyn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3kdotobch.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tndnzups.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qwxafnbv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xhiroenu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fvhuvsfa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qfvxzkzj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3oafcumor.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3plvwhtdb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3esnnvfcz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dfgfghse.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3czlwhxtb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ytsbgwww.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gnpvejzq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vtavayfe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rzxkztow.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3txbhfvba.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yhblhqsq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zdvfjver.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ocexniqu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3affowgrt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3svhiuwjt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gcxlegph.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nkxowcdp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qghawppa.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vlsqnfmg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ohfanxar.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gizalpyl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3bevddeqj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3dnmzaruh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jhhvener.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cqdltavc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fflbadrc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3estxbkkx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ebhjpykd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3oiljkiiy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vetncpch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3duwotmrj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3zssptfnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhswehnn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xdrorvur.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3prqbqptw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3zczcdvjq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ztjiktxk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cncpmjcn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lougevty.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yxkkczef.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3yxoblkwm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jmuzrurm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3owiljvqq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3maandacd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qyhragtc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wknzijre.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lzvtnasv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kimfljhq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rxcrfxod.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ihruvucj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dzkmhfow.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3cmyveoxt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zkbalfds.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3bzejvlch.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bgoeckff.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sqlkajzh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kndstaua.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3luovduhy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rreqywtp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kuwymeue.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jdyqyjul.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bwgbohfk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3teqppuzj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3alqmwrhl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vbxqfnod.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cwhtguei.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3duftzpbk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qlbxreiy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vbibxsbk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3eerjwlxl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3brhlufdj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3smyixgkd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jdwxrkkx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xhkzxjmq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zbadbnjf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bqtqrqqx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfxiuhtf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ashrzgfc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3awkvboml.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fhsaudbr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jsbtdlme.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mdijwnbo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tjysvokj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jsjldpcb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vgmcyddv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pvsjsffx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yksgjomh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3sozeiuib.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fiwtjzex.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3utbtvxld.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gttbcjiw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ivtbjoxx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vvseznpx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3prwrnrfe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3flnsrlqg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3pizsuhwm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hwwpnpsj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qgoxtydi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ltqhnylj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3erngzzmi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zbjoccwk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3boadwrtr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ywwmkhfs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3iwdeqtff.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zqxtyels.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzqdfgej.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ajcrkwwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuciegka.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zosltlui.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fggioqbn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xuztxsxb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uzwdxxal.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3muxijoiz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gcpslnwr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3spjheine.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3qftfbocb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ekgnwldq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3bmpqwhkc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pktrmloy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3noshnwij.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xuiclmqb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ambuixvd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3yvgacgqo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uupfqxzj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sucfbgil.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3slzfqtyq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3pnnohbcq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3grksnahx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3nokdbdbb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ogsjjlsb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qswbvomq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ddvqogfu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3svfoagmk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jegpkulf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ypixunui.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3zezdxchl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rltotwgc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3iroipian.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hgurkdae.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ncnxxkwa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcwbnioz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3btozskqm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jpsnadwc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mitlcxfe.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3esojbexh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cphpibdh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuxdyeqz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3btmryyan.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sydciuwh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3otivppkv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xgbzwzty.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cieifatx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3umemtezt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dpcxtmas.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lreibzjc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3osfsydqz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zzvqrqxc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3admvauos.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3guoxzrfh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3idbcrlvb.html


<!-- 参考信息 -->