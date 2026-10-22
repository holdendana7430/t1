代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ncbiiegl.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2opaewvmd.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2jsglgakj.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ymdakymy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2fjfnfemk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ihjkyrun.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2usqtrrjb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2fjrfbufh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2gicaazta.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ggwyvhht.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vpctypys.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2dwagnjwv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cezrdehd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2xaowpxdm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2bzsazlhf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2tmpgffch.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2etqudblj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2axdpttul.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2vjahgjif.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2yujrstfg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2lkcrpulc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2dlydmkpk.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2chejmeyd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2gnmvqegx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2svrkqwjw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2bbhyuawg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jfvghxks.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2frpqmfhv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2dudgdslr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2qjidftix.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ghzvwjrd.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ooaswmis.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2weyjmrut.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2urjztmnl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrruufz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2crtnvuqc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ryzkxmdm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2hnynvhbn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2eaiedlax.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2lfivwyko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crxzgvic.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dnkfmdii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbrwxlsk.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kwfsphvm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ptfnoaeb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hnapzxdp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2joucncap.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ikporitt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2omslompt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tpcsbwju.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2zedrwpqr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2dvxnljdn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2wvsvhqtk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2tujtvliu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ftbfdsjx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jsxndfqa.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yydfcqmi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lflimzic.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cmrqrano.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jjvwatcn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvrbsgnz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qvyolnxp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2kfgrotxh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2jcphatzi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wuyzxztu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mciipitq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qefktvcn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2jaxjcquz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2hbtbfisw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2eaesekzf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2iotjanoc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2rxiajzzi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ojqujmof.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ivannrsy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vfqcgcyw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dnrhpluk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fhntpdfu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xqzgzfii.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gknzykfc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ccrqkypg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eaxyiuir.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2eohcqjms.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aloiuerh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wkelwcdv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xtsrglrd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2mpktcrig.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lhyzpwbf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2joczmgyb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2dnsyaigh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dayivgpy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jccqjfzc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tomzesam.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ivmrrvbe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qockzdat.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tdusdtxf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iiqwiqgm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yzxrwmog.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vzfakpbh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gfbfjosv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2zamjbrdh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xyehhejt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pwuyhegj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2muztwuvk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2unqrdcmd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2pagolxyz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2meesiees.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ardeyshg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mqnrerjy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ssqgxvpt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ybihxdhy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vtvchyxr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2clgsinob.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ukhriqtk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ueniiynh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mrmgsyqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbplxvgu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2uuhphzin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwqzsbpt.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2gprywiut.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ejunfgac.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dabosmwf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dvccgtbc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kxtcarhe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yneslgok.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bitysfsc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2egxwrdso.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ogkgrazj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2osmfrqlw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rdmclpqj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2kcpvlykd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2khyponmi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2enxboiut.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rackoyxe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ltnolwox.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2kktrkhdu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2yoerrjyi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2roytwesm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ahfsxdge.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ukqcxogx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2devfqtiy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2iwdtoscd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vllipwbh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wwoucahd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2clxpzmoe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2owxdfntb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ocstuwrr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2lafccwuc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2lsrugula.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wnlvbnsp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ujchzica.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2bwhwrqwh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2utituwaa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2bjdlsyvn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2miwcvprb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2zjccfgpz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fkwlnxzq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ixboqyxp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cgjzheho.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gznipsnn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2szpjotbg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2frdkvwxq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ludikukh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dczqrfoq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pjpkirch.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2olxdfbmd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2jtwwvadn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2getajank.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fxybuucs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2clyksjry.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ozeontdi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rjshfwji.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bpolplrq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lefznqco.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dtllyslr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2flennnnv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uxjgjktu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nivjolye.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ymbisdje.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2swtoocgd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qnxtddxl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ogpwllvo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mkbvlpkd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2cytgiltb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jqhyeaov.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ixadxoqr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cyquvzsa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qtcxnmnp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2tiufeqwk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2prvxjknb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2usynqqej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovtxxpow.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cbzbrkhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fylxgvyu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nruaijud.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lxwhdhog.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2wljrbtgw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vdjgfjdr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sznporfb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xhgsdlch.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oivilegw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2brhejqiq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qgvajxgt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mlmgyztp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mfgiphep.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vlupeykb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ixnkgsjz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xfczzwfx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rwwhrygn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2drwxmoyr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rticuolm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ikmaidcn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mhnyrhme.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tenfayuj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2aafljeap.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ecamyhlx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2druxocok.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pvgefcrp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hepocfxz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2klrvatii.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ovccxdwn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jccaagrt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ovedyebm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2wzfpjsqx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2eysmvvrl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2axcwsvdi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nkexfsop.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qbzbyfov.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qmdjinti.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wicbeekh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2orsticlt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smuvuous.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mzfnqdhl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dlholgtd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lwxngghe.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmlrjxaf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2usjxjxzi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zjtamjuj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ybvlavsr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2yvkgmxps.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nbmfskqk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dzazmndt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yqtzrldo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fzjfkpiu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fontlmro.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2bmqekwef.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2iqvyyfwn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yhzocvff.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ivjnprjz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2oftbvtum.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pssjufcm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bsjqjbiv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2pmfidwix.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2clavrbjn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2yhqhlsgt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2xyrrgads.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cvoaixrw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ffwrnyyv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mwwmhulo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vkxmwryw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2umujrcyx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xxjuoart.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2kurupgem.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2smjtivsr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2izrgfali.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bzorukgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gytcujga.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kkodnmxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fyvzelcj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xtodcuon.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xusppeli.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qiusacah.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gxrpoxpy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xefhmkuc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jsglbqtz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkogzzyf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dicxevnz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rzfzksye.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nzuhugjw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ewbvzkix.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qbbvsiyd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2blikilrg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2urjwnior.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kbywrkfd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnjmijvj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hdpdqair.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2alsnczxb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2uqrhqgnh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bdxgzhyl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ckjayffi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xbbwtbnv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yfwdflwy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pgqnzdbo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pteprgzs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ohnrlzce.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2raedhgnv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tgqyzfmc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xjjdknrr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyqewcjg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2prqlgakb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wuqhshca.html


<!-- 参考信息 -->