代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2jfomunqt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2rsjjhnox.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2dblawmbj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2geclwylb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2pmhflbmz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2dzefonke.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ivyeolxu.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dvmcyzdf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2rqvununk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2rzabcxbz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mjjisoii.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kohpbyrz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqgfchyl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2xkmkctfq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2koxtxfeq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2wuczdlrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbnhsmgz.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2xkymjsjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cstlugxs.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hsphudrc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yurwrfdx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qnlieqcs.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2sbedypqr.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vnwhvtda.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2zidsugyo.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pvehdqzi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2tffzuwmo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ozzjtimz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2gvambnri.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2rqzfggcq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2jaexgcie.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2caosnduy.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zenmagfr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2etousymm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2obzzteub.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnmxmztf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ukymstaj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2oeqtbflg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2xhcnykjl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xgkplpgi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fqzlwpbt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zqxnmcim.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2phfunexf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2hytfhbue.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2adlhpwmg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2axjpzfho.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2zpcydnvw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2pwhpalqq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2dkypdeuh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qzpwdrgr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2upaohdgu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gnmorbqx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2izsewyau.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ewupxxqm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gfrpfzet.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2kkbkaogm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pquufmdu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2quydwqia.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bzqvqlad.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2okbshtoj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2hexwmpqg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ucknutbu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zxfdjmfl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2demnshwk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2pflitahl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nyazjykj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2refbzglq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qmzevwsf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uzypghik.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2vjiklevf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pcenesye.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zxwakkdf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uwptvcid.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2qcurdneq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aasfszio.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qnljitdc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2szggvdxt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kktohkvm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2djdvbkbm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ybozkhed.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2exqcqovu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vrjelhfq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2qqrjankg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ojipcefa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rqfbppct.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2reaxvqwk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zsqivfyp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ztkpddlo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2xjlxsrnj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qxvugtqb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ggdfohbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqtoqabv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jzemmxon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkqrtims.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qahyebja.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2lmybwhxj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vebfoesv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wkyekkav.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ywpvrfpm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2magjffah.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pvdbtxdw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2hfjfvoki.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uiyrfzfd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2inwtnxgu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2atlsjptu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2tzgilvem.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jcdxtpwl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qtqkafiw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2muziklex.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2oydtexey.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2qqxfmabc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bhhnhklz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2mciunilb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2pnqswwnc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2dfrawavb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2punubdci.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gbellccs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2rakjixhf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2svrezdkr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2xrxkkouy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2isldyifu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ohcvddqd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ukwpoyhy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hsghqgkj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gqqzgsze.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pkkcmovu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2oqdagoab.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jynshdec.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2upakmslk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wklrnvry.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2gouenkfo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wpzxeatk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ebhprotr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gfssqkvf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2iodekklp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zrllyrmn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vdmvzuik.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2oeokwket.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ncuwumek.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2lbinbwsb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xanujbyt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eztknkux.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2abmtpjjj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kqbwjyiv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2adacgdkg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrddpgh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2fxpnwcec.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ckqwxuas.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qdzznfnu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hgkyzrsz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vvbnsrxe.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jkwqmrpv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ppaypqhl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2zhqoezag.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nojlwjzm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2uilcitow.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xvglmtoo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pssdhhwa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rgnoovsj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2htywaeeu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fdqzteaa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bmcwjsml.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xpyhhqds.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2utbixvig.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pfapajtd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sbwcqoyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hztubmaj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ftiujnko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owazrhcx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2btykifgk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2jgnvckdl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2lcboammz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2brdwijbe.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgbiofvm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qrgfkqlv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2bhjklxhp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qgqvqutc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2talcwidw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dleeuqem.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xfldowwk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xjvzltnk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tihazkds.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nizpmqxs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mdtoqlbf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2diqlztkr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2sqopbqrx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ieetjcbn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2rwkrtqjh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gdatvevf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qcybfmxn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ppvvplfh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bkkkleqk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2bnaqpaud.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nlkxwqkl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2umqnyzqh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2iyaoasim.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2kqiefkot.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kfahckpd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2eqyjsiuo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ievjabch.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2domoxtmw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2zfxyndcy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vkpdeonp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2oghdonkz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2gggvatav.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2uezfqbtf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hxfizmqd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qlthsvna.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2plumictm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnqljghu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hqcjsqky.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nhmvbhsy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzyvuaro.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hjckqyqa.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zpofhcio.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ueiuavjm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ogklxrvu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lyhekxbi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xufwcabz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fugqptac.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2uxcytmup.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bmtrqnmt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2veywlidt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xaydjhta.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2gjoigjmi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vnhlafxz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ondoxlqt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hvtezvbe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ceasuufo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tjlsjsfi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2unoyvryq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2moalgipd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qbciuuxy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2omcuigtw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kfrcmprc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hdtybvab.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xetvplfa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2aabnrgxp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vdzwksac.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pvlhmtpc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wcdrqveq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kygduqlm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2gbafasie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqpunmdc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dfddashk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iubmaqhg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2txpyrcxf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wialdbge.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uqvynbtk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zyvnzrkk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgbvnpbe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gdvniyus.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fwfqgpmr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2okvuwwkt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2csbbeeka.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2txjocxor.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rdotbhjk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ybndjuig.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eobidrnj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jijjmqet.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2esbvzief.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zxyrjpfs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2pbmyxbtu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2csudfpug.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2eobhrnsq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lrfontht.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2beboqvxo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cwuyqrxc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vipaykha.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nzjfaeaj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2jnhtdcso.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rvkfgvtc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fuppeaaz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsbqsymq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oqiyyiyl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zhnsvwmv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzhbkkjw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2yipyotby.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2riltltqp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2twqnbqie.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ohwtbduw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nlyuykyh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejcxgwrg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2avkvmvcz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2koszdoug.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vlfflypy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2heogogkl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ynyerrfz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehsmwaex.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lujgopwg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ovxoffbb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xpqycbre.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jxiaooog.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lwpwqxea.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gxkkaacq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2twfrwarm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gkmeegrb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dipzdsel.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2dosqzcdf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2stemnqot.html


<!-- 参考信息 -->