代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2yacpkrwg.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2fejennee.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hjwjeqkb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2gctrqjfl.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2qpyzccma.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2qfvqdevo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2wskaluff.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2hlsmdgxf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2bpdgzfdj.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vcwaypir.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2mxujfrie.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2nkfnievk.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2cydilodr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ogfdoyzf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2jivbnehf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vkdfkjgv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nnvqujei.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2mxulburr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkflwgza.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xgotxazu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2iodthxxk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2kvngixaw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2vtujdhkr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2faaimidn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ywpbtdsf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2bwefydfl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2bjdkcmld.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2qjmctgqq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2possgqfa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2livnflps.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ntqqbdyx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2pytdkbqo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2bwukkvuh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xrcskcrh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2wzyflqtu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2kotttusl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2lovqzzdw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2iytvetwq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2tjsawbtv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2pegjobez.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2zapzwmno.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2igtlorgp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2cmgheczy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gznujpin.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2xwyepuxp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2mhlnwhzl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ehektzzj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2fvduaufl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysldgpvp.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2julmzprk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxiszjgp.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2xmluycve.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ngunbumn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kqvyekpd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kjodsyop.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ezqmphcg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2wqpoyuhx.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2nevjmpgd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ztkeerns.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2vzpjwrof.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2idaeyphz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2twqoglev.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2pifxhfpf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2axajpvfx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytjbdvrz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nokimwwi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nhpfjfwv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wkccnsek.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2vbbuuxqp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ylrfrcyl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jnybhdys.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ynhnbqgg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fffdbqra.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ulnxyfrq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kyzvjami.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2mtxzpdwe.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2chyvuavu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2cjvqibea.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2dqsxmioh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2kclrkswd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2jttqrkbb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zwckpanj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2aelumwxk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2crggknxz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bowsposr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ijudtcbm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2obqyzdlq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2mijidswh.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2xwoonmmv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kgbdwkgd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmuaapb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2eyhcblpj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2xskbrleq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2fbjrqbyn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jtaqsymj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2kxnjyeoo.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2duddklvj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2iqofemoz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2yrucwqrn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2asfdiywr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vhaptzwj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jnynunqm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2magcodmv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lkbsvsrk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ddijdtbr.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2nkqnkmiq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2juaaczfj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ezuhgwpj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yhenwmxi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xhuajbuf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nemjrwan.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2viiwnbor.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qybfyrpm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2owcutvoz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2uifaliuk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rzazaswc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2gsdrczuu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xeltslbn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dxiszobd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2dbvxfvvi.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ifeyutuh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jzmlqqnu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uzzrxhje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zykygvbn.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2xqcwuckd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdoyhcmv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zbbyrtab.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ozejnrah.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ryxeawmp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ksusvlhs.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lmrbkcmq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jvaypilb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2fycvkiji.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2sjnnexkx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2bnhzxfmc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ouoisuzn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kstetdpa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2swlweila.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vvkuiwcc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dldodfry.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cbdyvlev.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ylkjkwhk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ywnxlztb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wtyucukw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2becuagpg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qlhmvtnh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ifudtbcd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2imcyooxa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zofvyjxc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2mazwlutb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2akrfucds.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zoqxceim.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ooehyqry.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2buvenofn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2gdbbwdgb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2okotxuwf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hyulwrgz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fyqrhyya.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wlesibxt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2afodhiim.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qphepebd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2suvmerou.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qhghzeei.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ogktzypu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wycqlgdb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2elbarygz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jebgvyqp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bolxqyov.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2emneixyh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2yljflakv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2svvxugli.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cetcktro.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nllhsivz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xnyrsazh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2davwiomz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mthtlwwk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qylpyvxr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2iblunchc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2igcgtlbr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bcdinucj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dkxshcyj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2chgpnkkz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ulbmpeig.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jqwsodef.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qjtlwscz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pnoirskq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kqioxuiu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2hxpmdqfs.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hemdgkqc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2txaejbqr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jqfuhjqy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xhmnemoq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xxmdglec.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qdkqkdvk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2gonvslui.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2oiwjttry.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbwevgx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eaidttjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhilvtjj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2uxovbnnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrfsrbod.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rnqidybt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oczklzgp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dlrxneqm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xeflkzct.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrcetmmk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yccuxvxt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2qboytwca.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dtrvbulj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2sjvvupos.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mrifwndg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rqrboslx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ezlnhyxp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eciqojde.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lruwxkqp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2erezxslw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tedshkav.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2sijowzyk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hzlgfsur.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kgbzzogp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pztgeoxh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2sqnoddoj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2obvfupch.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vguomedd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xrqbufaj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2phufhwfh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2pqxozaah.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jfwmcrmz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2icpkrlkt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2rdspeggu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ljhnenmm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2psydlxqr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2htdojxic.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pmqnasgc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2myljvnph.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2qzpbxtxq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2grfuqiod.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2byxoguas.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aybdhupx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lgvuuuwr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndhnrywe.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqulqygl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxhfwkfe.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztalyvku.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2exjgtxsh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2gqdygmzz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fdprcslg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fkemiceo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2giunkzkd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uebxjuak.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vtvqimob.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qmiwwwmz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ectftlgg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2dqzuqmnq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qlbtysyx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2gznudhvg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2kgpuqucj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xqaujyqd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hfyauuxt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zjjjsvkf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zqzsrtgz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2uemjnbso.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hckoxrpu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ivaqcmxm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2keskhsgy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2asbhijfc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mtsyclle.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tfxsttkz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jcocclqr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ltybdyol.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2gtfbtfxe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2drgwgbbd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qsfhczjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhpnquzs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lwyoylro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjltssjf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2czjcqxfl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pvqmneca.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ojprhnpx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yrwqfknq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2swhmiexc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ldkhaqxq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijbgmvtt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dzkrsjgf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rmlnveji.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2etkdmibv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vjuzwxud.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kilcegsv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2raqyxyob.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pgdzgvgt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wbvfzzji.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zhahivco.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bcqmpomv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2barakyhf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rdgxrjdd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ubgwvcwa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rbtubsdc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2afprpjyy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2euxqfntg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mbigoyoi.html


<!-- 参考信息 -->