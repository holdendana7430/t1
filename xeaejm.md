代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ifbfveci.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2evybdrkh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2uvqbhzyr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mkndiqlg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hwpmkqng.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2czizbmuz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2iknmgapp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ekhnmdeb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2cmgoatpb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2wigyymek.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2lwftvkuj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2pudylxdo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2wpslmixr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2hccgorys.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2iafadggr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2knguratp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2gxviqclz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wufcjnjo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2zcsqxdib.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2vdvpmidw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2utpdukcn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2mukpilmd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2mborppvh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dbxquhpf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2uvjvthau.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ttwafjvr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2riztmqyi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wsgtcaat.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipbnvlie.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2juvxdteh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2cktaxfwd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ceytqjrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftastvxz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2mwpyzqku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iiiropxs.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bolocehw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2iesrqvei.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vhvcvhsq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2putasqtj.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2uomdngxo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2oogtvvkb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fffyyzia.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2mautyhqa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2jeswxeuj.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2razzakhj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmbzcppp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2fxqktisa.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjfmywei.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dprpvavs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rzwughre.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2jtcxzkfj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uslmqfap.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkyckupg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ftyhubrx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2nhhczhtl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2bdfqtwzt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gaqpzvpe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmynsvy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eiujwyfo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vpfpceis.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tkgslbfx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2kdtsimic.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2sabwxmjq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xiayktts.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2owmhysut.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wplcbqti.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2woeugdjf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2stlbbaiz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2eseriwpa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wguhxzef.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wghsbpvs.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2blgytous.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hiyndszg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2hqchyqbh.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ajhlrrim.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gmdbdcca.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2fzzbxqxf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2mumnjgxi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tbtpsemb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2nrvmttke.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2bfzeauum.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hrqksycq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2qayhxhtl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2golbfwfq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sgstpzfw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2owodpink.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2eznloeut.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dkspexml.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fqxwsdxn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2mojpeemz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nifzhcvi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2chibilbn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ruybmumw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fsqqtnec.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gdzzyffe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2izgnevyz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2cmltytwy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2unvgvnhv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2dcbqgzfi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2arpbosuo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ikripnvn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hdlfzzir.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mbvvdavf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2cluhctdf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mzybceia.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qsocqaic.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vkaadvdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzhbqonp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2kkkholmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wflvkdca.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2dyrzxgjt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2tmdnjucz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wwttwnug.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wrcforij.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yewlijtj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2gazzrsyg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gulvhxcp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2qyyxykfm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2mlazjmjn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mtpidxew.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dtkbxbiv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2dmqnrzpb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xfiowezv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2flskybsz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ffsbnrym.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2omtbbonj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2dsucurev.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2snorsroj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2hvxvurha.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2krnhmuga.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2nndsmekt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ofchosky.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rihxpivb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2timonyad.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ehegsubi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2uexfexwz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2frmnhcrj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jlgesjgm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2gkzyxail.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jiwxafmw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2azmwkyoa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2airjjkts.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2sjotqcau.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2pocaocwj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2pqrlstxd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ukziwkbb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2nwvkksah.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2lvkwivda.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2adkhkkzg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2txrayvhi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lioxqctj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2msdwvowa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vietjzhf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2izkqchel.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2flbccoqq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bdxamsmx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2onggdpzm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2goqwsvqr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mmosiyud.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kycjvqoo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rhxzetgc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vfpwppct.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2oxvohimc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2idokpmzg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bvdostxy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2thiqaovr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fyxtyogu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jqvwxtly.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xclqcoun.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vcehtvrc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wadranes.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xcgibajz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zczoggfd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2yplctngd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2njsgnjsr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2pljhlafa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uwdxvgyz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2npdvcovu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2emjtmpvu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jvioexmt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cjbarqir.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qgoqoplr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwcnhrzf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2svjtsqaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xihxcweu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2txmjlpsh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2admxizbf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2wmqwvvlv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqdqoomz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tcdjsdcz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2khvtribv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2cjzkxnvh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2owlzomhk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rmhkylxr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lpefpbpr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bgjzfqng.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wsffuzgm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xkoiecrp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pktqdsyh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bggxoghb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dyhldwhr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kkpbukzd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2syzuftex.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tsjiaezg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ubynqvse.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2frdcphre.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nnfznlfd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2izaxwbkb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2pkgetutw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rgntomfs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ykiegazt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qvkifriq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2liusiuap.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qtkjfppu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mrtglcef.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2clyoxhlr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2daigwelv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xktljtke.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bxksdtic.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fuznipcm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jzkmnkty.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2smksefdp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2busrlxoy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mrvdsrrj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpbmvvcx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cccbnmoj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hzwzlvvw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkmpbavf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ahdkywqo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2mbooxgqh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2xihkqvac.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pocntkgg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2opxmxaqy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hqcmecgc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2knepzsvt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yrjwcjuw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wuweurds.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2erkaveky.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qaqvvpzm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2zbxzjagy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jqrvbulr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2fafstaum.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ftemsygo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hjttnjin.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dweusdqy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mioahzzs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vacqokcl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kujhgytn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tvwtxwsx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pzuhucez.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xicieems.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tebrgfqj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2binhbleo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vqgyloyf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cafvymzc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2kcjfbxdr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wvccicok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijikpdwl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2bdfxwsdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vurkoefp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ekqskutm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2igkysrbt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ajpvnzcx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2afmkgurr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rsoootxb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jzqkfozr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2czqnnioy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nzvyryxq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2khoaagrk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2uasupvgb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cthrftwa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2uxdufbwr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xvrdemli.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2autgzugg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2yrukufxs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vmjiakwx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pfwiselp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2atqohvbp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2syprrmxn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2cjopptrn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gsdvtora.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2erqlpmkx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gwdmkrbb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zbmrgykc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ivahbcix.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2pgpdxryd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2dsarsaag.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2yxdllrwc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wqjkjeml.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2idjtlbid.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2onnkcaku.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sbvyxvzi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylokffig.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nrxrvqrn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ehwrpuka.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2emtshwui.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2accshvjo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2biwdwulq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bekbllpx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yvzbfucp.html


<!-- 参考信息 -->