代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3cqulrwef.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3vsflwkyt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3czstjcfy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ldifhfin.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3znfezybs.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3dbnhpmfs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3xcsiimaq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3pblratmo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3gqbkutki.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3tmgccnnj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3slnxmarv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3bfknghvf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3arjsrcrg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3knivhoxz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3xnozqjfn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3znhkhdwp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3akkicamr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3nncxvwrw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3fvikmfir.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xrczvdnd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xmlhjogx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ywblfqcx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3aqieozzk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3zrdwdtup.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3zzbrevco.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ngshknwy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3erbifrtu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3xqvkzmvi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3lnmrdknd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3zlnyaddz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3mukebxsv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3osqqixbe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3wkpbqbrr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3kmvisulf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ohgyacok.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3tdgaozoo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3nsybvwqu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3remhwalm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3xsafghtk.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3mecyyvws.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3thpcuecl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3whvnsljm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrnfrutd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ibvugfyb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3sraualxg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3elphgkba.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3kmcqcdgw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ecothpzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlafggsj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3duruhlol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvnpspgm.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cxomepyt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3vgadtscf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3twkxwrhm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3flfxfnfl.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dymvtoxu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3xnzpqcvb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xcwujorb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3mqelytki.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ngapssel.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3lwwgrmcw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fggjofhn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3nueogydi.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3imdufnny.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzyhoejn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wkdwaqfy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dwylynpg.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3alqnydkx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wpzrdvls.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3cuzrbpum.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3euepcolj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3dhkexhmi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tuxcagwc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xehrwphk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nrdqvlls.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3aicfdcjb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cgealpof.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ldjshvet.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3tersmzrl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3hooopbam.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3fvsadkhd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rybenydh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ryxtxikp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lfxeoukd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ckdegcvp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3pkmjfjdz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3whmlqjfb.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3hibkdmok.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eazvrkja.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3suqftlqs.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ltwyhvvi.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tbrtvfyt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3dwivqurm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3bihuglle.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kuryqjlj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3qzookyxn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3pnoortao.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zjazzjkx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3syeagomu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qxmxewvl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lpawvssr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tikedbpt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kigpsizp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rjspzmpj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qaltcdxi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3lvvqgzfz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3netozdvo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ewpbsuov.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3klkmnxaz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jpuxlwsn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3axpkmmga.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xsvqmzwa.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3otpbldbh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mmsaqabo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ijroqbxr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ocxurpvc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3twzzcpik.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rzsfmcia.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3tsphyjpr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3gaucvxoy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3wtxdmjld.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3vfxwpzxd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xihynbaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbbhmeyx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3siatakzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqievjsl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ucwcdpmg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3echflfak.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3gmgbejqk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3chtwzehh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bpbrnkqz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ksisqosz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fnixzsjs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3mbkhepse.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3swclanjb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3avdrnuug.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3esucdktd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3mcqafyta.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gjykqoil.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3abvagede.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3yizlbozn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3twigitas.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3paabemvd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gtdbjret.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tdxvwdan.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3peqacilj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qgoxijzd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gbeexawi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3acevouen.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3pyepgwlk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ukyocher.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ymcphglj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jayjmnaz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3kgorfdyh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ashtvwka.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ovturxfp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nwgtodpg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3pylnrkwb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rvrcuqci.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3oesojnrv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gmjraaxk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mqjxoapr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qvdoomyg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3epsskdcr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3djsrozkz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tblrkkje.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ozroobda.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3pbzmqitf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtwilzpt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3scyjvqlf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kvpmryzg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3jmznlino.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kyoiowgd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bnrsvdfd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yibunfha.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rcmdsirk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mdjtgtkp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3idzijhdr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rkcsvpmx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uamfpdhw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ewxraifb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lfitfcsl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ssvaoukb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pdbjtblo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yzrnuibt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3iyiokbyz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mwkvhrvt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wuqjfcma.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sjaqlqaq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3kkaitqcz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zwwzkpnz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pxsyxwox.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3syqyqdnc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ncchmusx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xznyvknb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hmolyrue.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xnprycjx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mrmxppgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwocwexw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3exgvorqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nluitdtf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zgpkieek.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ylwqspxn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hbsogjys.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjanrlvv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nobelldi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cjipbasd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3nhshyrlh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hpiubfmx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rmmflzqy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mvobcfnz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tmqklogg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rijciuaq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3chejffyu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qfbchrxb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qbpakeba.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qojudvpt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qeaabsiu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ikzapxhf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3boygnxfd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3agcqecai.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3oadwocim.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dpsunqrw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yriwinnq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fmyqkumd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3vcwfixri.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3vhpupjzv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kiluuzln.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3awuauowd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iyolkzjm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3tvqxzblj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ogzedmix.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3scenokyg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3gpvborgb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vqiegvmi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bvqrlkpj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jiltwbqv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3bzksaroo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3skmopscq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ncoupfvc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjgssniy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jgmsxiqx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwzklmwc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3twbcvyrq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qgybnaky.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qfbuvvmn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qcoieved.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ajvhxwyk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xyxtcsjf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xxamnqrh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ywprvyog.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ayrkctsz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zwxkddrl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3nokpkflu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jslnygxt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mhswsgzm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zpbltowl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vpweeliv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3agdyesrj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ngtpnrey.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bavtfabo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vuhwtloe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kqtedmik.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nossxkcc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ckisaemw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fjviuxao.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3udplisec.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3khyaayei.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ukasgoiy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rahsdlfn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dggocgfl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qdyyhhun.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gbwfhnjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uicdyuiu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mijrqfpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phfomyqj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mlgtceqe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3puntggin.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sghyotjj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vrljxeoc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ghplyrbj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzfhxmqn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wkalvnfk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3todzanyo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xnyjftuv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ivbbemnn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rpolxcxm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vrrmhomh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3giawkvsf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ppenhjss.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3regypyrx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qyyllogd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mizhftaw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fsjzgage.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3whiepkae.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3oyapwrjt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3fwuotciv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pkpxipgh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zkgjgtqw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3kaaiobkf.html


<!-- 参考信息 -->