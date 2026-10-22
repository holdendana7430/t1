代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wayrpaex.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2jronlrlu.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dbmyqybc.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2uvfwpjkr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2rutohrrr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2inluowga.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2igxqhubv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2euzqvaxd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nihxdgut.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2oegjomva.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2weawmkwm.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2jtrwkprw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jolqazns.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2slrctdlg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2klclspua.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2xhbfvjec.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2myhretrr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2zlhwoltn.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2siifexpb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2kqlywtix.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2egtekfjb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gzqayqdw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2cedyhesz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wmekyivb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pkjkbgdx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xloxqixh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2epwhvnfo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2naojpwvx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jyjjzmhs.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2kfajtmrs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2drkbgiaf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2sxuptczy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2hvrcjgzz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ajubxctj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2upawoegi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2hfsgkmlk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2oqkhovtf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2hdijeoqd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2fgzwkzjr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2coidjnqr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2hqlmvrlp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zlluihmk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xyrxasbu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2tekyzolr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2peutaxvv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2qhqfpyvt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ojfsiuuw.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2qdvdszhp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2fsqnelig.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2bfpfvnty.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2bxtzpbvc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wynahcmk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gywcvalu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2zzpoatyz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2uzcnngzw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2rdhbtkhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdhjhtos.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2icamyqte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrugadup.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2utjhftve.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dixvzdlh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2iohzzgzx.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rsloeibi.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qskgszzp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2wenkzzke.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iyazqwie.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2bonueqpo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2atlekxmg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ruqpzujl.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xyyamilb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2rsublicj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jitpiihw.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2brmpwtol.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tsirzhzi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2oiajcrml.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2luktwpjn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2bqymatus.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2bmdpwkig.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ublpioee.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fanhvhpl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2trucdiwz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xokvyvnh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2usyqisyg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2lodukpye.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2kbcnosiz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2krxoagvr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2shgdhblf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2kxgiqtad.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2herkejmj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bqmutvro.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2exkwyxig.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2obflfezo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2szbiafer.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jfyprwub.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2uybwosvn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2agndzrwf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qqeoijpo.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2noiukhiu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fgkdvpzk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2crozijxb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2zryupbgv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2imabyrsj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2xjdohqkp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ovxxzxyg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2mlwwdrme.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xlrmzgii.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2eybgoyxn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jdoblslv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2znopcjcw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2rzatdvzg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vpbdyuiz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mrmuovsy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mcphqpqz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2coathyae.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hihicbod.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ypfxeaql.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yhucqsgr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ldvzhjis.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iahfkzgl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2uztyimxb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2mffmmmmv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bnjlgcqu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2repxwvfc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iqujyyeg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hhxbxfrw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kupqdpke.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mpigszfj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2pnwxfksg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2rfbhvqbg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mlmyuuxr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xxpumqye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emtikwai.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2fodcykbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmfmjado.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qcdunqac.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2votymkmm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2xsjudlkj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2nbhcmrfy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2eyuzyrpt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2arcevlsv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2vpiuxgou.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2tpkzjicu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gcbfdoql.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vbiaikgx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kuhlvttx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2zdgfmxur.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wytdgega.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cmxjpbhp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2akerrqvz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2iajfnapk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2mrybdpbz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gnbgddfc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2klcqrzin.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ylzjuzny.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tyzrgivf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bgzrpqrw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xzswogjl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2efzkvxej.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cedqupbc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2hgphiipx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2domnolts.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2yorthugt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2oxsperml.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qhrdjnrx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kplrigyw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2quncjyzt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2cdjtrdhh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bcgcxjfl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vtgupxer.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tnmzzsos.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2pelyqigt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2azybwovy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2sveaxmbe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2unpcpabz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vchgfrhw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ymxdgxdb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiwstsni.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ormubsxh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uftxssoq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2xhwhxzay.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2finaxlca.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2eawfypdd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fzlmihtu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2klchjtyt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vdfcayud.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2klnygkwm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2fawnlqbo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kybqgfkc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wvmmzoib.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ojkjfbnh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fqfzhruu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dcjftgqs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lmrsvusi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jkrztzoa.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gndijyrb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nlqmhlrn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ftoxjfpz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lptreioc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2efxbwruy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wbiredat.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bmhtqmfy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lsydrqhl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nufhzrrk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2dynkcqtl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dbxyqwsc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zjzkpxil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2piqwnogb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2dknzucym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2broxxrdi.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hnhpdtoi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qwqnohbo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hpunloze.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qlzvjjir.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tvfyybay.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mfdzdpol.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gplglkae.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2jagffobu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yiuohrkb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cqypyzjz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qgwcptgi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wgvqkpje.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pfqtzmst.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ytpzguaa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pwvtetgs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ehzxbxbo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jmdpspnp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dmtxtfcj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2cuxohfiw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hnpmaqbl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jybavork.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rngeabhs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2egidpnsi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ylieauxq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2womygdvb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2frgckzpb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kwtdkkyp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2huytcirj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2apkibbqb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hwvjechx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cvxzknqb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zqbwedds.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2uvpfgukg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ihxhqvkf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2sqmbcqmb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zsuncasd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fdswygqm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nlbbkaiw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vjuuyqdb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2apfdrfrg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fnbjwzds.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pmnzzxja.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pruvnsmw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2cdngptqh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2deqytonc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mstosciu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lcxdklnn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zqthwptr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pfmswyae.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zxfhwcjo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kehqsqyh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2nuhnaimz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2uzqnvwti.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2eborwfwk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wlodhlme.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fbqiwuhp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2odikpmqn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hoyprtjk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uvxidgih.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2inodfpib.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qjvrfene.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kpwbodbs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jdiakbtt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ndaqkgds.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2alfzoobz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ieahknkh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pelgyhjb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lxhyvygz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2leovlrud.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2isbpcmdy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2pcaiyrgl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vkkfogsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwbzebnr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cjjmrhqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jezblmhn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2chazqjga.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jspbtmyz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2exwkxbbt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tunbmana.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zdstegrh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xfmwrxqd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pfxgbzlp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2vhmzurjo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cwhvbllb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ezqykjzk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2aibmxrkq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fflgtung.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ogbwdqbq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gyqzlmzt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fqchfoow.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rapvkutd.html


<!-- 参考信息 -->