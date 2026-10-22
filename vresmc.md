代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gzbtnkyf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2szhsttxv.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2vzalfjcq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2mwaqfkgn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2canvwmmw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2rectijrs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2csrioyvo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ibkvquan.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kulhibkt.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2irqypqcw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xxwghxrp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2hvliljym.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2gmxgwzfg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2puribppi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2vgotdrno.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2juethism.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2aklwjnbd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2gkirvssy.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2wjevnzmo.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2mqpcnphs.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2scjxglac.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vfockipn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vkucnols.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hqqstnsd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mykqqcdi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2bmvhfgfo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2aaogjtjd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xgvfudzd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bznrhjgj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2hwwhuvfe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2iwapavme.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2bkkiifkb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ohnfvhii.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2xxejpsvb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2tkyrltci.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2nubblyvo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2qekjdtdp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2pfuzbtrg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2zgfecgnx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2pdrdmdxl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2lejhsbhd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mjfeneqo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2szncxhqi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2gpmpncvs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2fmkyrapl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2bhcmzqaf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2fqbxithe.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2arybuhlh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2vrcpjsbl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2arfmuhyu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hxshouya.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2tseakmbu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cehrecio.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2lfzmpisw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2hmnbescr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2vreixzro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmrvsvfa.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2gzvgnjms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eecbjdee.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2rzvxfmsk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2sedynbcu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vzldbkcw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2bpgvjuth.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dtckzoja.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2olxfvmdy.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2udpgwbaj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2wwswsckh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oymqayzi.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2voguogju.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vpevoxqa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2devamqfh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xoijgmau.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrkdibax.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hvgidvbp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2neqgvnej.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tqvfnuft.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2blfbmztq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ycheusvi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jbqahniu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2judqdoez.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2aaavnhsy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aixxeixr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vofijcir.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2jvbesyxk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2oigzcddv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2hmoahpsg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2aqvpuaxz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gcvlcizh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ppkghjpd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yxfeejmw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2iasxfxfj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qmlljcbq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qitpqnqx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kzyuwsrq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kexhiuyq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2tjlncrfu.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ptyzzsth.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2cyrjbzid.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hmlkyuvm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zjlobnzk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2lwxeegyw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2pudrwtxf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2bhahakuu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ulrafllz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qysqgudl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kttifuun.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2wemqxktq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oggorrsa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nibxlmzn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2qzsnyhyy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pvpvjjxn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2shpretob.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fhtrdmbi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2zlauchpy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dtehaqiq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2bjnzwijb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2abdhvalp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sldtowzr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dyhzjzqi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rtcgwlcm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fyshihrv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pjyirnhw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ycvknjoq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xvebzzcj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ktgpijvy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ctwlawic.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2miboqwhn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qvolwxka.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yraudczr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mztckoym.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uxunqdgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbzwgxdp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2slzyzpoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tyyyufic.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2szfehvfr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2etcclecr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ouepcmki.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2htpplwqw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cgorwief.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2lzxsdzbm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2rqmunhyr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2flnaabbp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2zpqniezb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bsxqdeti.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wtzneozt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xhrciesw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ofghctea.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2klukvimg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ielamjdv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2fkwqaqac.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2znlbmghf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lxopyymr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mjtcujym.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nocjmbyc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gucayqga.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ewguiozh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2eptcvnon.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2izyqhipu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mkaqmtxh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2uyvbcjbw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rlekdsjg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2rwymplnb.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2nrwzauli.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2qeyqxqtu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pqrdvfim.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2njekberc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ellincbr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2bmltdzqk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bxihedfz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2cpmlssxv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2kbnjtswe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2fuaaxzoo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xyhrovvw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ftjzqiov.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ldlnadub.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2lgmiphaf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2nypitgdy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mdpseqfm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cxeucnow.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zrtorxgm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hwxbwjng.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dxemcnph.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qjzwhewa.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vdlenjld.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oijzzdsw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ydjepjrf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ntehmnqj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ojlprmzd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zbabdlfv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2auurbmih.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fqvguozq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ezmwbtud.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dasmfyfo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2rbbfatdh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qahhxdeq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wipragge.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2itxhvwmx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hvdazhde.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zupdudcb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mdhqppyd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ibxfbldc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uxsmxheb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2rdtgsvod.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2lflvctbg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2carakcrk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2joasezgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsodxhhg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2binbvxxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2muberive.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fyrzltdm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zpmmnusm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2pdwuogyj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dfkhlhhn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2axrjpspt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lmpboytf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2haymvpzd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2jpwwtnkq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2phwponod.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2whbbnczy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ogkhearz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pibucnyh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uaimxmqu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bgypegee.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2evqpxqsc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bljmtufm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pchglcmn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ixnpxvgx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hytvlowm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjcpfkb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mwzoijgw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jxvxigjh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uzlcpzrc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2aaosetmn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2meuulfjg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wgcrhbdt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xhcmtutf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ssuswhfv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2txbiudcu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ihukrgiq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cduoryew.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2oirgmcit.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2lfdijsxk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mgudmbce.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wtyjsppk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2bptdoefx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bkexlmqc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jflcsydz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ilibquiu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2resndjbz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hgxotftq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2suytyvzj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wogswuey.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2cvllfork.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lgfvjbfb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kmdghmym.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jashjjqy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hwgorwjn.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jdloisxl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ixhsnlyx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2emlxnbwz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2oivtphzr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hyzmrzzv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2txycsifv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mfozoddf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dfalnoaw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gpnngdjl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2evznvxlv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2whnennwl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ovauxwco.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2otiknifx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2erososiw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xhpowzeb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2skavwgyf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jfnzgiaf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mqxhqdou.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tgzzwjjx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ssjpbesl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2wpollvbl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2xsqkhqty.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2atezxolz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rzvodaes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ciwdybxk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wlzumfeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijorhnxg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ifliuhsg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bbbyykmq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vqflfwqd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2spouifjh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ltfdbqgp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2drvnmayv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bsyxqtkw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wgwgnash.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wrmxjxgy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2yuafpboq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rllgyrpd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bxeatzix.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2drpeopab.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2oxsaveeo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vabewaks.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2odjchliu.html


<!-- 参考信息 -->