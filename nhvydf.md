代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2yqksonjz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2cdvqrbws.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2gjtxfyfn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2lvrtsulg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2gdzfjfeq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2uvechuby.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2sbiwyiwh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ydsruxpg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2rdeyzdzc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2oiiieesg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugqlhrit.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rtbpbyuf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjgjbqmh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2dsdlenbh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2plyadihr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2houxuknl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmbmsphx.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ouuclupm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnlxgkse.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2mrezzzzq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zjpatxzl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ulyrrqvg.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2exhwkssh.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2sbmdznth.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2gtmeilvr.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxbvwvz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2miqugmzi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2znbpdlyg.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2bzionnjm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vouuyzck.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2lqylclyt.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lieuxyxe.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjnbadig.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oqmzyorf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2bkchrpmi.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvzxjurr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2juosesif.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2uoxnbpqp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vcqzehhv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ybboyjjp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2rgswjijf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bkndauim.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2jrvgxekq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2rgrsltip.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ulhovxcc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2dlrzdczx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkvbjymf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2valargvm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2bmaejxxy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ishdtnsz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ypfglklu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wnkowzub.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wlfkmvoy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2sdwqkdbe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kbmrcuyr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2lebcvaiz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2zejaicll.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2oycpthtl.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wgsinnvr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jqwumqkw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2yfqibkfs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2bidqysxb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2biqrkkyu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kyxsvgsq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2fatogqkz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qwqkrrvb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ayofpzxl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2uulwjuow.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ugpisiuv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kifddzwz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2blhghnuy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ualkpmxm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2chnqtjgs.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2vjnnfppy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2svifszet.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hialjpow.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hrsgwnbe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2foeblysb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vysiqhir.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zarvyoit.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2sqzaoloo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2epfamdpv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2oupifjlg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vupgikjy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wajgkffx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2pubkbkkj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hlpgobzn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hsbsweko.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wevprolx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2maufvpxp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2odqigrxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lruckrqn.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2hzdulrif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbdxkvid.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zzolders.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2elwahesi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2bcrwcxvj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zrhyhgaj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rhvkvdrp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tuyxyqxy.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ghrtnubl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2suksdzkz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2snfowfkr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xtkrmgwt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vgipobrd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mcoipgck.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ouurpkog.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cscmiduc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pscuxyha.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jdbihmue.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2axjiumwy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2cdwyqvfr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2wpxijdcx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2icknfmxa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2wxjihifb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2grucikzg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ggnmllva.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2fmwfpysh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lietypki.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2koirjvkl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mvuggeeo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xaawcffc.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dotaasln.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jaaaqasz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xfsmmsny.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mseytdrf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wbtwtxhg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2rxrvzmal.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2catatmwi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hilcufay.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ogzhnwvh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nsttfvdg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2srbjtzxx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vrrdgydd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zupuwcry.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2aejlmtdg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vspcrbhv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bomamczl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2taxvucgd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hucyshbg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vxcocnzu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kydeuimu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uuobamhf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vdxffcui.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ljtkofcl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2fbjyczvd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wpstahmy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2eyxjpctx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ecesqvqw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hyyujzpe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2orqbibqx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ywxhludo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qzvmoyzl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wledffsv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2omchifui.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2cxkyywel.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tqsmetqz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mxflxoyh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rxkhmjep.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2sbqgpnae.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wgfltnyk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kvhrotcq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2sdybcorb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bzivxdme.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ukulbpvd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yoymznbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvzvcnbo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2jhqlcbds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lablgqal.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yeqxgfhx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gdfoyqkr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bsmptpqu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2euwrzfpq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wfzxlohs.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fmrxepya.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ubjocdwm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2yijlyjlg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bpwkheow.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2eozxrrqb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ptsonvma.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2txastupz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2esfybmzh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vehuotqz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2blnbyawj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dodpkmkd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2pmxreuah.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mkfxsxxz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2pmzgtocc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jxygfnda.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dohfnvhu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ykpjxigu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zcpjlcmb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fsqhodpe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2aslxsifz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gzdmrkpr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2hogdrlgg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rwazyfnv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mukmrzzc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2uuqoebus.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jfgknjof.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zgbfehce.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qdvrrogd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2nymphwgd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2cakvjkas.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qvawzwmi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2oxhtcyao.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xguvhqzu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mpedlcdy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgmiwwij.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uyzugtjo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jyvpxegz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cpcnrjlo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ysqazotw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xxorgrow.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gpzpugcx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pxnhvqyr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nlznpxao.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2sxtqamfv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cpdzoohk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pvnixyqx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vobnrqpv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xqtgwset.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2hezkhjpj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2royswmyt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2adgvrvmo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2izsolcgy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ohsmcfhg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wycfxzwg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jybjmtuv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2rwglmpma.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zxzpvqbq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rbscyryl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2noiopqoj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wcynonpr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2utvbytwp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sejqqkab.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qubdcoyg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nlntctpk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cagvuype.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2glmxnzby.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2aimbkpwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdkjmtrg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ypopqlci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oysanmmg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2lmxsgqyt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oajfceot.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2msfgjuno.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xxycdvef.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ksnmcetz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrbumxpm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sacibiez.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2onqrbfrd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bzijwdmk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2csgwaksx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jxzcbscd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2gbnvhzkn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2izxecual.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kcmcbnpb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hmmumrqk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lojpkbac.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qqvgasek.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zdrmfkgu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2knodjypu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dgmluwwt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qaifslsh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2liqrfxvi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2oddymeex.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cgijpfir.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nwrlicow.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2pjfgjrqw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2thbxdibs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2aljjugsx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsxpdylr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gwkzcqkw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2upleehqj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ptjwadws.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgepjgrq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2abzzgplx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xuualmdp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2smudtdpa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fjikcjzi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2urkzgwds.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltoagjpn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cceydbxi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gnjfictd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vqeplmkr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2iqwlluow.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uzzufzaz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2juacwuji.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2fdiwmdtm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wddydbxm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vfzrmguq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2njzaflvp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tdfmmibs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ulclyrgg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ddwakuua.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tkbkvyli.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2efxtwszg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2cxietywe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jbmkwbwg.html


<!-- 参考信息 -->