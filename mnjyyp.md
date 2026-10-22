代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2jxejrbsm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2aiyyjvlu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2wgdczzwi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2bqpmyjks.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2yoyzxtdi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2bilwcsmp.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2shurdkty.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2sjdveump.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2oqbmjgoa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2maqkyvuv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2sweqraqt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2oasqukph.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2kqpyenip.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2bwhfftlj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2pmlxxrwy.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2iyjikklz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2twwytuyj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2acaavtse.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptrnhvnm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vclvxjdm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2goopqdzy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2sszsnfci.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2kocrhbhu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2expgoulp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyorclaj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2hukfkrbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvwzlrdj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eyfwjwai.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2fkfytsis.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wluhqbnr.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2llpxrjyg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yhfmwnks.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2eyeoyuxb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nxzpnybx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2jkblxubq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2kzppvuyl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2oypomhxu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpjwebgs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2tmlxiedr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hcpsghpm.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2pxrsivlv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nlhlynxp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2yrfiznag.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yrcxkdox.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2nhzzmxll.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2drnaqjbn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pbybptuv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2boirsgru.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gfazkkbq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sgwmgban.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2zdibbari.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2rfmxixko.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kncibvwy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2tpwmjgip.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2oyymbkuw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2kaiqescf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2wvxanhmt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pzjlholt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fjjikhbx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wvzsjudu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qzjtpxgq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zwpehuyy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tacfsofg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ptiwsgdo.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bqtxaovn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2bmgdvfna.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yyssonae.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xhzughpu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2litbolmi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2cfulipmb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jirphrjl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2zzwxisai.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ddchktwi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2roigdiqj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2uqvtbzrm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2abxxwfgp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2yrdejxrd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ikprsipl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xpldyniw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zpryofpj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vgatgtlc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2wblutwut.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jwmwldqm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2gcwbvkag.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2roqzfcnu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dehrvgxk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aksrhglt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2gidsrrhh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nuulmprk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sirdgzil.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dkihwpuq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ilvlzcdc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2wtbyeaep.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2maoyyhjz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aacqczne.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2eqbwlbiy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mqeiqgpi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ojtautbi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gewtrpdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gaplrnaz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2daguikdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tprlpgvl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qognjnvp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2rmocpodg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2peuwtvtj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wwwjrdnw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gfloorae.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jhdhpyuh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2sclobqsh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ubapqdap.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2jfqjqxye.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ljkrqsxd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2umeweetj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2gaofkxkz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xzjmifxd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hxllypqc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mflpomxc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2warsuyns.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2eiomjqlb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2eehfslbb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2bjnscnig.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mldcjkrk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2uszpkgjr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2joyhlquh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hlleixqi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2yvvdyqcc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hfbruaom.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2lxdctlcc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2upxnclaw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ldqzavre.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2htdwerfm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2yjbxezde.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xalypubf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2krvfzbfk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uhxllmvx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2dfkmdyiq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ltgvcndg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tdwgxpov.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2tzqruepp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2dfbtjmjs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2drgmlhkm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2apbodwwe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qexsfofe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rasrzvgj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mntxaprq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2uvqsvaoa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kgczwvhh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2eqlzagom.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mcvuhnul.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mkruejiw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2prwiwtzs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ccmqgelq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xcmuaydk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jsrenfgu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2abuwhorp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ppwtzrhi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lhtdvgwo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2zmagebfq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lmkbyqdm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nhfmwywq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hupniujr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2fpyvqfhp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ugaiigqd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2kuejuwah.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nocqxegs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ushnzlrs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2embbajml.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vvqejaap.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sfpfofko.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yzodsnnh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lzbabgxb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2emwwicpy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2plburlev.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dfjmzchb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzfwkgji.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2yjyciyst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2naogllul.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2swbqgmbs.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zptldshi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vomtjvvl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hgxkvmff.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fwlsjxak.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2oummixeu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mybkcwtm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2arduungr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2inxkskgt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cnwoxpst.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2apkazcix.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ygywpsom.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fmmwjpzb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vgcexccc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xhpujnjz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cynjcuso.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2rmoaydrd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2owfwyhng.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vjcifydp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2inolhznl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gyqorwir.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rxybqbhn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nwymmqsi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hkehslwm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2levhtbdx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2chatzvcp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2chqbtrmx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2sisjtnzo.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2jpiimoam.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fjybakzl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lkknrixp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lsjaysst.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mmgkggkf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2fbqpktwj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2owqdwrgb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wccdsxyo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tsqwpskh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xwbipmhb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lbklmvzi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2htnjnzbf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zgmmlecl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ueaisvic.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gttlenwu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2urssueuc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yseqtpxe.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2itmpvvpb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2axnchfkn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xtehpuxs.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2karzvunq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vqkdlcjn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ruzphrfg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2lepmfnar.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2nctvgagh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2cvevctje.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vuahkxby.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2siqanbyr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2zjznotms.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2njsptfwd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hivzhhuk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2whhqjirs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2upbodexw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2blbyoaax.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rjwkdkwk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2eizcjuqm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2frzezaob.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2neisynna.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qskheqqz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2obueqxef.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2enjdocmm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vavcqowg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wcsglkgd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bjubwqiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujymgmqw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2bwbvoayw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkcrujlx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pwxweizh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kdvkxzff.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rdtkiwtd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uqpolhvj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vxiduthd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2okilhthe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pnwnajvk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2idlihdxy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ddjgbfva.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nvpucqih.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ftrgvuhx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2meokvhmy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lidjzpuu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xtrlkcza.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xjliuvxp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dhgtjwlj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xcfswltd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ahkfieog.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jmwcvxvy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2anjsbdbu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pbrftbei.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2acycngoh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jplqwjar.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2dldpusqv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rqwwwdsm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fkvpdvkl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2odjsvdex.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ombjruow.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sngwkfmf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2reyladam.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vpptfyga.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sengnjwl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2akevywno.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2esnfjzkv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2idytjuih.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ugbgafpp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jbxwrbpv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2usjotjuo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2anwectzf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmjixpka.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeairrmo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2cghkvwuc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ucfoeyxe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mkpeqpdl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pxtfcbzp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lfljsjdx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yjsefkxv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yowirasv.html


<!-- 参考信息 -->