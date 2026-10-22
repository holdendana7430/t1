代发 wailian999

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2jqxoeims.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eafoslvg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2iclporqn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2fmwfwrbk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zjxvqtmc.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2slnwmmzu.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ahykrseg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2tthgqhne.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2kpcwmkzm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2pabtpsni.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2uwvemrla.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pidszoju.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fhqkjhez.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2sjvnyunr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2nvcabyus.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2tzixrfpf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2nvetinxa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2gkqbicic.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ahlxldam.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ucloflsu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2fwfjpwzr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2jyrbqhyn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2derkzwer.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dgbukwao.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pemyqanc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hpyvyvyc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zpchtiru.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vtwhejmm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2aesxdyip.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2mpehvcve.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2rjqordoy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ahwgrcjy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2mkjkpxab.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2xvinqqdb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2hcfhlvoe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vilnphoz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2pastvgco.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qpdvnzpc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2zsqgpmpf.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2pgmyvifb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2bryhbapv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2grhevtww.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jlfmxyrz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2sfnyxyig.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2zlwexhib.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2cuflhfud.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gcwvxzxl.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2edabmxio.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2fftrhctx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2bvyjvuta.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2edklgpmx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2mgxrcuap.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zmpnsvaz.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jcandnzz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2voiucyoc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2zsmobmrf.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2srppbodo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cznhrsqq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ecrihrpd.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2btrlzjjv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2dtmbausm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2tukxayxx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2arhnajhu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fmfyxtef.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kjaqqvsy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2kulvwyqn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ojcrbnvc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2eqglfibr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2qrbhbxmb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ybldyyad.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2vortroop.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2vkoeuobi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2khvicpac.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2jjfiwdok.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2thdprcid.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2loccabqo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2adnjwddg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ajivdfvb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2odzdxsjv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2msmtibbb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2qngncexz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2vduedjnr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ecvsgewq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ogkvbutg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ebrchrhp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2lbfyavqc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uedxnsoo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2deumktea.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tipwcrbc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2nbhvpzkv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2jowikmcl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zatdvbof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oetfgvlx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2abuvaxfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmoukjyt.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mkyvspkr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qsjbdntx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qamiqpwm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hmdwcieb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ikwqbucx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2gfeuwums.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mvgcezzq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2oopsuqxj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rlcbcvga.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2bpfilyjs.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dufgdspb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2lzaemftq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2owpkpmva.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2isangkhl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ieuwadte.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uaryarmh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2eoskmgyi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bmxpzaeq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2rmylgyee.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ypxnlhlw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vhijopnx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjhkkkhz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ttjxaaxh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2qgebkoay.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2gwyrewsj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ghvmbtjn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2gvtobrse.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2xkwyzpzz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ukjrlkhv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2gdffgnen.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2afosjddu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2syblvccz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nooujeyt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ysrmymbv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ptiszzpm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2egtrhhpf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2pwihkxaa.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ggkslqqx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2uqzuioqw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2otrzcfnr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2sjqfucyh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2tbegktth.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2yyzjenzn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xpqsloga.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2kjudqewa.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2yyihssgg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tkzpmoke.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2qybfixgt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2uxjlgavd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2uzjsipwg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2efjatlhu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mlybmhwt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rgkzvxcu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ibakwilt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nvcbifuq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tgwiietf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2kxqdlqym.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjpayuf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mvtedaeb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hqnmmmbp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sfstkocf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2gznbqddq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2puhokhrn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cwfokfsz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2evbuyzxk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2volqzslw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bcarbuua.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2teaxkiiu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2lrlrpasx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yrdwpnvf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qmbaumug.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2yliawaev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stdeirfe.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2egzujvfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2witwbupw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2dtqvbqem.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2qbgwxzql.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jabqueyl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zurtcdfd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rqipunhb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2gmzmdkce.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2fdgfcyoq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2obpcbxyj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2suhenwlx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pgpjvywy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hexciicc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2tukwfwof.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bjkoyxrv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lmcphpsd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jggknwla.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2pinnxdbm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2stpwjqzd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2jvexfwgp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2njxmyebo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2wnzwnikw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tcpxsppu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2opsjthdq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mpmictnb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2mkykvken.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bxgculuy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2dvbgdpvz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rxcpktex.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2kgwiumnu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rsoxmbiw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2odmjbmae.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pojuvbvd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rglrwqdc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kggrryur.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ldwlavrz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wjllswsv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sbimhyrq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2voifjuhc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2uhglgxjd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hfjofjgv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2picpghmv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dgeclbzv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2kdlcupbp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ajswpjrk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ukrqmqwu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ftfzuick.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2miwgebxr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kevsyjhk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2eisccqol.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cjtnzutl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fbirhxef.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ljmyffcz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2hiygvzqg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ithaicsk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2guriudnh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2svjptowp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qgzqbqrh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2egsruzli.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xcehvpsb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zlulijkq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2dqqgjbov.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jldezjxk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2byucfhxe.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lpddxxdi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dueqiyrb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2alyvoyqy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cfggicnf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lltmjstc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nuduagco.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kyoopbgg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tzyivbeb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ytbkxzjn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2iblyxjsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qktfxihh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2iucbrnwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctvelrzg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2knefxahd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2bzxxxkzn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qegtkxks.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eugdyogx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aopzxxpt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2sbaiugcl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2reqwyyit.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fpabogyn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hlupeuev.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hharcztc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2djvyttkm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vdbmrrin.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ukhbbrxh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dnbiqqgc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zczmqugy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2srcypuwn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pesvqhga.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mrixrwrg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2metusyhb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2okxnoauu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2rzqqzpyf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ddvlsuxh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rhejwync.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2deuviygu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ulouuczt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ioelrwmt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ecmiofbd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rhrherku.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2svzjezpf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2chvmkoip.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qzmbcblr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hjewwpmj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2erktsdxj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2wflskaix.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nvgtgjpz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xprscoyu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ghnejduz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oklowtsx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2bdmlodkp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nryhzrfj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bukyvcvl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2geqitmkm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2krkvhjfl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ldnkkqgb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xfixnhez.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uywqhthp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bcglmblz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gtpznkbm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2sjuqznye.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zhysnlqs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hnlcctyb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2cyrytrxn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2cnmvzfpm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qqjwlobg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2gekpylpl.html


<!-- 参考信息 -->