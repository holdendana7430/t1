代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2johvgzwb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cbxsbcfg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2qkuoskjq.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ykcqkxxo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2odxnvgiq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2wuftmnhr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2roojpwib.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2xsvmyqgk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2olvkywat.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2pgxiuexa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2girbhbzb.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2boumranw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zkjpjvus.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ihznpypp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kdwspqsw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lbakdeot.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ioeecrzs.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2lrmoontk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gkxtikec.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2aprbmikb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zrtmjypv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fgqwwcul.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2jmvparsj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gahjmuvd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mwscjzxo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xfjjexup.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2xkevuvyc.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ostpzhvs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2pmoeqgxm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qjiuvgqe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2oapozpiq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2eqmohhvu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tgkiobmx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ltuarzlm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bwkmfuhn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2nadjobnq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2uqwewaoj.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2gcxozluq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2gkjckruy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2owdhbuir.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2mqtnrirf.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2kbspkhyf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2kiorbbvm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2viyebhxm.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ejmiluul.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qrklymwh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2neiruboc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2wcbdtxdv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hmgyvcsw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqkzchni.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ttrrawud.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2esbturnc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ctfdsryh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2pjqwdror.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2dpsuxmia.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2obayehio.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2camnrfle.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ngwyzove.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2evasybcm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2slenghyl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2cqaujozk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ujzjiaze.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2oqgsmyuh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2amxbsaoe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2zrrzcmmt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zxkulxft.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2uvpgfrdv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2oukhrvnf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2qctsudid.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2wrjfoccp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2uogjjfwh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2hnydwozd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2grnnhzxv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2agezfjqd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2hpjnrocw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2uurfhusr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2eclrfqcm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2bauecyhd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2qjmrbkcs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydryllcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpkunmeo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2wgoxrtvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swcnwwdx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lqmombop.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ifanvccv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2arqgfevz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2cdojcnlg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jeborasu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2zarjnwmr.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2znwdgtfh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2bwopntcn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vmzfrgdy.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ugpwlxdj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpjuknxe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2kheevpjc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnrnnyby.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2odnxxerh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2anmrmjqu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mxvyvupk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wntqezhc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpdrvabt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2dxvoytgx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2exbbnhmz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2keaxcdug.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojinpckp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2utrutmwt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hfhyrgus.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2nqbkwhqf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qnswlofp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2kposwvzm.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2bcqulgyc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tpfcvslz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2eswvrjqx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jisxxrwa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2depmywvw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hjmrtftk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mrfhhlku.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jpvokqul.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rynjwxac.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2bvejunxu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lndskshp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kopqtpbq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lvkahzhd.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vyxgpyfv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2fgohnkxh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2xowmuiip.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2hmfabigi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ahzkegnb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cigcfbgi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hcqfhexk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2butvtfec.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jqsbdxwu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2szkoseju.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qhxlsxgt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mvqiduxe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2slwbzfna.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ysluqauv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ooypmpxn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wqlmsagl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2pdwruyzj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rpgxsuvp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bztxlarc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yaohwfhp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fhdfapqw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nkkayivv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hiritxzn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2iozwxjdh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2otwnlzxr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2hygpxxca.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dqbnwxaf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2nmljcopm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2bypjpjil.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mpunhfix.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wqfjkjea.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cmfkhjdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aglrrzoz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ooitkknx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2badqmfhp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ghedpsnq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ceflcars.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2widvyrne.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wfmfbmyw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jfbxfuxj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yzquxwxc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fqsxcmok.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2lnklevpj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2sufchxnl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lnkghlkx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2uanxhcha.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ovvjvsbb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rajoobrv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nvggwsnc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vmaevyyq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2omywhsob.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ftbkndcc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2jueochoo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2sqtnftvo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2yqppgjua.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ceunkgvo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jtfafsvw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wvhkugqc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ikxhsqol.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wghrmsld.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2laxoqkav.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2egovteal.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2yinbdzhg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2nbowrvhg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rpmkkjed.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kampomas.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xkgolpqm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ftkynkcs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2nqhxbcwt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2txsxfpwl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2kubbnmxm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2sdpzfegv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2kxsyloiy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hyyysycg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2thsyuddl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gazmchfb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2gpyonnkw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2lenrsxtn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2sblqgnmj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iirqoeix.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2gydbjdtr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pkaopgpb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ezyiijil.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mzeuchys.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2inbbhvmt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mxhvctxo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2lvegudya.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2yctkuzuz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yoeumzwv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pykqziby.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qyqkyzud.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ltfkjkqn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dppvhrff.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2enfhwnlm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2yrzgrkuj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2amhzvnnp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2rldfzppu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uupdgqgg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ehpancro.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dbgzbalt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2dktxrwgb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lettoote.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2syrdlgan.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2cxmietvz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qlcglkoq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xsxkrvcb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xpsrismr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrkfzmlb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rprzuneu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysblwcoh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tggjspdu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bqiekiza.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qjmatqnb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2juelvbke.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pbodimwu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jbuimdbs.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yyxcvsom.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rzwfzpav.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jlcntrot.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fcffjvip.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2klquiiyk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2iohxdxxa.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qvvbjfgf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zvlwtjdt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2abjodcxh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2byxidejn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2sgdswpch.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jqcguszb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zpfkyejh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vchhbozr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2yewlslsq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2afscvnpq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2foxtwcgt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kcxgvcud.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ieahjrfb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rnnpywpx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2iazpekkp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jhpfnhlk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hwvlwfdu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yihiewxu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yfdnjdqs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dxtxeffs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ejomupwn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zytqnbvi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2qpdgpdxo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2aqrgownm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xdnnztbc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wdovchac.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xqeyhatc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vatsmppz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dwhyszxi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sgxyvrsq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rmgtsqkf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2fvonnwrc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2birdllxq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2txgifqsy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pozvfxvl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2vtuudtcf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ynngrbjn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nivhohvk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lmkzhxhk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2cgeugjxh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lmdzujni.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ormoqfyf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ptnullje.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fxsrcqpu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gqcpupup.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pphooppz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kjejrtal.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2brapyxgx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xwvvgnje.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2omjifsmf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xrdcevtw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nykitpgu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xvkahjka.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wbtyzthm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hxcpwcsq.html


<!-- 参考信息 -->