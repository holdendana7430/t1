代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wpvvvshb.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3hqniaopa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3rihyutmy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ytoonyts.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3dglvmarm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3aslujypn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3hyuhfhpq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3bthjxmrj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3fdsjdyfy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3zdetmamv.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3vmmsrpzn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3vqqkhgez.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3hamtwmog.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ecqjvvvv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3osuchiku.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3morkzwid.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ctoetrtt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3xshexzgt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3inwdvwdq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3fxvpwiac.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3wndqgmwt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3tmqfrcog.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ylqzcesm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yoojlocc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3edwkbvns.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3hzpcqegv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3hmhzrkly.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3oopycsar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwohehky.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3uhnzehdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twqmixav.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvehfnse.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pbyzrzzw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vmwbxwly.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tlwwjmrc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vntcdtdt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3caqagcgz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3dncrvhsd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3vhlaftnv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wrxyquzj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3krkzugwv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3nyyxhjvx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3vxwkmsis.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3henclbio.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cumcozlv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lpntykuc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ktfboszm.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijfocrke.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3btcyzysm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3qawyeoct.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fqklrysr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wqxmizqy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ximyfluc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qgglbwtt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3incopjde.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ieklkhjd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3azcabxmf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3gbkskofr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3akkkalvi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3unhwlpiw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3wmeioycy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lzvzylug.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3epwupjlm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fmfvtqwr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3mdzuqusj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ddsudsvt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xdlabemx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3buwrnxpw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cwcblwjf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3sknflhag.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uuikpuwq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nabewbvv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zmlfgcgd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3jukpjbac.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3eedzsczc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3svypfpsj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3tmyeyklo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jaoilyzl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ffwyiopp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3exdnhiwq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nwiekkps.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mechpusm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dwsdwnqn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bmiidhea.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3oxjezssm.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3junfsbhy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xmxnxpfb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mismvmqk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lyittoxq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xeefhmur.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iycfbcxv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3lavsisrk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3arprrbje.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kngfgrtj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3xsrmiuia.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3iivmedil.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bfnpwffb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bwhqvhnp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nkxfqrtv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3htwwyyoq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3lqtguyqy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ezprtylf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3oeookhxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uxfytqkw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3aslvsfxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yesumgsy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3nlaupmdd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vjdxycib.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3vcukbxoa.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ghihigmd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dhylfuhk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3qkmffvte.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3amsrvtid.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gsfpnwby.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gaolrtds.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mkmiobws.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3aesnbevl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3nujvqrkl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3stqyjlfv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3izqjycns.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3drimorlu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ycopngju.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xssttzxj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ratfihow.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3kyiaeziu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3abcucnye.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3jhmsscsy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3womletwh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bqixespd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rrnogmzj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yywtbqfd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3mcdmhqde.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ikdjhjpx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3iiynowsn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3picgyayb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xjdqraig.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bqmztmpa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fhjsfanb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ixdazemv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fgemuiva.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3sqqnoucw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mxluzwog.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3obshdodt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3aurxreed.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vxlgstji.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3uvvocgms.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bvoxiaru.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3izdicdih.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbjbzwhc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3mjbhsdqd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ywsfjgwq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3smyrhekr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fclfhscn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ixxiumzx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rumqjqfo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ckxhpgxy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3duocsyhv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wjndgxqr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3uurmfcca.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jybywrar.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ceaxovou.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3cgcqbzty.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wssxegax.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ocgyawzt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nrhsqvrg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jxbrnalc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qmvffhzg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nhgjeftw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3yhlvzodt.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ouujmfxa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jazsomte.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3gmrwsmyu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lxkdioxj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3czpzgxfj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3vwyzinns.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nhispeao.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yqsxyitt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ijmkimzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvfeunjc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bcvyklfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bygkexxh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3evfjmqtf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mutegrku.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tqridyaf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ikcylgwn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tfmdtpoq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gucoqeek.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jolzlebh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zycnkyrh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yofmeqnj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pumpjmft.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vjzfoskd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vasklpnb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bonxreft.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pnekllln.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ccosszce.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dlsfojyt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hdqodxdx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pgrxxnuk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qbdffcqe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ewvefzqm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lkjxeqjd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ogixoyrk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3edyeocqh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xgdevyye.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rkkotpmd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lvyjimmm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3meklaucx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3utgyobfi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mljczrjf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qncowmsb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3avsvaspu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mboybfuf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dhtxxwqc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zygppybu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jbtgtkgd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3gshrsrlb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mivvectg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3axajotsx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3gacamkuh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mjywyzqp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uqpyaaxh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgesntas.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mzmtdaeo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ptdrvivf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wnrpnoij.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mtfxgtxh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pczgtgmg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yzmhsyre.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tvuepqny.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nwcpqqah.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3aykjwfrw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3uzwzblih.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3zzzfonvn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3exilkwgv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3znpiwqiq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vbstekzy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gcdqfpsa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mdyojxxw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bwvhpvzw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wghrpqud.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lzzvuipk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ddmogcqz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pxlfxjli.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3opxtjscy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lwcnkwnb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ofxussww.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gbdjzflw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3blysavum.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3dwjzdprr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zywmdjgf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jnxujotj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fujbdyrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulxbapsv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kbosuggl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glddqere.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jzactsbl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fgjyvkqe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xsltozuh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kvwfydmv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ktxgmpev.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3toegbzkw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qoaazace.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3bukcllfp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kwsxlgqo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3jnvbanic.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bcpgdytm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mvudfwqm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uuvmlgfn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cewsxpux.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zwvwwppj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mwjoowyi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zgcwclyp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3evvtrkks.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3hsqxbqgf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3cubmrmgp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jmsttkmb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xynorwas.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fcrmbgxt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ujsqrhca.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ocgasyfu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3thwuzyvg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jsblokok.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xpytlgmc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3diruttuz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dxnsmdoz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cfxtnpwo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nfqbmuux.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwlfkhvp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3glgnqzpx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xzgwfsvr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yltlmnse.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3dynhbgog.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lmiezzfg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ukjwezwa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkwtyesf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hudkfesg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3afulpcvu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3bkmnyqss.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ghxmuccl.html


<!-- 参考信息 -->