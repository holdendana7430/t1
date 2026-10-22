代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2muqejdbu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2bahjbrwr.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2kdzwwzsj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2rpsktbsx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2tgsnzoyd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2mmqlzjrr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2rxjnsxcf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2iknzfpvb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2xhpasoim.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2pkhodruu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fykoqfxn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2gxxiiorv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2purylyix.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2fzqkjhgm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2lpygjafa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2eliloilj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2dlqiwznv.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2wpudnpfo.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2tawzjnqc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2vbskyfpx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2zoumezai.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cbhbejws.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ymzbqutn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2biotocio.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lypulelp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ucgwnpjo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2tmftksyb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wxfusxlm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qcdsfbyq.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ivcngyyj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2muzqylgg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2gbaoueam.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2okuwcavg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2bqkptmgx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2osgifjxu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2dwtljvyl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2otylovku.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2yrcurvgm.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2jsonryzz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2copsxkuv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2sldlgzlr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2gljmnsax.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xabhkjii.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2yufrxtma.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2twfrhzpp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2ytfdzkza.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2lzkxelwp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2finbvzox.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2acufxjnn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2yetclsqs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ycyvomcx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zsmadchp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2azvsqjtd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2lcjedrci.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2xzxpysmz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbtpfgpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mefnzpgc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2tdkyircw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kekkuxxw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwlapjgy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2iwhtosth.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2pdrtfyry.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2uqmzeatc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jcjipgsz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2sbzvxrpq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2smfpruli.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ikofysfh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2sibvqjet.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2zkpnmquj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2wpeieits.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2yihzgvkk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hehkwpkq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxzpinnm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tkgzmrqg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2eauttqlp.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lkaajjyz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2lyvkdrux.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ggclzism.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2otnqeqgv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tooxxjyz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rminfbyf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmwrkaql.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2nehealio.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2xzyhjmxp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2pbpefwkk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2jldvuoxr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2adpqkwzh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2mkliuhda.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2tafrqpxi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ymgppgsc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2oyjoxgud.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2knepexcv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2isbeahes.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zjrwexjx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kwftxcor.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2amvechml.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gheyqxry.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2vpgiprfn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wkptfjpc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2drdcidun.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2bzjcxhvf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2aufyvruo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pquhyyes.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2afllyaqj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2pfmysura.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dnixezoo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2evrboxbu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uufqaxgt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2foasusfa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tjrpmtpe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nmiuaqhs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ptveqnlw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rylycdjz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2mlusufuy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lwwpjiyj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ivgefbfz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tdsmzsof.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2evewvgkh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2apjbnyux.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ipcivpne.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2brbajtwi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dupgnxhu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zzozznss.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ozgcmfuf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wujxwtgg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2htclokvl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zrmhuqlg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2exmveuzh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2xvtshbnb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fjzklnfy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pohxwvii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhhnsbua.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dqilwdxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gisrfims.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jfcksrka.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2eflrxwsp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bcbvsuhv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2reatobaj.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vtykbnce.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ydxknvcv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2oyhggzpb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2upgkjnma.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lstjotgj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wkuvndpp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gpvdnvnt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ymddojxt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fcgkovrc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ngsyllbx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jrfnpofd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2trsghcrq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2srnvngvc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2yarcfbnn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2osrhognf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ybaosznv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2gbilrwsy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2iifdnsff.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lwgxdgut.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2fcdhylrg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gymfrmuw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2pbjzjuuc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hfdakzkg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2luxzcfur.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ijsgkgkp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xfkckkdq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2imrpipfu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2akfygbpd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wfzontxj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nuayovhv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vwmopuxu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2yjenejjo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2lxfcsomm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2msvbbovx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pfnduzry.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ptpmyalx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mrdudwac.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hcmaspxg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2zyfkuegu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ssqbsiae.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hrfafarc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2owrjyfys.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jplvotbn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aufueewh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ffnycayx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ffewdizs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jhhrwtcw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2wiizvkeb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2oqmtgsfm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lrvivrnn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2oqtkvoog.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2razwgkxg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qvdkdxdc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fyhyybeb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2thkxbizp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2oolrvgaa.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iuzpqxjl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2isqgulhz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nqywptmd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fhepepjo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jvxvhsnl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2knpmlmbo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2grnhfllc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xfpenpmh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2bsxyseyy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mongqrtx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dvftmaea.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2doixuvju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcsegozb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2agajfwur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkzamgyf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2felfjxmw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vhgxxegf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mfzorygy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxczbwh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bsnxgzjo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hziaoekx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ypjcihbl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ajdqqrsi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ygbdspme.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wniramnl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pycihiux.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2eedenhpj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yyckiywq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2miardonm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bytffoni.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lqpwasuq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bpiozhqg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jrhocjou.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ectyswko.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2kmwhicdt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hbgrgfro.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cuvwktbi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yreawajh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hdobjpdo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rsnacpdd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hnbkyyib.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2qtpeyjsr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jrksgrjd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2whqpraan.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xoreeedh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2eepgiauc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2crvmrann.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2uabgrnmy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tewqzhgk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vmqrquxo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ymviwuqe.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2dyumesif.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2deszgqhr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lvahfpjy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozrrpgyd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rbigaweu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fduviqeb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jnbvjpvk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2osqoxfmo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2gnvixvji.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2uktorpjn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uspovncd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jptkhdig.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lfqdqqqn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lrcdgnya.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jluzkrqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2sbkbxerq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2okkuuydc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qdrsbgeh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ttkivosn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2qujmsrty.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xdpkpnfc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2iforvwkd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2arfpzlim.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ejohksec.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bnaemzgm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fprdowuu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qhemaxbt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2caiopwfw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yzzxcimg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2scfoltkl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2appmvxtu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xvytsxde.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xiraqdoq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2spxeblsq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2svkowtlx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2atueazmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imeyyzfy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cmabbdzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lngwvxmv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nzjqkjem.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2layilkzl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2exznxkxh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dnxgyboc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tftitgaw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fujsgsks.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ropdudxw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hoejqkzj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2znhqluqi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zkezcqlj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zhykxtjy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oczldxzc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehqliokg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ifpufmtq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gdvmxone.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wbfzsiul.html


<!-- 参考信息 -->