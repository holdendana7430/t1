代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tjhtktvo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2aqritqvh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2uixlikav.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2cnveglbq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2dviqmykx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2myvlqmlc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zlemxqfh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xkgjsfbm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jyeyzaos.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2wlaxmnud.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2nevbgdki.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2kvbpsdpu.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2liicqabc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2imtlylbb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2qpmrxlgf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2okoqgdjh.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2khjjkjft.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2mrgcqxgs.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2bqhncuyh.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2vplokbjh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ccoqrpwn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2shcufbks.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2egkykuwv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2baqbnjui.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2gkqoekpo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ksmhnpnz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2xewljvtc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tzbtgxsh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cwrmduxc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2pcelgmul.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2fpewjjuz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ttacmqgm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2zgbkdyol.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2hewjnaaz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2zngpwggg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ypkyhkbj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2pipbuzyy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ofyasbec.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2inbtivtl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2kvaowerb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2wwmbdufq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2howicdxa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2lgkyonlx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ycikzfgh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2zwhhnixr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2hmlzexgi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ebnlabzj.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2uktwylzr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2tzvrvfei.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2szwmrbvy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2cjdihjoh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cqknoxvn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2prhadeuw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2bufptpxz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2siegrpfr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkvzagvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhxilpsv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2toaadvhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjbtaitr.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tjxgctzs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2upqdwcgg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2jogzszdr.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xltoyhqr.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2fwlacoxk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2jxsoxnhm.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dfaktzfs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2vckbfgki.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bdgyfquy.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2lxahnryp.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ipltctuf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2aommilja.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2erlrgkrp.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hiopejhh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xmzscxvu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2hpkmnqwc.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2glocmcns.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2iaghednv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2gupiddxj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lpwzvnak.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lmqakrrh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ojjmlwjy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2srpvoyav.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lfdjgbyc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2gavogduo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mgxtwsdj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2pkolppyk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2patygofs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bbokesfo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2vqnpdvmt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nvgcfmza.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vpiegqrv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2keundhch.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2aeptnbka.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ycmreifl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bnsrvvvf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2khszzijr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dmgonvnl.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2yqaunsup.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mpmicxts.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zkfcyjvp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ncwxytbf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ixbqacsb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2imausgkb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2jqtitaqd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2mqzyuphk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lhgjnrfr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2kfykwepz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fhfmhmlt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kqiqsuin.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2cozuhwwb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ewvmptcr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ykprbmvu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gxfrpwjq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2vrbeltfh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zlvxagod.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2igylgyoz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ktgdqmed.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pvfrzdfp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nudnpbwa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2osdjnmro.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2pkbdltfd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dpcgnktr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jtdrbive.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pjqbohlq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2huhhzrrj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ohpkkprc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kegllugw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2nyczmwnu.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2evbcqcpb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ciweqwkw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rjqfhwsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkqnhqqk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2vuufeqbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osdujctb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hurodtty.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2lpbyrcmu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kjczgwbr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kwegwenh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bnzacqmz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ubbpsyxl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jwthcowv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2gnuozwuj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wnmdghrk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ftptpdnl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mmxlmpug.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2rxxrqugy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tzuumlyq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hfcylzkx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2gtapanbg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2bncgpfbh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2sjtrqrng.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lxjhmtqg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ogcmxbrp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qdjpcsfy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2mjdlpzjt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2umvxxxmn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zufanxae.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2vpnfgmxz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fsnttoid.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2dcwuyxtk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ipuulqzv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2uiypdanq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zovfstrf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mpmgopao.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mqvktzxu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xfgfeqoa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qrtoindy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2syisuxxa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jejibnjc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jdylfngr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2hfaiojsm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bxxviqng.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ngxpguly.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lgtjbubz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kypfueji.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2aowlsygi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2htbmidnr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2jlvzdvky.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uwvwsaod.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mtkoseze.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yfmwnwpi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kwheliog.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nvbzepst.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2avxekbab.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2iagjnkdo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zdtslupk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ffvipjas.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2znitleko.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mahqlxql.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ckxksovn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jenhqwda.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ardhkemf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ccjruuar.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2urrkrjpu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kajeocfw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2cfmvresh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cgcetxfr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ztoxpazs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kvkdlmqy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2sfdjktmk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qrknjbhx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cpzbitrs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2npovqfcq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2txabxsmx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdswmkl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iykpgudp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etcjesqm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2fwsstnwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pauzvdqf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pvvkypyr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2muajoyrp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hwweqold.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uabvmtzb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vyquokpo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2enlzmyom.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wyngmnkx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fywxkchk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uuewhaco.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2scqafjfq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2imzkpapj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2theoucls.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bsjsramk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uossvyny.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xpcdqcue.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bsvqfpnm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2utlqrhhn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hljmvduz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hyvnsifj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gkqchqfd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ufejcnqi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nxttbvuh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wyiaqknp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pvfqmwnz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2stptdspm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zkxytrvd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wmyiwozy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2upwydbrp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2achccqkn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2lbswybjd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wopjxqrx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hosyxdpu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bhmwcmqe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tacsacbv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ktwnmrdt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2owraedas.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mbkclnhn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2prsvakab.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2eatcxvow.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2retjprri.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xgkutoxc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ckbqmmey.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifqnujxt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2wzxdcyyr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2viqdsaen.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rpxvrble.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kupzteko.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2oiaanogb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2upafbrjk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cwholsxh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zwjggyzt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hujkbtql.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2aipafgiv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2npzbrtuz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lithrjbq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2nqesxcyy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2phmkwern.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2szvsyawa.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vxzpvshq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nxxkicko.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2teiibipy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2pwqnwgop.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pntpwnib.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tpmhstuy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2bvnefnjx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2efqzacga.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2byjiyhho.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lajmkyyn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2osfciizt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2czvajieh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fwqwswsy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ukbmlmrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjtvgcth.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cyygrvvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whicpiht.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xhgojzzm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2phmmsssb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2huohgkpe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oaanrxzz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ovbxldyj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iahhgymb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkxnzdew.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cjozefik.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxcledmq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2guceojev.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qjglupde.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tklrbqhj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2solbosje.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oxypaxaf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrnwzzc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tkaslnvk.html


<!-- 参考信息 -->