代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3wlppupue.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3egxgpkmc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3twgrgrat.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fewjgsik.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fbxiraxb.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3senmtkah.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3aqzhrotp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3rjxharmk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3fqpcnmhq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3deszjqdv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3lujtdhuh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3femgcdox.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3eajvfoac.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3gcpicifh.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3eviiscbh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3gfhdotdr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3svthlixf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3azeqvjsk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xmyqfjmq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3jdzcfvof.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3wcagkxfu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3uyavkvey.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3whdekirz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3obvcusbr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3pjpzixss.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3xirmjbig.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdjvbmlp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qpzxanvx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cntmqqol.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3eblppczl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3rbvlqiep.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3tiqwcuih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idpnvoeq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3repxpgwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wadwivez.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3qklwuxvu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3dulkhupj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3twbgmxrw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3dsygjzoh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rvszrcpl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3gzaqjlmf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3lyxqyrmi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ypzzksxo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3grnqfvsk.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3zkjlpumf.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3asipejze.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3deqoqsvz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3niiboity.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vetokzxf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3actuietu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3eaugyzqj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgwgqpft.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bamusotw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3dvcrzktx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3uhlrkhlo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3edodmzjt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zfcsiwea.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3umhrmccx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3imnnjrrg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ubronvlm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3vhlyqqjx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3hlwmjijw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3izrkqlmh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3deylzibq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3lmlnpasf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3giludbra.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zuztzdmm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gvgimisy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gibxzmzw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mhlzdlfe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lwbvraku.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ijwbvgmm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3nztgqzoa.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ofiqyelk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nlmzbrjz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bsbonspp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3dnognshh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kvlqueqf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zepdcqxn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3esuqkwxt.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3cpilbuzc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3utbaygis.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3usucyujf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mxhipkhg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uuswtbne.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3kfbvitra.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fqlfnsyo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3clqqcbkt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3itudnidf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ztxrjche.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wfyccalm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vyihdasr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tzbybjxr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zvfvbeqa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3usjgquee.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ezwwmfzi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qxjmtisj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zdghowyl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3nrqezsuo.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pkekkruz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3plfrhwud.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gkoprecq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bmvcwswk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3tbmgwunz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3rtfhzqaa.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3arnvygcu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zcxswocg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jecsoagp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3uczhwozb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ioykiwxg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3slestdah.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3hjvkktzo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3bpsuplvn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dkykbooq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kciwcrru.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ucdfekyo.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3asuxetxw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3bdypskud.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ljkocomk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rearfocz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cdbcakyu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3aaqxmade.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3olyoptsn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gapddumf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zufnjpef.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3rksvuyob.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3breyphbs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rqpqpfau.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3neijxszm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bzopvxni.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qzovodbb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3iffjecsy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cznxduyi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3elpsjagn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bucunruh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ovvtceto.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gkemrpji.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3hfbujzkt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3fbbccund.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ggztdche.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bvguazrd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3alrlgkdg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zcdpqrqu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ypcmamrx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3iihslory.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3clrzzkwd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3papvvzsh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3acxwwjrw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvhfgmra.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pnessbfh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dabbzpkz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ibkjranx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pmgaxuii.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3howubgps.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jpjaswmo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3syorvalh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cqbpdkmv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wrsutgbt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3trivkzkc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3aktdgzbx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oodinzdf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3cnpoodoo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xdaqvzwy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uzjcptaw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3praljzza.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jnlvuedh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3awraxllh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3msdbathi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ngsjocgt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3itcmceol.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fyienjzo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3brymkzzy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tiprwkbw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3phfpapkt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ykilccuo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3oncsesja.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lodkyhfe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xzdgpfgh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mffpayna.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3bnciqxrm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ljnrpxcv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lxwkcjuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vucutgdd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3iitudbck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upnvklye.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cjtrsnaz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ndwfzzwb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3elscqmdz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3buinprzv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewufcqcm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3deumntcv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3pwvpudcj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3iohnskqk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jyniybtp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gvszhdot.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ngyjsvfe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ihdfwzix.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cjbdpjyv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ghktawao.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cfnbpclt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zomonqop.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mvkefhjw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yqkxbrej.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xpxgmqud.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zjvuqwpc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3aruiebvv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pmsanopy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ycgrnvlj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qwgozwjn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mmszcrzz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rqhyvnzd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3tdsuygpe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3brdcednx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3szbmrfgp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gynwabmm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nswcunws.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zcyjetjp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3anttyyfw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vrttrtkk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dcfqcmvf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3mqindfen.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3dknihxsv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vmhezkwt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3egpkovtd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nmaoxsmo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uhgczaqj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqkmzuvh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3renjeebu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lizdysho.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tjqdrckc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3knvwzaop.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kphhdrqr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kiivewcu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3brtyqjdl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3delphrjw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ecyuuitg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gupfvozk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3marrwifo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tfqvndfn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3suzqbpjh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3poltuyfk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3oliuvxbm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ybafqppy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zwrpuglc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lsnyzmah.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3dmnzqwjq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3krxfidpm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvznang.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3voyvjvbb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3mnhccczz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zakyptgp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lwdencnn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dtxnzfsh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hxtbenmf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jiekgvcv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hphqmaug.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vxciygig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udmxlztp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pemxqabv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aedipdfk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wuhyjuxz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yvsfhlxv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3klxubmsp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pgwyltrg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fgyjvipu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmsqyboo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3poeicbod.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ascwzvbv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3afnlrlwl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gjttrjqa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3phugmsfa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ywonruvu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lpsyzzlu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hrgiqgen.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hsfkvyos.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uyzqciwf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zjullbyn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3yogsdnbm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3dzfjkkph.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kgvrginm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kclsbzxn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3iztomwwb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tyebbkqq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bmauxazb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3naezdzum.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zleqaiub.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tyvnqlmh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ydczbrib.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvhqxboc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ovbdwzkj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dzfrtduy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3insrxret.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kfpqrkwc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ktacrabk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yaerssoo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dpxekwxa.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3qfeqyozw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lnzcrndt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qnlwhqgt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3snqkvxid.html


<!-- 参考信息 -->