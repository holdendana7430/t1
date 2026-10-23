代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3yrbfzpqi.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3rjtxobro.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3jcvyxhvb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3uocafblh.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ypejikdg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3fhnjzali.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3scvmxyqj.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ukbkvdao.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3wptlwflu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qtbrilvf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3lqmrkadn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3rilpmnha.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3frpdcusy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbcrckk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3wwnfeyjo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ibuegtqd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bnpqsvxq.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3fnjtcqsm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3oedhdlks.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3vorjqsxp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3jsbpbgtw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ezfqebax.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3tfdwzcag.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3kdmkfhfj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3umupdxpi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3uonjsqva.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3gnlxliho.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3lnhpqeff.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3foskfjib.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3gqkpfnjg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3agcagjgc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3egricjnd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3dwkbflwa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3jzkzktoi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3lcrmjyzb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3qifzzrcy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3qcdkioee.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3eihlxuzt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3rmwkptpb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xahfinsi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlhdhrlo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3vgerxffl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3yxhlpcll.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ekrhivdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqvfddbh.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ufpudneb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqinkwdm.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pmfycvrh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3smncxprm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tghbmeex.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hqnudsdh.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3cfklxspa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3yhmcgmgt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3jxgaqybh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3mzkownlr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gycbwfgl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ifrlvuso.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3dddfsdhc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3frowuwbi.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqzohrxx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jnhycdio.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tcobcpnn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ffkrhtcn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qtndynvh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ehtanlna.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ugliovwr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vxufbzxc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gipaeufy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vzfbbsef.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yjskabef.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ffefdorv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3zcchwfpm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jvmvwsgq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3swfewuqk.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxwppjdu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3kaevgwaq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3edtclqax.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ihtlkrux.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3pnhkdahg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3daudebiy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fmdemkkj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lcgqnyqb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jxmkxzyz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3symhvxzi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kofzzaaf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3aqvnmtde.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oecefkak.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qdwthzol.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3dldwlulb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3mthaolkd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gbdeuhte.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3xtwhsbpe.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3cipgonou.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dflzzyhe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ozktzurh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ltjkwzyx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yvzbqznb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jlxxmaeo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tuiomaxb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tnylvepw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3izwlezya.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mchcxwwf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iapvqdau.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3iuwtlegc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ggufeavi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lossihgf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qbuodmyf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gkirdwqy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pdkhmzwt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gvbwrubz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dyfqcydn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gdgbcuaq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gouzvmpq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qolhvjxc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rlqbuyln.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mjvzlzdi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3gtwytzyp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3piptiwrp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nganhruk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juldfzoo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3fenbypuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqauulvy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yvojxjeh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3mbwkayad.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3cesfaxmf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vupeafbz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nsrxutew.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3fbukglrh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uaqxlyml.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3tuxckems.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cmuwbcuk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zeveyyno.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tbxraort.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3furynecg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qpfzmjed.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3oghqpowt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gufvhuyu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ijbpqpqg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3axkalnyi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3weevkzlz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3avakspml.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3sueqbtbz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nfbijoki.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vhwcvhoi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fvtlnfke.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xlnzrxit.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wbeovxsu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3zuxvhkxz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sxfiophs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3emhnfwrn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ncwkjcek.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3gguwfvot.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fxqmcjuj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ujgkiexc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3bwqewycb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ihazvfmj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3azjgzali.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3irgskcxw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3chcibgyb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tqnnjumz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kewoprhd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mjwgshse.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pikzbrfe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wkpoxhru.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3lpzomfpu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xemlzwmt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mfmktwdz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mekkeutv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qfthxoiy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ifhpinkc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eynbvgsu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3oiiswtin.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dcrtzrzg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vtuczgpa.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rexhfdeu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ivxisnqa.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3lyfvrden.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3pedzxndq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bfluhpxw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bxalfrfx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3psdwxoie.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3umrvfsab.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3oxedaoew.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vljokiid.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3njkrmntc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3etmigzus.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3iuunvjle.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3lwvuiqse.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bsbwhnzs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oimfjwog.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ymgtkmtn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3zjicdxhp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zhcqutew.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3engmwngz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqkefvas.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zapyfssu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frnkrfnd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3svghuirr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nuonxhnp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3kjzyyxdc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3moflfvfa.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxqislkx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wraumatd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rlfwgyfl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nwvvbcjj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vxregtuf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gapdavhg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3adfwtwyt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pbnidlac.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3essmbfrv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fiktpwod.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ylhdpxbw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yslorybi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vpyakhfr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3skencsgf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ufmjdopr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jijqzlgj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hspsundj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zzfbouky.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3aeioqdxv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qqidlmkc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3dabcrhin.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3agvodgdl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gnqasivn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3usbefauu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bthuxgsx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3picpftvd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vzcvmwxa.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lcvwexbh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3vyooqqgk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aiafxans.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ftpgkfql.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3brdykvqa.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wagwudjd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fjittncc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3alsprmlr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cimspnpp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3emuxtreo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bszxgqtp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lajjrbbg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3suralvrc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ynbqslne.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qrpqgxbj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bebiuodi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kurtgzmd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wqggfilg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yegttpoh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zgumphtc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gnqovuuz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ixfpjxtr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3komjfcfe.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zttmcmul.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qqcchquj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jfeyazyo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3chzzhlbd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lwgliegp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bfajqezb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mqdboehz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3gfdzjudu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fwextvgc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3syxpzfzh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3udftxecl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3schpnnwy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iljyjhbf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qqzpwxzl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3efqbaskj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3yyurwszq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ihzdzmhj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3monysnxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3didgzgvm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3phfrkcmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvemxmwr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3iymyqhft.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gdqewqae.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ylxprqba.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ixpmwdto.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aqqzqtki.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qoonttxp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xumhgzgi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fzjbpggt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qkuntjih.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3akjegeej.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zdvsigyp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kjcnpoyb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yfzkllrw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3netrmlie.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gcbzrsrt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pibjgiys.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xpzheukw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qlneojct.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jkbhjzua.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3lrdvwhln.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pafyffhi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fubhubzh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ibjrxfct.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3chnesukf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3kvdoimmz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3htzzxvon.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fnwiygyp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wndodjee.html


<!-- 参考信息 -->