代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zxantxno.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3wiiicabq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3wnphxaaw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3uqjmlgur.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3jdgxcvnc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3fjbistur.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3tauodofv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3fpenuqbf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3fflkiehl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3mghptpsz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3eoghdeje.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3nygmonfw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3xxyqxtna.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3vvixyjtm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3emsdnred.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3rssbpnrb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3zqczyzpb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3rkscmqia.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3khglamsn.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3vbxhffpo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3imockdki.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3fchhunim.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3bcslopfc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cxsqrnbk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3rtyegffd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3gxgrmxmc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ovuukugi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kxwwkaue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oplxsskc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3fjxjhist.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nelewyld.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hfktnbch.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3colletpc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qdotqzgr.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3bzyhtvms.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ertkbcmi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3uwnlvuli.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3nmzoblrm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3zmypmixw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3twlbefwf.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3hwdtrupk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vydneohx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3kfxbngmy.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lwmjnsbs.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mhydmhtl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uambakrw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xkfbobfp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ekmyyqel.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xmmoavpo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3vrylsozf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vpqloggc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mezsblmj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3khodykqn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpvltxaa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3qwrjjawt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3bnnbcrqx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3dscdjhmb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3vjcdmtxy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3wndpwgnn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vleahhag.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3mrjuxcgw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3lryuwvtp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nqilnxwb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xicnojnx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jpfkumtn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3uzcsubex.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ngniqoej.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3qobntlvj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3rvitxhhg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3yqfoefcx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lgfqxbhp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3smyqrexk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3xntblypq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3gfljkulh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dxumvmrf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3qiqrdkwu.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3vfrlnppi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3otwkbcqr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3tpvmbvcr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ufommzgk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3siuayfhw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3kabsityk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ikxyfkxw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rcpussge.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cxkmlpzv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ualkwaei.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vfwmdbhl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3xzskxwhg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kqdlxrni.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bnpclzrl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ookqamfc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kuegptcl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nkcvqioc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sbengmgl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3nupmvthb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rlzkyyhn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iyplrkvz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gswmyvib.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zkqamibj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3jsywjfdx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3vtezwiyb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nomnuami.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3soxhgmmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkkcztjv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3sbdrkmwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sshphgsf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3nyaflone.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3tvpbyxtw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3skoqwvwy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vxmfvfxg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dmuwmyii.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3xpvkxmqp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3yukdncqd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3bdigtxzt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3dgjbpyyr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tdkulnty.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ytmxcvos.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3mfcsyggp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jqgmembe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mjbrtwtx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nsyhlhjm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ksjvnees.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3nkzpmiki.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xxliddnv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3gkpndxnv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jjkyvibg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qvcettbn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3oifyybmm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qvnbtbfr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3pzmpqtii.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ednsjboe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dqtorfjq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jvobibgi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3zegngyol.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3glvblyfe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zzaergzi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fzzzngtg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gccaedwu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ofyakakd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3oppxsomp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3aopdboti.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3swqvysey.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3yusaazyt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ptqvoznh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3lxrfhbkg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3koxfaeur.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ppfvafix.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ggxashnd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3qegypiya.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3lggnseam.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ctvemnlf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3fqewosog.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cvelzdci.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3anmzhvtj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3woulhsmq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qxpdneoa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ehvdovim.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kfaddebm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3nawixaui.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3srejgdrl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wcdzwtpx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3eunyogbo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vytmbnbt.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fglusdek.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gpuycfjb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3kofmjkyh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jwekfleo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vxcykgml.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ngrbsocw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wpklfemg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3gndhgpmt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ofwsfqvr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sbzaqrtv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vbxgycsq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wlxxzabf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3cobddqmr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3twviputl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qpmpitlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykjthcun.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xqdwaehn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isqfxiov.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rqltmfoq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dnvojkjd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jwnkyrcv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fgjcnprj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3iruzhwua.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gjcgmqys.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3azubdgvg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cptbfpxz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xepymtiq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3etuqhujg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eenfjfsg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3navjmsud.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3suottgqj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lgqzklxx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hkbdgjas.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rnszbwzs.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fnzfqadu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kbttdgxq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3twzxyzhd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3angrmzzn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3kzeispjz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gebetkna.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ywiixnve.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pztsrmkb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3dqufoshf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rpodsmyr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ipauidcy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3pnzmebda.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ggrnojqw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ypyacxsa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xpzsferc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3trjtcody.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xpdvnhuv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fannkito.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tzxvszeq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3sxxgjqlh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ichmosva.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3glngkxvt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qhhlvmbj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ibbdfikv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcnvqvlw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdqsrlrt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blnwwtbg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhgtuiix.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3lxqkawsh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3cugnmtzs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rntpkjhd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cwjxfemn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rttwldqg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pdkgyakv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3davxvzwa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ncugxfad.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kgrhybot.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uhrsxhsb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dfsiyhyx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vivoeqqw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3izglvjww.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gpsgwjtf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3aqrdcmaj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ujvnaucc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nmnqeezb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3yfsmahkm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xarcgruy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3cmeajsoo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3puqlwhlm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3epojizwe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bhopdrly.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3exmmykjt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3iuxmnirg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3skknyiiu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zjpkkzmr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3aasjhcxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyxytxon.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3emjbohmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukryihwv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lyysakrg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pqlyrkgj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jzofhepk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3efuyyopa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hkixaari.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qifhdafr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbhkhuyc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3fnjwksec.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3usbimrgo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rkmvdixw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oecculfi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ftiqxifz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rakiancv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjzxvho.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qgbjznkx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kbmnvbdx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nexneqkv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gzncjgzi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ovxgpbml.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mjmjtypw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3mmifntjk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3smqvvqpk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ewbkxwxw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rdavagpt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3samlvenw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rgytlirx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3pdjvmzpo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3pzvdyrrm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mosgnmwv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qshhlbsx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rupykrgq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cbwcgzbq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yuvjyrqn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3oicdctwu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3udqhhflj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3odgvocnq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nqbtfpkt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3oqmvmgye.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3nctidvde.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vtcsnloo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyhuhhli.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3sonnozdb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zaocepbl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bnkgcixm.html


<!-- 参考信息 -->