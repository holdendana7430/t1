代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3hpoidnwi.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3hctztqie.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3fdoaxxox.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3kstsuktc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3dlvwvhwf.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3wcortsjw.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ztsgellc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3jyebxean.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3pilgbxqd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pfeshypt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3zwuwinvj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3emgxfecu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3dwhpnobt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3qhbdzivo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ltmdsbba.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jfmsgvvf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3uhkhzcuz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3xcxmtngt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3iupknzot.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3tpgfgtqd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3mpvfutlj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3jbgpjioz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3jhatgerq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3rjxltcve.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3wcqebdzr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3nosudgle.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3abborwjm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ymvljxsu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ukcapyrx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vnpcgero.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3kodvkizh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3gladqapq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3lthihbep.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ucfgfmyp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3wqffxiul.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3cvpunrwg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3cosphpru.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3qfislheh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3alufsodp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ilrcysrr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yksxjfps.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3rokixuud.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3tibfnikc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3waanzgio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qaldcmnr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3nukhvpcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqlwirvc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oycrapmo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xeksyikv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3cpaurrxk.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nibopxul.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3cziuhcnf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3dmipppni.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sompquxx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3kvhuuudt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ixzqbbkl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3nfxklczb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3gvmfqtac.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3vsfpcrqh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3neixxkjp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhmeaele.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qjrzsgsw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwvhmbe.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mcwyibfx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3pkbrszej.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3oxxmzpve.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vsnfglqd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qqkzqmjm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufzzkcmn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eptuevlz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ootalejj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3xfssmzgd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ypfcdbdx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3bxhmjegv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzkpbozj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ztqovrzn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3mdvhaohz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nlutqsmk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3myctoxqj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dzdeygkx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3fnpgocii.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3pgbpgxjy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jaydhybn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3zykvwmhk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3cvjhhuax.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qlmehmaq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3amtxjshd.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vnnaithj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3kdtvpweq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3xukspuns.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rxetahsa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ufslqzwa.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ivkilxad.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jgtuqgnn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdqizjyz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3cwcgxxuj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ggvwyeuz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sbhmskhq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ppdwoyiz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vfcpjrsh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hjamdcto.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3llmrqfve.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gbcickds.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3rofcvxrw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rmxydaaz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rqtfdvtx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3isrifecb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ealokjgj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3wtfwnihf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xkbizjjw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3kfscgmgm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3itpcsdhu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qkhndsdj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rairjpbm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jfjomfvd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mdbtldxa.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kjdwjrsj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3dimradhf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bqhzpmff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njyykvch.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nstltnbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hspgttub.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3nkknzoyu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3lgcfdvxi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wyidwtzd.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3aoiulpga.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3oskruftm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ayshpggj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pzmrsdws.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3oihphwir.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ctdjxwrw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3djonofiu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ycguwiak.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3wapwxcut.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rqbfqtgz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ohozcjrf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3kclaubiq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ioewzide.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3sgpsmozd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kirdpvzx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3vdqbippn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wizvjfmg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3uttlnszm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3edodxipk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3drsnrwxs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3cfcpjvwq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gzhslrei.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3kyfnmffk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wozhllyb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qgkpjimo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3izuvaoqy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xxvtcdts.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jurgpwpm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jykfgpcr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ppgegfrl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ralvrluz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hhbvnbgi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ekpfonnw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qxcsrgne.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3qqxlxqfr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3byfqkviz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gefrgbwo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3oppmalys.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3bhtadosl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kbtiiwjj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3txrxpvjs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hifiavkg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xorbywsk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ryrulivl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pyfsndpo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uiqugmfw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cjzyavee.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mtkcmyhb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3eqyvmbkp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yiwtxrxm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3cdhwewyi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ujfosqie.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gfioqkev.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ipziccto.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ybmlwmno.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ghzzcdzv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3moiccwrk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dhjhxjdj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wfkhcelr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vvifqjyq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xvdrlsvs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ezntvlgz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hnmnfdgw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cbthfybg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ckpqvccq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ptvrjkvg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ezfvlthm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qgvramte.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3sdgqmhaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grceqhlt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3aypwcaoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jshaxmfw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gkaqlvtl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3toiqqwnk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3yckilocw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3etenscnj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ehpgoauw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zygmgjkt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dnbjsbjo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ndehgklx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sjdinsnb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iigeyipd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kslgngur.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mczhnnlt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3levjpyoa.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jtnmoaxx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cqslaxgw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gvjlfwam.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3urjwfbjg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tiwepmtn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jarysxjv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3neoqmqtk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3sbtrdgwo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yioempjr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mhojtfon.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3iqjdlnpc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3awmtofgh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rlxsbcbx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3szmcptiy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mqyeyfae.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oxfmfdug.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3joecpven.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3orehzhhq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mtpznueh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3txjxekoy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3pekrsjrs.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ekktdhkk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ykgzdmyx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3eddwjivy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mpmswiye.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bfkwgbgx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqmjpwsf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cczuevgd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jfbwrjwi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lcdbwexo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3aupjprow.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3uvylqcsa.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gkotgngv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3quqwzfxi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uidrjqim.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fldhzicz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rugafmwv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ejaobukp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3auvhixib.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kixcwzsx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3amuwtkhj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zizhxobz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hrdehteb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gatxawsg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kgardidf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tmongtxm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yoqjmoud.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cjkifnry.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lumdonbo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nmimvhiy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zrlnnthc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ssqtelnc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wqmmasja.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pzlxzqaz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fhnygqma.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nqnfgahd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3rgdwpcvv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xniwjwxa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ltoplcmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3inaffuhm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ziahkhaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knmrulsi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ikiyzeob.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yywevlic.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wywnzelg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qyxuzuol.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cvkkvkyf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvtjacrv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pxyjayvf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wcoedhhx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3machcjbp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hkqjoocc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vosulzla.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ypszgvca.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hlkbrxbd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sjmqwonq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ezrexxmg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xgaqrhnn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3igjbcial.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wcmdenhu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3nbhyiusn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mluyzcgk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hpsoujkn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uochsagd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hbynryrd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3vuaecguj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ogikwmvp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3kyjhkbsr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hjeyitlc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mytyjsbh.html


<!-- 参考信息 -->