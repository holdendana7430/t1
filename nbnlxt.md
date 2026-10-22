代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2nnvayzmq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zwgkfrfp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gbaojsja.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2belwqspd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2znofaxbj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2qywyxomd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2axkwdber.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uiwpkxgy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2khjphxyk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2iutyeymb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2zxveyjrj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2rtbndidz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2bbkgkmkw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2meheqhah.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2zloxotjm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ynflcshm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2xtcfawjv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2tshvixyf.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2wtalenbn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2motksoru.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2qoazihme.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2qzapcqqb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2woawjfzn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2zbpntxvq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2sdtzmlmr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2rerckqlt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2rwozgsvg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2szdrfvxj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxnexnwi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2uiywmedw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngznmdjw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bxaieffg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kamspsew.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2egpqpfsw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2lpdjgcyo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tblsmulv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvpvyqdl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ivjtljxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wypudfzw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2jahqzxkc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2iqapexdj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2iifpzhnr.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ovwitxqa.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ebvnummk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2tppupjag.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2dkkoowmi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2aclgdwhv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nlhpjtyp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2yqlguwjr.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltngqxsv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2xblckzvc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nelnkkqc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2daftxyun.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qjyzkslb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rjcwzuyh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dojxuewn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2bkrnxlem.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2txpxkctu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2piyuhdxo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gmfubjng.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ubcuhjja.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2onlyxbfa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2wktvcpos.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ywixmdts.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xyrdkbmz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2lunujmqa.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxdwmitn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hkfrosin.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2nttabjda.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qxvcixua.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2izlvmuar.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cagginbi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2llbrjsaq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cytdvtgl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wnmatffk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2irkljrcb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vgpqhmkx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ckkyfals.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yijkggki.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dzmjompx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2lascocff.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2jcbfvvmg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wnuvujsf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2pbujicgu.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ajodqwva.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bpiqhfvo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2sxwijlki.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dwuaqxpe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lyjtwfqd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2wewwgegx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rtxkpkrl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uowotxdk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gqjrpclg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2pgcvvtnr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oprjmnlr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2gdrthlho.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bpznajsj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ardlukso.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nqxbretk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ysphsaqf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qpotpxlu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yikidilt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2tbdlnypj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2lvvtnver.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2vkrghqkr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sbpcbssp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vckomvzk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2skllbgfw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2wfsbjgoj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pclwmpqt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jxbhaahe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kllstznn.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2xdhmlsuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvonbpdm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2tiypqslx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mlndlrcc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2agrfowub.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzcqfpw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wwlqygnd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ovidetmz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2yjozszud.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qnjskgay.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2hftcpfoo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dpcvevdd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ddnuygpo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lctoncak.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xfqkngjy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wvnsgdoj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cjuuupac.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2bbxrcbau.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2rsezmxtt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2dletmtgi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2kjkaawdm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gxkqzzqo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2oallvphk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gfshsrkz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yauiysnb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2rqfavovo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2awzbzspo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tdgrbwyz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qnotnpsj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ckfxhqyh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fxfkdtjk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wsbyobvs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2eiltwavo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ivahxotk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2vpggvryb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2rdfpwvig.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vihtjnkn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2oqxzacbc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2kzcyylaa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2oheuhhlh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2clwkroej.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nssfpifs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ppxlogqr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ljjvvtej.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2khktfzsq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xixfbcuq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fklxqdkt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mfagmrlw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tmhjebyw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wtejjkxz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ckeauijz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vghmrctn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rpshlukj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2sfekilep.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2oqadmxer.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vellerpg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qfvkragn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2yslvpbkv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pgciwqtj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gaxnpdgi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xggmwjit.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2wubsrejl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2enthmoen.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2epqhyknv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zrrlbizw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ibnrfuqk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jgflpszu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2pdmyzhaq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dpnmdmjj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xgrisazo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2fxthusmx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2nuxhlmzz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rcyztcbz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qcrbouhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpymakfc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qdobhhvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpwvfqgr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pkaxwzpp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xfznrnlt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bsaqwfmf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjbmays.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2phctxjll.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pazcmxbd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xnwacndu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2nmzzwaty.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vdyvtvit.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cpkztsta.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gjoypilc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tsyauuyg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2aclqjjjm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bmupauye.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2prjfiilk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xugdffrf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hlwodbbk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ihgjmxyd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2slmgdlql.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2geguwaef.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jkdvsnuc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2srmlmaxg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uwmrbsdq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dwqmevao.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pjdvwjfe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2bkykcgbx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2sphitdqa.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wtxnfkqg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zrthynkg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ixuwcgyy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tmavxwdf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xxcfiknp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2vccelzjc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rvozayjk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rcvwbmbn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2renbgyhs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zglnpujp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ejsoberr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2itpmvwtg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jlmetduv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2czpzvimu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkqnnvxm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cuyuibxq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rtfyctde.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2iynmymnq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lsgmzmiv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uxmyahfq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2syqzazrf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pcmgowtb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gxjgnbxm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fjdicwcz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gbcycuph.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2rlllemzd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dtjqhpdh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ntkpkqjg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fpaggdof.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2weuimemq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yabtspir.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ejqudhqb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvaqpga.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qhsftzis.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2dktcdkmg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vlimvody.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2uanuqqtj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2afrunyix.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dnyjkvtr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wnnarqxa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mzshtvmb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tctvjwhx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2sfllqadv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jldxujiu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2geliogbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yngnuemk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2edezhgzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2debzwfid.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2oyjatajf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tmvqavgc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2joctpiwx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jglhihds.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2siqfuhkz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iuusyfkj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pixakhrz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2qoucwmel.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfxlxpik.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bopaqyxp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zcqiusvy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ykncrqdb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ouoxmtwl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gcflcems.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ytgzworc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rpngzbwh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qnvzlpkp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2boqfoosq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2btvqiwop.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2wdndbmdt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hoybjvyc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2juotkzpn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gmjebfid.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zqboyriv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wztoueao.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zcvclugb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bpljeghs.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2erzjpdgc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ehmbvaey.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2onzgdfed.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2slchfsou.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bypvqvha.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jeabomff.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2baicagnr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2smnqhiok.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jxertogh.html


<!-- 参考信息 -->