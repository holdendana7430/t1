代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nbzuirdm.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2jrbbemsz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ojgrjske.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2mxrqpucy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ifyomjfw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ileabpmc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ptpjfksv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ziasiuwx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ttplwkxy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ideybftf.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ovolnnfn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ypzbcvcc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2fbnijmnm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2dzhwlyhn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2feirzxbf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ndfnranc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2bpugskck.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2wnzgsyiy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2skjerypi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2aiolvtue.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ncjtblan.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2wecgycon.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhuttmom.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dkrzqvix.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2dpdubvgc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2mdwkmvpv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2toweqjqd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qddciwmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjsfgjhy.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qvymwtuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srsreilz.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oigzijxp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ecqbkoie.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rqfiybyl.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2mqzbmynv.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ihlwpuny.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2qiacdaph.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2hfwzxdmf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ypltvnxh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jcsiildl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2pwqjaxdm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvbsiaku.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2brhlfmtr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhtvkrei.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2eqspixsf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lszcyjlm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ragjparh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vhpcbwuv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2gzfxdlwo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2xnmooimo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2nrfbsoee.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vxcvtngf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ubvaizfr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2exojyfmr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kscmikaj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2rtnevhuc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sdgofkzn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2nxuddbow.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqsxehue.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lyodcgdu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2sitmxkeb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lxxjldgc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2kepaivbs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2juerftsc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ggarrnve.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2djfobzac.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pldfkssw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2pbtdfiwm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ldflkhez.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nmcxargi.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yqareeak.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nszglpdb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2yuuxowly.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2cpuhdhwj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2menmywrw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2evcfezhw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ynpfpjvt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pugjizph.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2gzpljysp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2emcfitmt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gohiigdh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2drdtueim.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lnsostxw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2abxkijdd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tvjzbtnq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ngpfbnzg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxmblkf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nennimms.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2svgbfpsn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qkkjiiql.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fpogeojy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2wrsbonlb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xuuvwmoj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aodpvhin.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2qizgzqqx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ypygqoxr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2nyhyvtbm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bnpxvnhg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mvdfydab.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2rkqqrhhw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ppnylrfk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2lfnyypaa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ynoejkhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpgjwjma.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ggnowbiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgaxaovf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2szlfbiti.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2tmwpyoxy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2nfrabtkx.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vxjmotox.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2twblryes.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2kakxywyu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2oearbeam.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2sbczjlhi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nfhqsnjq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2txcqtzfh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jkyjqwzk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2avqcgswq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ykyyomct.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2odtujhfi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wbpetnqr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2oqwmnlit.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2dhjckjsj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2jpnnyres.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2eqfvbthm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2pnnoyhqq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2omalmdxs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lbdzoohs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xzjisfkr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ffgxbcno.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vrfowqbf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2udndzpbt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fkaqkces.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2msjbszla.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hvdnabqo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2eeospztw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2poxhiihb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lhcnwnxr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kwvekkks.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2tinvpqjj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2glevvvxa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2qnxvrwiw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2frebijvk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2czepoozt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2vputzrio.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2iusoducn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ptadpnyt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2acrnnshc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ospfadqi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hwcrxpnf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lvrhcskc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fdvuquzj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vwomrkad.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lzrdfnua.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rdoltjpy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fpgnjugb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qkcljrnh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2btxjulci.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jswnapak.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bmgjrrsg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2evaerqyn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2sozetptd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2uhbscppe.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xfegfliq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fqpxodwl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vuzmjgpp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2koyjhhmi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qkszjhes.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2flglmtyo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2iyfntjmx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vtinrals.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wgdcbsqo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ivnavotp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yzemfoyx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2enontzea.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pnvvntcs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yvhdjrnj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2frflirgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srwquyvn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2wvkzcuui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyjkggsf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yyzpyiaj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iznpclly.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wpxuiprk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2brvhvjly.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gblmvgms.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2syydxmgt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mygrinky.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2kzzatkmw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qudqhrvk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iomgeoti.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oywmavxv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nhphohez.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2czyspgcz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2udtmgwnk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2goazphtt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oayibpza.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2pdgcioiq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2edrnrqoj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qtkkznkm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2igfiywuy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tfrvxmva.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xugvfonn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wmvakskw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2khwyjbsh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jjcijphb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2vwtqgthk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bkpszetm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gdimmxqg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2brtjgvvl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2exiblpcz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2edzjmlkp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gjxzrzxb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tkprywrb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gpfcssqk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2yjfsjasz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xsvajklu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nmvahuul.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rfnjrsos.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jjlnmuyq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lifqsmvu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gyobahvt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vcqwahiy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tgfaxdhn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2oechkivl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yiwesmyp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pjuhomky.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rqcpoqua.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kqubnemv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tpzfjyku.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qvdaosuo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xpsiicol.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tyxgkebg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2yxsvugky.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2axtdyhqr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2fniztqhu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tgybdshj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xvoymkrh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2debjejpi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2taajcvsk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kugopaws.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2uhgkfulf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2aonvgmkb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hwkwkmvl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ycltlrbj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mzehhgfn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mxzqbbsb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uzepriek.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zqyfleod.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ltobzdlz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2nshcspcz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2krajfhhf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2riqvagqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdrkrelx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2prchmguu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnhbyrdo.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2afedehke.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dsbjkdtt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pfxphowq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xrgervha.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ixfdvnys.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yaihhegd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mcbkrkqd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xaxgoqpf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2awgrmbtl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rybwffnb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hxpgpyyn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tbeoibyw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hshqcnwq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gubrwreu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jwvrmofw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2juuscddj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jedcowtd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2gulvxudf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wsbxierp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gkmjbquh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2khdaufag.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2eihxwlcb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pdmrtxeb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ybcqmrqx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2efjgzzpo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mkwklrue.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2sskwfnjz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2yetgdqjy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ntnmxvbw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2alwljado.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2enorhkol.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ypihbvyl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nlxpxtao.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qzzugmvh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jffxshpo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zwrnpobz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ekolfezm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ynrhrsas.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqoxplla.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pufjwlfx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfoslcal.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2yvumuxom.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2irejcotr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rpopsmld.html


<!-- 参考信息 -->