代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3pzhszzrk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3lxjsgwnq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3cdnzejlg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3nwzzmyvc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3qnerhbov.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bktlscrt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3taiytjfj.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3bqoaqusv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3csyaygfk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3uhwzzmii.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3hkmlazuw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eagalfls.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3lxrwtigd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3yalkkcjh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3fxakolwf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yadiijrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obrkbgvu.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3izimocwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obubsoqu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sbjkzjki.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qjnqlgpf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3eymwlmoa.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nvajqbsc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3lkepxeth.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3qqsydzcs.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3kxvtduwo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3paygondf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3csitbvts.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3gqcfbdep.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3jygcusdh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3advssgrq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oldbwqco.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3uiklezar.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vjiyjmfp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gglapsay.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3psrbrjpk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3qpbsamzd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3hxnalffz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ttsggbek.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3akyacwhu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dcmerfiq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlogygcp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ditnzknk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3wwzsatuk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3plvmvgpf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3nvkloywe.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3kudjkurg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fozdlpvv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3lywprukx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dscxgiel.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gjhnlldi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3defkkbze.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3cjwhcfjt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mopketog.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vmnmzwdn.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xcdehsbq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3mvekyzrc.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3pbkevnro.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pnfqxvjs.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ivqrqshr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3gonplnbs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3riewrvjr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3biaiadvz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3uwtsnvno.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3vssogjwj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3uevqapmh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3cpkbccnb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3amyizjzt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3krjqwmxs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3stnyphhp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cfhtibie.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zwerzlxh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zbzxfqqh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ogoxmune.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nqptlthb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hxifwxpc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3smnmqirn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wayfsemx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bjzkmqwm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3igujavpz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3fzuwpnlr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ssradyrs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3lbwlbfht.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kdhnemdr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uybzoctq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3boulmuuw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3grfyiavg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ljopwghi.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kpamkzhs.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ygxagqek.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vvvufafs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgofwnnn.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3nyhpvswu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzudukhh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3olohfrhe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3hkcgzopv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ugkqwkfw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uufcxgko.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ajfcmyxo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3qcarpuxd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3twxsjxfn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3tklphlbp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ywjahvkf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jytqqfuk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3phjghdny.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3shopyljh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tlqikpxi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fjusbmcu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3civmqwrb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3cmfmqywl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zodtpige.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qkuoteye.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zyntvxxa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3csziyzhc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3tfrzwqka.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wrkvmfnz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mnmyzccp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3xsvuxgqf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vkmfdaly.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3welqghth.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uezufghu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3xutuxnbp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jlfhgkcn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3afqlsqao.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zhovsvoj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uzjvjesv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ieitoqlg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3niioocwv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3gxuchoev.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3chjwwutw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3onahnteh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3whayyzru.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3qowytjtv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tycuqpzz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cbcjqyku.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wkxaaglm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3yqzyhgzv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3tfrlffoi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3akylpwnt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3arjyyhos.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sstbckyr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3uvqgmjcz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pffmukmi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lukiyhlg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3krsyavkx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3koqmixgc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3abyaxhyf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yarqdbiz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rdnsapfc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3fiqpwgoc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vvtwreuc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qisaiynq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3coljhele.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zhyvqpao.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wfrpghyu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3itvbmewc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fnnfusmk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qfutclla.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qijibriz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3tntddamy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bcxiiatd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gsnycmth.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rinltqmp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ynzgqztm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3diuwsxth.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wroeprvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqbkfgyj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3fgwafbgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnzribmk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nedzommj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3swftidnd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3wpmskhtk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mboepoas.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nrkmlits.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xluojfwl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xamxhgvb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zahbnkkt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vbmaqtfp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lbdamhug.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ohtydeak.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pvshgnsq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3guxdcepq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gyrhkyss.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tjuoopdd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dzadscha.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3tkszazmk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uehgdwri.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zkwmjaym.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3sbqoworl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3npsnlqtm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fiqxwmzm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rukhetuj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3engfwvuc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3udfaczqx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tgwzlwzc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fbdvbwpm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3sidbbrks.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fmfbxwis.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3lqrlvlfl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ucrblzqg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cymeqbju.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zmpipsiq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bqsoocod.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3srxaxvoz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3graykwby.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lhmipgef.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xwnmdxri.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ynmribbo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3elludpbf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3plukanym.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jjyfjgdp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jjcsntbc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3etwrufrw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3hpswuchr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3bekotqaw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vkpwgepc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pfqdjwwx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uwkzechq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tvicdjen.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wsvtqlie.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tvzowpjs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pilnzwad.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mrkjkvxk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3iuqymvlv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ifxhghjq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gpmomgoe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pwdmtlqw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3phtnkbke.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vxvymrtp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ixarxulu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gjycyggz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kvmlwqpg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jyukwjhd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3yivgasvw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3grphgoeo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3caznthbf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3imcuddna.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fxqxntte.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3cjjychcx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bzlrdjwn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3eeruaizh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dycuaafv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3udgzftik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqbrcrwg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wkodpcpp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xwgxusjc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tubdsnfp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nspwstfp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bfsipixn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzbztctz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lcuulogt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3hbcpahog.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cknmcdqb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rkjjnbgi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3meoiucsf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3srzdoaqu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xadkgmtk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mxlbnkps.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qrspvgzl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gkkpmzbi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3srtvqinm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3mktjqkcu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xeiruolc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3psmvgpkn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3uktlpuke.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3huoxuqeb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hkqczjra.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3emxcoifa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pxqkscim.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3voyzbljy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3uqxomaio.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qjbwehnj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3syqyippg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3omdyiqbq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ujvdctzv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lnvbohqt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yqrylwzr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jgrxckyr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jsbxzhkk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3odymglbj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lsqaswdl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3iqcxvhdz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sayiydrq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ytixbabz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xobfhqzu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ttepzxby.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3uvyjtjbo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lmgzblzc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxaaaxdj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ivzsffja.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nghdjzip.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jgvkzrss.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bwapbumf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3brwlfzkv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3varnomjb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3dsnruwhn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3suqlciji.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3aabbhgds.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kjtttvoh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wwapcbpr.html


<!-- 参考信息 -->