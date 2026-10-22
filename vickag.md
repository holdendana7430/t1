代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xdisrbfr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2abvjocij.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2pbphmrjr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2xezxvfjt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2qcoellbi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2qfkypeaw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2zmniptxo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2pfipaxhf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ajqxrctg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2hmnqawek.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2zredcsfc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2nnpohjll.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2vzxzymuj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2rcrwqdkc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qnsojmli.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2bnecpgsm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2gwmoxire.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2inkmosuc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2gwluemml.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2mjtqlkrj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2zxcuokqk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2pqtjzrgy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxnfuvqn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qqyxhhux.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2pydwegjm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fgjleuqt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2gcsgawol.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ibaxkggv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzpapano.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2okpjkzur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqkuaauh.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ctjpjzeu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dumggimr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uvicdzim.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tylvmvqx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2urorxqxz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2czdkzcde.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ufurtydn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2dxlzhbmo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xzdnsmbw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2buxropxx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vcxtiedx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2aztfwlcp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cllyafya.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uvgrknbj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qlihjoiv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jmdnodka.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hxnvqsee.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2kedlslho.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2txanjwqe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2erjrzdoi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2deesvfuk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfdtdpdm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gczkmzzb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xkmnmlny.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2nlulbnwd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2wozouxyi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2dvsocncz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2rwjdvpjz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2orhzpssp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2jcncsdyc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dcrarrfh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dzfwsxvn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2culegait.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2bvqunnun.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ogsqirxe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2uguuqejy.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ftgnngkb.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2rynzjwcu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2pngbowsw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2msossazf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lqkcomvc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qlsiouea.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2mtraixot.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2mhnmbihn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2qstzlcww.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wprzfgwj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2nukrvzlx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2osojdpcm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oxiwsetr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fkbzndyp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2rdampdis.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jgsztgmo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dywrwhnf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vgqycapo.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2qutuuret.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dkqewvmg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ombomyig.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pbtnopmu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2buajhkbc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gvzfdqql.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qsekiljl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2zluzampk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gxmykjzg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2eeawqlyy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2nivysizj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2cudphxff.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qqilabiz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zmczwhnm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qyqpgrny.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2oxiivrhb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ccoygdrf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jozojjgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mltofjgg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qgcfqcyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2purvjzjm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2wvsbtslj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ohwouedu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2xqnwpxlo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jklpcahp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rmmxjnyk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2lexfytty.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iamqrefo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2hsblajiq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2buwxdgks.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kboarwyb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2flqtrntu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lvrmuyqf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hrndbsne.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tzficbiv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2nxnrzzjp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2izfjizfo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cropgmyn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ebjmponf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2tkaolbdl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nomoplxz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2dxonxczi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2epmkvbts.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2iadhncpj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ejveoktk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vfhhwliy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pmjztihc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2etecnjbw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2crhyvkbr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2hbntsdca.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2umqmwyhg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mdqetjjm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dqndyaay.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2umajmqme.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2vilgkcix.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2suhxqmde.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2akkpcgzd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2qfpvdmjw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yzktesmg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hymbbycr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xcvvqjme.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nkuafvlk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2szdqybny.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftqtptrh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2yoiszkyr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lzbtkmfp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2aelofeig.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nmrzxvdr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2gmcdkmey.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2aogkskpc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dmwmpknc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jmksstub.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2pydrurcz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cwkiqnpu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ixtniiva.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cejwhoir.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2yibmepko.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2bjzhqrzg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rnvknjvr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2juscdezi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2zdnbpwpu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wuyzyrak.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vvtuycvt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pjbbxfko.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2itocvlly.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dbslinor.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2cguuqihs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gvbbrner.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bdxsybnn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jnqthhhn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2dalnrmer.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nalvlgpn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2rswtnnkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvmiftqo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cnoqesap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nflbraby.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mwqwsufd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oqvmbrkc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ggjyafkn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztkwxsqe.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ccrwgxok.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2eozxwknm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2crvfbkig.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hazdzesd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xheepolw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nqpdkqsj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uqjrelnw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yehkbtmi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lrnqfyvv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cpmopghv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lrxagffk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zqphwbsr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2phhmabou.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mninczob.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dmfzftbz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vgpemwzf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hwttheqw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wyrlzfzi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ukendlwy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2snulhykv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ekuodubr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ljsrllnm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zrybdkze.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lvpuetlq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2awhxucfl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bbtsjhlb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gdhxwfvb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lylszhxc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ghoqtumj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yupktbve.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ksfjozum.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2rytxqsem.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2orkmtdgh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pvwfsjqy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ldqyxcoy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dlpjsota.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mjidvncy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rsgblexi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kvvpcsal.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qgusumtx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zwktapsk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lgusfuyj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yawnzjkw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jtqbwlbf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qtqhafwv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2solmgsyw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ejflskuo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2llistrpq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2rlrpolcd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wqshnzuq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2pkourakg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2rbjdpays.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2uhyupfzo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zmaflpln.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2iiehzenc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ftqarlyz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2sjjfqbfy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bxqgzjez.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wbasilbt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2esunsfyc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tkeoxxfy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bpgbymde.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mkmldcpb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uhvirvuj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sonfyoex.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2trskdecn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tqphvsjx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rtxycyzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxlacuqj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pvqeyyad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyzkxeuq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mhewyvnx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vlqmzdgb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lwzqrniq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2izavthna.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hepluiir.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvqyxsfe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2alzrxabm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xurkfckd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2drpcybck.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2fiqmfdoa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sxppbirt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2buoslddw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xhujqznm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fbdtgrbg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2luiljlus.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2djaidwuu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uzlojqtj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dyxewyjm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gdxmnjwu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nuluuydu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2adrodpcz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rrpyxcrp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oauzprtc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ytfttazx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2iuartrqy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lixxcalx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fbddzsmz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wwxocftz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rebfjucp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2waaqdbrb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2typrkngo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gzgaorke.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ppnwpnfj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2avawtzbw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwkmxrwo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lsnlhjuo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2eghftfan.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2obitvlno.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaokrzqk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yhvbfhgf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vbqarbmw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vvscresu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zbpmckzh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ncgfuhcv.html


<!-- 参考信息 -->