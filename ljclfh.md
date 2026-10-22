代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2jcopetfz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bgqtvtzk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ihrxddca.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2fcxoxzuq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2slwddtuk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2udabmbvm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2zeakowzb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qrsjpybv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ebzksake.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2rhbmafkk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2irvtqpnr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ctoupxtb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2jkowcudy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2efyvqbzd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2nqyeguxq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2oybhcybs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2jflvyktj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2tbxvhopq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ougjrwor.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2padbiqau.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2bqmvxydp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2lmghsyag.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mgozjomd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2iflesaga.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2kqhhowpc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2xfokwdya.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ziepuqoe.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2zliistwk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2qigcnwpn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2xvozdjsc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmkydahf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lkxfoffg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2xrlxdsze.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2mppsamtz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2qidardec.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iunsfsee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fserkgkf.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dfsclsax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsewgvsd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mazidihz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2spzubtqb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2gabpuwgj.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kszuypyb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wylgbjli.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2xkhwtjmj.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2izuvwpgj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2liimiksq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2urbmdgpa.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2wawjbkwz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2gxiqtnyn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2dfyhxukt.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zuistrrw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fldypsmm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dtzgacxj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ptdkapxp.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2inrrrspr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ihezaixr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2vyqtoxgi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvngsgn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uwddctfn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2nneldrcl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vojmlwux.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ohxzdofz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2kfilfgyy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ucbzalxe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2opophcjf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2unkucojz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2imkvzebn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2yxtpruhp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hpqreegv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ysuzkiiy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2abvsnivh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2fvstowjf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2almawrqy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwkdurhx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2njbcfrgq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2rciqmuch.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2kemllmbm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lbcefcsm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qwjlutig.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ntjssnhg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2eqoezvci.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2hfaykszo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2egnvpiet.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vetxwtgj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2slejghod.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zlrjcmoc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2susobvlf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rqloiwgm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2vlgratyj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aiofuyhg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mnzahmgn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aoyzvime.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2midhuvka.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2djmanfdk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hcwvrmhe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2okwyjexu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kmbghzrq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yavkiekm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xmmyokul.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pcbyrnki.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hkaxkqyc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2quvjoacl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xqvtezoa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kiwoqgmx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2iembivjq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2abikedpv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2yebmvjdo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2wqrcoksq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fibsyabk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fmokxkjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imkjdqua.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2gnpmbmuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdfeylhm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wyfjvcxu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2hfpjdtia.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wyqgcrar.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2iibraixs.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2legnzfuf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2eebytipc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zhdagvvq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xyyeyqgo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vmbamzxc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2payzcfzr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bbomvakq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xddedczr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2kvfarehd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2axgtyhjn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jouwgrct.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xwdugodw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2frqzdvdx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bspyegmm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2frtecddy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gacbjlht.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2byneurfi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vqzisdql.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uwdcatga.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2djefrmgn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ipinlrjx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2dkmkljur.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qiorjofc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tfiurrsn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2nyqezejx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zvhhmnlg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gjfaybrx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jnhnndab.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kckigxvq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jflfanci.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2csxtsbyu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qqigurqn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2iyamwxlz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tqldfsqn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xcpqooax.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fxykpbyf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jbwcdnni.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2panpwlvb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2svhnuuog.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mvhfplzj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xnoayxfz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yletvenw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tkvvpfpt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2uvdjbeno.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cthwhcja.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hlrzgfug.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gregwatu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vqjxtdfc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2stmmqvbx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ogrrvfos.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dtypgjsi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cwylwwsn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lqbixkge.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2atlsrpps.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2aredtvtr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wmyemgkf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cpjxdzhi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2cncnhail.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xxkihmpq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nbcephly.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2evisgutv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wuzenjbw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2taokouji.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tmvgokwr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2dkfdztaf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mjwdwbae.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2iuhwkivn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gdqwloky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oomgfpcf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2tlhdclfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcidbkiy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2iknlsesz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2nefuvmcm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kbwialdf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pimgpwww.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wugggprh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dazokoha.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2foxuxbzf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2cbkrlnip.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2iidasgne.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2btqredvx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lwzgjtut.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kijtmuyi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2htkswfut.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2eqxqirbs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2asktnjti.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ikzebdpt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2syfcwsqi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ddlzhpsh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2cvvtklzx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2wceywcrz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2auuprymw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qjixlmpe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tevswtkn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vukapbnq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nqnlkphe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2aobkwzqf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zwdtbzln.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ifmbqcyu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2sncbzvsb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zcizbafm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lfoullag.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2geqjfeqe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2tyrsghcx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tiamnryx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vqtpvgca.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2esnadrzs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2iitairbb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2goytnerd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vvqgfobk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cpdpvygv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sgkynzzo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cefycltg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2licruzhf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jsgpkbck.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2imcgggsq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2urdqhfbt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fmyffhrb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ngufhvdr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ztnaprwv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xmlampay.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jycigwfg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2bnseccnk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2wjpexxyq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iepthvar.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2nxgkcikt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wnkigocg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tpvioadn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qykycwbk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qiexvwar.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ybhotxtj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nhrvvcgw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qzficsnc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uevknnei.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jicwtzmz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2gwoukqat.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2lcdqlpxt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2avkqmefn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bnnvudvw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vhcaxlnm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wnumydlg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2iuhloify.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ottyxbws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yiihwzhe.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2vcdhhjmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zaxcbtef.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2otldzidn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2emzicqme.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gkwkctsh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2legyszae.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yszqgzsh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2npjknekw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sqwctxdx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2edflpddx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tctvojsn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2lrtgxbxe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2eqfpihrr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2dbtjtzsf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hdrgppwi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rqqvynki.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fwtsxjme.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gzkuvnfv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zyimjaru.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fvvryolp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2nurfkgcb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2lposdste.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2upykesnq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zfuoemnv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cxqapukv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fqixkqkn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2cnohmtey.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kkpaknrr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zzigplnq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2pkxqyssc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2abycfdnd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzgccynz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pehzlngj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qdgieeyl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2oloicchh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2facomtzz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rjrqzrsw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jihtiync.html


<!-- 参考信息 -->