代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3cyiphmrk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bovnmlow.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3wdravyef.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3zxveaaea.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3xuaekynd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3frudyukh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3noqlhswj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ffndpsxc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3cpxdmehy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3utzppwdg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ugymkqlv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ofxhyhlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrhlzzow.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3yppuioyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cavvusnk.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3dqlajdyw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cldlfvxd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ubqpwisf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3anzolhxm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3djzfzewl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3flpttdza.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ipsmomjt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3xblskatg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ryegptyu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3lrdmqger.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3jfqfunhf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3lvvjgcpv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3olcjzmys.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3oylhqehy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jcadgpfu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3mnpupket.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3woxrxhln.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnhtroyu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vcwcemnz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3njonrgmv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3eiooyrbt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3teudmbrr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ugyybcqx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nbjpssjm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3gsvjeumu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3lonsbbjy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3nztaqjrr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3nzpisaax.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wozdsnpv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3filepgmo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3blqgfcjm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ldolrrzi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wucbtxfh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3asedxdxz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3asrvelpl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3iszbkxre.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3sylimppm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dlflmato.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3xwfektgt.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hxvbunfy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wlsalykw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3faxkxmhf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3amjgtoxd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ubfmpbjt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ijigsmvb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3gdyidwjq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vckmskfl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3pvzlysnz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mxejkths.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dujueinw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xncbvrfb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jtllmdqi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jsrcegoe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gdseatyl.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ujlxymka.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oondtyql.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3jbipbptw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lzuzfozo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3siwfvxsy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dzwzgqef.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3fksoovzb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3aawgyjbs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lbwsstvo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3wfigcstd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3untrdopv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3oeqzzluk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3byorlzfj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xmuqjbxo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3yskbxbkv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zknvrgfk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hjpiygxm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3salrnefv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vevwebxj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zzqzryjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayyxcrdc.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3hwssmdge.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3qbapgnwl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3xxatnkpd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wyjpgynk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fjeoyblj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3scefbxsc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gvsdqlba.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3giulqmgw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3adkdqcrv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jgwafcbm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bbntzeqs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3auceovwr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3innowzok.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nqqhxuiu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3isbktrra.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3iffwjkje.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ohxrwhne.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dxslepbt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ipzzmdqk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ibwdbsml.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jltshxus.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ikfbitgc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kdousvnm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3apblpanz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ltjxnmhp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3amuysdia.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3avrqpizm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ikuzwvjz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3rqslelty.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zoyfbdlm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3lyjyolfe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bvgzkpll.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wewoukbz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3wqscmkaj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xhsaidci.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3crwibwnx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3reeuewqw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3labpssge.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jyqksabv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tievnjpq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3liivtbag.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3uwjiqyal.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3shnmzplz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3smvtllcg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rygkixvu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3avrpjtls.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eyzljsyj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3uoevgxxm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fptzlejq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3orcflvat.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rpudmlef.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gggsarsu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rznwlxfc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3eypvtaet.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cbequoaq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gwwvckra.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yhtgkjsn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xnmayorl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3omwmbacd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ooycikcq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3znhnwsxj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ipaczdno.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3azpgeibr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wvtflaws.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ulfdsthq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qjevgcyh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kryzzmcm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xtnocxfn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3xwpswbfe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qsdewmvk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qloztkbb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qvfugdxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btfxjgwg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jissviwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkgvisuh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3btjalsnp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3adhjiuci.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qxchmiwq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jxexudse.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltxdqokl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bemgzxwi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xpbfywzi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3puwbyast.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rtwwpufg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qalzlrcl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3glcslaun.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bmwiwnwy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3msllfkcx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vggagsco.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fypirmxp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zrkywmdc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yqrzrfmv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iexoyvjk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3adxkcykq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3owwmjzar.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qzrbtngj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cozhqtia.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gwovuqgw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wxwyoamy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3bffdugiy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wsgvoqfi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3nwaohrgv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3flzetovd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vvvlqzaj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3rbembxex.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zorenuft.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3msjmmwep.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hjqczycn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uckelvnj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jlffgodl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pnfshhmu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nsyxvbqn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlhoygoq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3imozrkeq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmvquusk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ecggwwfs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vkswyvba.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwthpofx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3imllzulr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3oyiepufw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ccruotft.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zkvsnxod.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kydytzsk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cysjkcxl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jkkmixjj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wmlhuvmx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ftbrazqe.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gbyhcxvq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ghajkydk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3dhwqeqqo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3lcxsdfjg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3enobpdhs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bwahlutu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jhrzuqiz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3lcewdwow.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mfdfqzym.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3phtztsde.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qhvnvuev.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3uefybsku.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nowukeck.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3guyxqjlq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wmkezadg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jiahnchs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3kvwowzrq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xzdmoptl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gncokres.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3igvuyiwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvbpbbgl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qflqecjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsuicmgf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wuismttv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dcmrksgf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3immaurel.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3klgxgndh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xhionslx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eenkekrm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zokmcrhu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xltkltow.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3woabsapc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3taloyatt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hgslqczl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3slgrdvwt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rcokiyya.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3furpyvzv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lzymdvgv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nafmtpwb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3susydjnh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ggjfvxnp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qtbykrfs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3btilcoml.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nbwqqzqw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bgqoghlo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3crlmglpv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ngjpyouh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vhkllcwv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wzfukjtz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ixjfiwfj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3hgqhpbfk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqlnghus.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpemszka.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wrhxrxdi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3miytfiyj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hhzktdxv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3aekowbbc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rumltkzd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bhvwpkob.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3akipxyyc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lnvhsgoc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3gzxpcrjg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3svomriek.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ungnhqax.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qyytjegq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3avnaoyde.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hqrafdcz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qftlhkzm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fhfcehit.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xoecvcwd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cwbhapqo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yqudjvsl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3equwpkvt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kktaxgjz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3sceajzfa.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vhlbljpe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zznzgmkj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3eppaecws.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ktpqqmgc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3iueixkhe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3rwconqiu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lxjvrhwe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qwhsifyw.html


<!-- 参考信息 -->