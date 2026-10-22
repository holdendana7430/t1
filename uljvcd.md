代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2jrtmfqya.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2dsavipqh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2rcyatlhu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2msamrvyk.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2nkeozvvm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2cygtofwp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2xmcsneqv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tougesnx.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fphvnwuk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2oachshfh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2exlbbznz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2srmstzif.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ttbtlmlt.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2rbuhjvsh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2utjxanqz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2pgqmabsi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2lamnjslt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hzftapuw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2chfbxtks.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2jvugjqxn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2lrrhxbgp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tczglhdi.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2tpafumiy.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2bixmpunf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2oxpjhmyj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmnlkof.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qelijhsp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gabarkzh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2lkvezwba.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2vwgpjhco.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ucfmlmru.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2oqxhuhfa.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2cqclnhkg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2vsnleqhc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2jbmilhrn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2mquqpqek.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2glhiparj.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2isgzrjjm.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2zgiliseu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2cckamfuj.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2lcchbocq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pwrzepnt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ffyvofoa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2fqqannbh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2fqnextyq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2imijxdta.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2skhdctqh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pcozowcx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yimwfonx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2kfikpleg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2jxzldgjf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2pdevmtkg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2cntwpvbm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2rfrkshvt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2xrdrkhit.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2whqcsbqp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2qixgtfcv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2slhxeget.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2kmwcdejw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2dntlylfz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2iryzshsk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2svszhzti.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ilvfwdyl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2eakjvncn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ctlzyceb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2osleopmw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ibrsblwm.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ezavnjir.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjutxolj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2sasneydc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tidmfppp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2crvzblul.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnafgxpn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2qfozrfap.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2rjkqdgfo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hwcwsvlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2heiquhog.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2cksirajl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikvdceha.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hvlpiciq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2nhzgbjng.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ksznxscz.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2memclukg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nywurkfk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2pzojgros.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uceycklg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2htojfqgk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bevwvame.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2wpzobysx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2klhcylrn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2dktgxqtg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2auznjjve.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mzeebxcd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ryfhtolz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qrfkoqkr.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2owjzrjlt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2fqgslted.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2aiagrygf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2uggwfvmu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2idltktwk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wexqunsn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rhyvpfyc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2jmlmmudh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2qqniwrji.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2jluifdcr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2lroycyvr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ffgbwcps.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2abkvrmil.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2rdzsqyjr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yltpwofs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yrbesgkf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nppcnvzd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vwkhggri.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gnullsqx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cmhhjicw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ehtsuhwr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2bjyazzfm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2jhuolmxs.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lqtqyspa.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2imcbdevs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2elomiwpi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2rwaokskg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gtqjruct.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ypakoocp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2tsipmmfr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vatrorht.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2peohwegh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ekrliwpx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2plphkgnp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mwmjbofz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kzinjnrw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uvaagbwd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wvssbzcm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ddljffdv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rggdwlam.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2bxpkapad.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rkklxotq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jmfccgws.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gelbjqou.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vhapgwmr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2apoxhlle.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tkaldznl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2rjwalovi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2qpswyakg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bnelhjsn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xqqjpwig.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gftkvpuu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2tcanmcai.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dxbggluz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vkluirex.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qkiuwldi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrkofjet.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2yuxllqhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqllnwxs.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qvnwhxdr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2hqqyzhqw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2pujhevgv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2buquveko.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rhueskmp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2rvzlffzg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2umghwpil.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vwrdkpbk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xljdputa.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dthpejhb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2eqnhtikp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ucxoxodo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vjliekhv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wvzsiaqj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wryonzgr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wsrnsxzt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ieqmgiry.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iytsvzcd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2shbjured.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2jlchcgab.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qfrlruta.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wnibcnbq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ptpqfwmt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2uzqacjnn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hwegngro.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2npqxiwyk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ojzsboea.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ogjabkbu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2cgyvtkbs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2okumvxpw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ppocjycw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ygyoexrz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2esoabbit.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2fcprahsc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2awjwhsne.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2baxvcngj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2yajrxrih.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tsromzfo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zbfurclx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jmuszzcv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2eisuqzyt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2xbvftpog.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2wolwnbgx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zxqsmlvk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dxpxrtwz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2lthlzhls.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dupewxpy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2yxyehtlt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mzlczgme.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yctljrir.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vitpjdor.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ezgjeqop.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2xyfkagxs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jxhyklxc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hbtwifcn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qdzvnsvd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vwqfqtjl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kezafxtq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wueafiys.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hrofrdsy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vdkvuonv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2yofhegbe.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fulrvsws.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2drcwxwlb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ycxrmhzt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vozzbisx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ktaetxdi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rtgfmfcf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ntvfawjd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wdmgmdvt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ztlytvzk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2anuqsige.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qudhcdaj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cdmbvzpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urtajkgg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dgckwprq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2pjcfgxgr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2oqgndpck.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2siijqizk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eyumrwpq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fqtajacm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mjtdptbj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lvbviwnb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dlvsgxcs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2znzhfifn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2slxakeon.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dlnuctla.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pfmbuegz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kjjeennp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2daradxlc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2repoqeyh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2uyuyurpl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jostqttk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2nvjyvsgs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2yhypatfp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ezdylihz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jiiaciql.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tihsnpul.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qfmjpckk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2baixumwp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wormofvx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2aoaxgrzx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ydrhtezs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2eihwmxhy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2gmbghyir.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nukchdhq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dtpzwfjp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2elpxbzpx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mdpgpugt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kxqbqlas.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2owdufhhc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tlxqddua.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gwkytiaz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wytnsoaf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ecfalvnb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cianpinv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wkubthqf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmsjqhky.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvogrbon.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2imveyknb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2sepusgst.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ylmxibsw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ynpkcrxt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cehzgqdh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bbkvmson.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wtjfjzfr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2slqfyius.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2sqkebesq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iydocpul.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bmcqhabx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2mbhmaeps.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mppekfdw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qxjdbdkg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qcwoxows.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2fjqsrblz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2lpsyhzfw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2dqaktcbo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jsgzajnl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2pnodscet.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jebokywr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rnvkktzs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2obwbtbqq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qduzmfkj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2gfpounhe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mhbivebf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dpzpyvqz.html


<!-- 参考信息 -->