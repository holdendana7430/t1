代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2hbbhhrfk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ydkodllw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2cdcacjlv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ozzydyky.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2gtobybot.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2obbmnagd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2oycwzfel.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2yqjypeqk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2aytarrzv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2sxhdinzx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2iynhvhcz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rdmgkkle.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2jzienpxr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2xwjdjixk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2zibvknmq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2igxivauq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2kzabfpjy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2nwjzegcg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oshugrul.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uuyxhsbm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2oeeqfksz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2uosubtoc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2lzhhiwsm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zlgxqunw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eblslzap.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2omvlgtqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abgkhcwt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2msqbxnik.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ufyelbmj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qbcplobi.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wbzzxqdj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2abiriqmx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2tflvltli.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ysgspvdm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2zemrgixh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2gvkljggp.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2gxtzsqhk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ljqcvaph.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2gfhpylnp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gipndpec.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uoyvpyrk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2npyqnhok.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xibhbhkt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2abxibbae.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgtloih.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ackxxhti.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2axdbpwxb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ewrbhlwu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jyizodrp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bbpuecyj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2htyxhbef.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2jwdzjeyf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xpxsnpnt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2uyisvioh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2nyfemshr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcbtfcbp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ebojbyhj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zzbuvmmn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yhepmduy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zjnyrqsj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2djuaorhh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zywdfnct.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hvuehabh.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2qrnivima.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2psgyzzxa.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2lqwhbidy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2swldnwuu.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nonqbnwn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qoewduea.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2eksrpaef.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2dzhoflek.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ivzpzcmj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2sofrotwa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ziuewqfc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2plwlxsxd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2muotrrwi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fetsfgjc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2omrwykxa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jypvfxcy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ukleovhy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pvyvdmyy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2fnvqhway.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fjkcmsze.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2uurmvmet.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ukfyrjkf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rursfhlm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vdixlwes.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ivxfkhje.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ggekjxwk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2suhliync.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2xlutebjp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2snwsmrtb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nzewnbxw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mwgbpviq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ecqzhxui.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2lgpsbjni.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ujvayyms.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2rdofsvyl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mwgjlvto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynpmmggq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jzinzpcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjjkzxkl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qiezkxjk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2otcjifzz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ugjeqape.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vuoosbvh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cwfnxuyd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2qmbxgmps.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2vftdsycn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2vjubtcyo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cyzwafms.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mvwfjglq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2cabvvvch.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2borhkayh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2repifzid.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ojrrqals.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qqvizcxl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nirznnfw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2uagmaous.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2cxuetuwb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ljfaexth.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2mgtbwitz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2qthrrpmd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2frdnmsao.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2exnibfei.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jgjyxwkr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2auqwhuhl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2edloauzv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rbhmlczr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2fsvmadon.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2csjszyov.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pnhvcsen.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hxexkaci.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pgxdzfbo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vprxzjgq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gveysixa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpgytwz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2suelsrwu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ikimciun.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2cvytszdi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2tzynfvwu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yantlqzp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2flurgofq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hvxdmmvy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ievhbzgo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2utavoivp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tcglvxlg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ihosgene.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lvmcmvry.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pjtkazqd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ydngdfsv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2opzatydl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dxiihbbw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2pejcroem.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2makseccc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wurvqtww.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2crrlqfdk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hglxfqus.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mncqheue.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ojxvmhra.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2oqedadvt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2dgzrieeq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tjuhsdbg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2auxtscxl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pvkpbomj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2gecaword.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ulznvigw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zyzwqcmx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bnghxnfl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bczunuxq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2krzhmzcf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2sgvmfllx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2msuovtnw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lrupbqsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fifttotj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2aqmhhzlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzkyvujm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jzuxipgg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xnyssemn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ljauvymd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jnlkcnsr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2femnrcrx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2soqwqsyc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ypzxhtqc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qhvyczzi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lszmfybv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kqcgsprv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bfcdlqpq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wfobhzya.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2psysprau.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wwledwyy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fqunksup.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bnghahpp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mqspjwgl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kncgjvxi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ptghpbfr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2sldsvyco.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2cmaeuslr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2spwvwnrc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qxzfxlgg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xusycwsw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2anevoxim.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2icogwbpb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ilayqvdn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pnqnxldu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wolzcbni.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mqpxvmgh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gdbyneid.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xpbtmddf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2sfnrcvsd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qrarkwxe.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2waqqyzsv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xnvbaihv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wzzuvyah.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ixttvvag.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hkpfsmgg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qujgndzh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2randqivz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjamndzw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2czmuywkc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2nicmnvte.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2eligcnpi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bagwyhfl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vvrllize.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ymqucnxo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wwmbofal.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cyzyndwh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2tabnveua.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jvqjvlhg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ctxtzjlr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jnqwelra.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2yjgdkpne.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2sndwzzow.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lpiptczu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uyykvaaz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sqgtrjjo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ytpgfinz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jaddqjzu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2blmsohlo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tszgnatq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xjnrhkzm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2unanaoyh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mgsndldq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uggesxlk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ttsrrbvo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jxsdtprj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tezsquqj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2lmnjwdqb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2diejrzbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smwknxyo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2dcmfmrhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptvegxev.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nvfsiiqu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jmtwdmyl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2otkkdojq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kyjmbdai.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wxxdabtn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bqunjjdm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kjkfnqsx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jvelxgmk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xdoimfcb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vppoevwd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2essbdavj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2iugdfybe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2svdmlitf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2slicthkj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bpbvdryr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sgmyjtso.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ocmxczmj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ypjzrkat.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lzydjdph.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gfxwvgkj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vhvnjkmy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zkeabquc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2owlidzos.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xjfiwwve.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vsguyeff.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2bjcztxei.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jskwlhtb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2rjcbjkog.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2guninjsr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2whglgoet.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2djxrsoby.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gmlaxusj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnjdjomd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2biopceig.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2abpzpozd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zhavhwkf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2pavwkkjd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2taoeaoia.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2koffovak.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvhjgbka.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhzenssb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ugywtfgn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dehhltqu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rkzztubr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2shletybs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bsvfhyux.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2elrgeiyb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2youebajl.html


<!-- 参考信息 -->