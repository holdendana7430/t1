代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2vguppisg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2iittfuqh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2lmvaxqyo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2rnqrtnoo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2hoseriqk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2gfsdwees.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2tvqzvcve.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ohtpyovt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2olkprrrw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2pmyiiick.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jpciguds.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2keckpqiu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2blxubcnt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2ilwcdpoj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2yegymewo.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2vegjotfw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2ecsewvxb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2oflqhsnq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2yzgwated.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2udwwbute.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jznfmpow.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2rhsucnjo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2vtpfkbpt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2khtoezgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkfbuzds.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dzilgaqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkoxmdqy.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pqyoguei.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ejueiejm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2szfooxlf.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zcsjublk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qpghrfwo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2wqtxesul.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dioxgsae.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2bzqndwrz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2lcvoqxhp.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2xludyuzp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2pjxsxddj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2cpzberig.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlluyzwl.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2thijmzdx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yuntmszo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2zqbnulvb.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmgiwcvt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ntaajkuo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2jpollxmi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cwkkglwc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tblxsgfm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfiiqand.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2tybalmtg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qgvmfmzw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2wsamjcyi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ydiyizer.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2minefsds.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2kjqvvwnw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gkwdfxkq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2rfjxytqd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zrqncblr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dgeiffih.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jeffzvxw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jydtprjv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yrlpnudl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zcgzrqpc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2gvdilsnw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2heibqlqo.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2xdykvxnj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dlkmrlwh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zqtkxqbc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2edbdicre.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2jlizwxce.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2uppbmsuy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2rmwkmpwc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ljgtxqqe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2trlaxjgn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2obrfzyvi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dkfkbroc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wfwxjsyx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mpksqsas.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ltieunns.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bdpsbspr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lraumimg.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yvudiliv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jjidfeox.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2iniwfidj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mrtxqdwb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kbwruhnu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2myhidcll.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kxrqiunz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2iliguahz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xytgubui.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2usrsmgcq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pdjtxsfn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dzxrbhko.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cjytmssi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rdjividb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2bxqxxqub.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yxcyqiob.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2snbyznji.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2duxuqggi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnhzbcyf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2chabwxyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmjjgyzn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2pcgruxhb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2gdhplffg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mmdesgpv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ujxjoioz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2owrzmpvi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yxqlogpr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2bbrdymdi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2epfflqqv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gwgnbrek.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qnqmbqzj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jxxypwdh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2czxfwbmn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2woetrdtr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2aigpfvsv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rhqyxwpl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xoeupphf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fnlmxxdf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qcaqodbt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xnewrrvz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2gkjtydrv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dercknhx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2sxsqgpnl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vvfrmpoy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2sgyjlyqr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2uoibadqt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2eikhgggm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2yywgarno.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2peaxkxvo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2fxybxhpn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2qiktsocr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mqopjpyw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kleydsec.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hsyfirbf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2rvxmcsqg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vkzpklju.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nvisfurm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2fqeqqzai.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2euvhrqzy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2iozqvngk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ecgoiagz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zqgpimcw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2wdjepfvy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2fblfpluf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2qgkxowgo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ycxzsazy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kwmleoau.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pzmgmwsn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tvvjrqlf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uufxncua.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hhddates.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2skabqirl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zuvbrvpz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zcmhowko.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2edbztlky.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ecyhmubf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jzyfkujm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vbsttrtp.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vvhcbina.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2statruss.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ibmgrwln.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wqbozsio.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2sgmijtjn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rrtlqobd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kxyqxtsf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2smghpybw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2minnihum.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bohhpkoj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mhmdqync.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mdslphve.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2yfdretyh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dpfsllcl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2colfhjhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwyeiubs.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gmfcvofh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cojuyspi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wzcelpir.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2yqwufvno.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qcjwztuy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2housrmdr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oovtfdmw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2issinnds.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2usrzoahn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xumrmssa.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mgexnvlm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2firagugp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wnyhfzpm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ljajfyod.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fmmfjgyk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xfbytoum.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ezkzmhrl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ffztvrit.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2spxiddqa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2murhouub.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qjhlzfbn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2uygbikaf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gaqeqerf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ntqnpicz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vtpjtxyj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vwvhsjbj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2tipceemx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2eszlispr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bhqepxpo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gnjzhuzy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kgbeised.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xeueevyk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jqzohguy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2biacyycf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2newmfavp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kknibttc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2kqnmptvg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tkzizyus.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2srlgqvou.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tpjmbavf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ctmyxsga.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2brwrgbvj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jrlxrgab.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2najiqtot.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfrvijzi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2liodzbqj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2clbwazzp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vfclsvjs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jlzuifza.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2diurtpfb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2trbjoork.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2anwjvkgf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ognjujkk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2sntbavyu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2glevfbrt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tqbhkkhd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2wjhgsicm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pajzqjxp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2euzdrrtn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2czyxvndf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ntmgjzbe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rwygpkzi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2sfevlbyn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2cellnmah.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zdceuhtu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qqdytcdc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ymebdzwj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hsavxuoe.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sgmvexbk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2brpsryhp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sbxoexqs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2lseddwzu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2egwomdie.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2okgmgknr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oemkmuee.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mqvfkojo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzaptgtx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gisdwqud.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ljsxraft.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xhobyjio.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2biyafkqd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zxumekiy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kjsyrxde.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2udcgcpta.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ehuatcib.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxlhoqil.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2gdusojam.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mlfiotnl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2lduwbnvi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2roaystnh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2azlbklpe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jtuslgoc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tflqnpwt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2aftirlsl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xrgjctrw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jnjcdaun.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2trzdrlnx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2lvrubpym.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yvfdksfb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2shuxfyos.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pkvsxipm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jzxwalad.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qtfkrksp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qehibatn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2iaxrqxvm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hfdayrjt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2squjlgvn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2atwrdnqo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pdqmqell.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jnwahvdn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2dndujfgn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rxfthspn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zqgqzyhv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2rnbomimw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jlixvenl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2alxcxqgh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uujdatek.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vexcrnci.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bhzjpwgg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2tiztfzvi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qgveufhc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2upeyjpwj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ipqceouq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qgpuexet.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mlljsbkk.html


<!-- 参考信息 -->