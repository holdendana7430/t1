代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2wwrycqcf.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ybwgfjdi.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2iiufnnbm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2lemtancq.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2tgxnivaf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xhdotymo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2fctwxleg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2zusqnlfw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ynrlqcfa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2xekgzzmc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2yovzupds.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2cfkixqwe.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ngrjuvhd.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2kbjktwqc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ucgxwlsd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2eudhaflb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2chtictkx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2jdigclwg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2cyihgqpk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2oodnrjxl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2perwhrxx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2avzmcxhq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2hbxhseok.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2rigtyqlr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2btjdvdud.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ouwkeonm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mqyexflu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2vqtjilxh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ddtdbfyi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2fyxapgof.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2veqjuiat.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2aupvxcpf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2srfryxvm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2xhwiyxgq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2esaeexod.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dehjohfw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2lnszulyi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rbjfdpat.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2qaaqzbsd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2exllvfgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trvtnoyi.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2unyqkswq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izjjatfa.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2vmnhdaqs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2irgdpxcg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2exyxlygw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2udazbitx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zemvzpwh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2rdvfzlpn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kzjfiudh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2bdvbhbbx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2okxszlta.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2hkkjrhad.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2szhimglx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2frrqyiae.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqxnomrf.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fjlhmdbz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pgasxvxd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qridizqj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2phsdthac.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhpkbely.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2raytcxmi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2engznikt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hwwfmajv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gjsgqzqe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vyvbqahj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2kxgrjble.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2rhbbcmjk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bsrczhmo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2quhkflio.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2qrakqcfl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2quvjihwh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2btkgyovp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qlcuiaok.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xleoypdw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2aixhcsdf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2zirdrzxj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ncudjlgd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2giprqhqu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2cjcbaevg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2dweuernk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2osudjwox.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xgymxtfd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rnemstst.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2etvsjuqq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2dgjclski.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rkckhamd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2klnmobvj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2xeiwiuec.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2naboytxm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zknmaigm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2arqaplnl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pkgkxdvi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ofaaxheu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tseadlmx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rzxgkcwx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pcuiygst.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2sginkefw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqfcwcs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2kuorqvzp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kmyoifid.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dwjbwcfx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ixypounq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2krvdksix.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2gatohiso.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gmiwivft.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2hczanakg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fwohqpca.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2olgbampv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2loqvwhrw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wkcxmyls.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2lrtoqsvr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2pbdtecow.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kwqyabmo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ywkegcau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkruahnr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2tuvqmahi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqtqmwrb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zdeqtlkp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2gvnhraze.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2bsmirhbj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ombyxomd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqodoyi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2klqmdcqz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2eszzgfxw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2lbpxcwrr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2rpfnnnmw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2loknsgeg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xqrvbwxh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2rclomraa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ksglfjod.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xqzraunv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yylcqyqc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jbojbtvf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2kbqoehho.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tyrudtag.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2apmgrmvy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2bxkirnob.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lhqkuwbq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mtzhaucz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dchsnbbz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2myknnnyd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2binesyud.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pcnypqpo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kbthzyoz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xwpkiqyp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dwtyigod.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wjdxsybv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pdrouqkn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zmwfskpz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tjeemzuz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kmmhyjxl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2lvihprtp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tgppesll.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2brwodoga.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hpsxcjap.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ivqnvjlu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tjublbuj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pxhqwpkc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2idrwfxtc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2yzktbzeo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2fnfsgxzr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tfzzzyzf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2eisityfh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xvqoazar.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iserlqvd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nrefhmje.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zuzrbbcq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpbecgr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jmkmrmvd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2piallcue.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2sshegwcj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fwwiofpy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2nxbruoyw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2xwxcnfjl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dfexmqnk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dfhahnxq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2cvmbsnma.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nwlhnrye.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2bexadqis.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dezkndcw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2saozcbjw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2sduganhz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2csniwqwv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kkpjefzv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2thxiibhx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bhsqucsv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2vgqgjlfw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mqlbruzz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qapgraam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpybnsha.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2wnyvhdud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlnptzjf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kqryfhyh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fbdiltaa.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2uhzcaehp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tuetlapp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2argcfhbr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hahxotkb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ecwfgovy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2isbffkbd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wefeasgp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ljttorec.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fnyvoydy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rrryiojo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qvonxxlw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bjanlqsm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iicipxap.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rxsbqzhe.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2flzezaqq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hxgqopyl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2aleqxdzc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xkqudkyw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2dtignlrc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ipcdvrdl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dinmqaql.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mlthfxgh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gomakktp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bskbqhwq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2lxatttup.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rzpurfxw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kjwnyhsj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2aztxeztk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fxbqsntm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2shfxrgoc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2vnrxmkmn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2uagtfgot.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xgawzezg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2muqojasq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2iqqseebp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hplsjqws.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wiffcpdi.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwpoockn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2panpihgd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vxoxqcmp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fsdvbkay.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2nshpulye.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2oqhjrthd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qsdfpgau.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qltjnxkk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2gzruwvku.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eotwltny.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vihoiiim.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2awygvyhz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2jtgyvcxx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2nqwklslp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gkffbarw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ntmwzneg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2sfkrtlzw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2yogtlnsk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kzvgmxmv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lmuxylqs.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zeniabqf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2barbnola.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ldzqsxif.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hzefarbu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fjavztwb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xvvnzwwq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xjomogrv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cdibtaqp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2julnyrha.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2skmwuydd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ljvckfxz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jlotxtdx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2fltpfpkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2alvgdpvd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pjwmwoso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbexhrtz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xbkpfcun.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qeiafteu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2efggbygd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2phbtdmas.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2duexgkyq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2isivhloa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvskxttv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yzlbcmqt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mrrjitqb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2usrcjjxk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ztmlymyc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sdejjzzj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2grisdwcw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dncuppve.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nrabecdo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nmuvlxpe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vvucsvuc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ocjkrrmz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qwjegarn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gvdilxgy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vjhuqwpt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2goyewsfi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ubngbmjx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2stkdzsbf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nkffrmwr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vasiexhj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yhpnhsej.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2tahatidx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ergswksd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfeodwuo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vzldvxpg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jmmuxvdd.html


<!-- 参考信息 -->