代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3uaqrzoyh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3sychubnr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3rqmkzwzh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3igqoucdu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3lzbjdmpo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3zuumjbuy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zzwerswx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3veprqwnw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3zkrarcrm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3lbkokope.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3exnltlen.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hdzgceqo.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fmkigivi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fqrdfouu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dytscipv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qklznnmc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3xyvxewzl.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ivzmhkua.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3etilxaea.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3zkdorlyy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3xhipilup.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3fxocezqw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3uesqytyx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hftkwihr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3zmtjtegl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dikclnuu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3auyzbufr.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3nugtbvun.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3inqxxojt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3lcspnowe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3owqsxjtz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3gosbgtqs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3dvzcfbvr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jitsdprw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hlyfbqiy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3fngmkbae.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dnnidcas.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ssmsuwih.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3nysrafjz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3opavhasy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jepqbjxq.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3kqzvjxno.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3buoouiuz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ygxnjxqj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3lptskwex.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pvdaevvq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3xmdwydzz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3lozsivqr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mcmcbgtg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jdbnlmrd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3unacxgzn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3iaafoglz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zatdenwv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3lywoxvwe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3tyhbzayi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3yxcvsfok.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3dckgrjxe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3cflmopfw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3tfauxuaq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3wbigxpnb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3kxmbmafs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3wgjgwomr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3kntjfktq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3xypeywjq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3fjlaajya.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ncojkcjg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bbpaycti.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3egrewtzo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3nndqxneg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3sqseuabd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3yxcvceeh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3xvhnidux.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3uhwnjhsk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ujigtxng.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3efscsarc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iltoxfcw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3rlvtblck.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3evucrily.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ghdsgmge.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3llwfmtlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pximgkft.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3nhzafvrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hinuhulg.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3bxvcmvdv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vpmnwceq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vimvgzpo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qwagbmkr.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3actcbcny.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3hdavqeps.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3cgaqkpmv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3oatkgxam.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3jpncalzw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3oviypoii.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3xqunlywe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3dwfjcdpu.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3uspfktht.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xdnzwrgr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vurmniwj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kyxbstvg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3peiqagir.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ljsmztli.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xkshjxjx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3iszwlyli.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wanjbhyt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3snsnqphm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cyfznlzz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3apcfyfzq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3oulnqtki.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oudxuodu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3hkrdzajw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3vjmiupln.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ocoqzmlc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3pfumrxoi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zsxemsyp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3spgxlxwa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ungabhkf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xxjbxfdz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3yilcjjye.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xqqtqqhl.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ytjyinov.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gqubhvti.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3fjhgqemf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ftmoaqsd.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gnisqbqz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3eyyguihl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3drmlmnxe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3vbchqsuu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3btcthdph.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3siudcnmg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wsjdcxuu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3rcvflkkp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ytnmqrzz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gnhqptlg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3jgfzeblh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ctciyury.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xjorojba.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3srrcwxik.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vlvykyny.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fuuefakv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ppqxidre.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zcheljmc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xkicoehr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ozgynzde.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3cmxjahuj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xqsayvln.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mpzogzxn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dkeshffv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mtdqeuqr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tvtamosn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xjyivrmq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lybxrqud.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3yfxjzyni.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fbojfekd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmiazoe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3sqezaphd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsabpcna.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3hlaztpsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwqakafd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ghfuaaro.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3lqdwqxwa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3tnkkbkrl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zvixwiio.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3urikcmou.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3rwoeofod.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3swiagthw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3heblbrbb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tlizxlqr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ysmfronx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3usbakzqi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vuibbbqg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ucahccsz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ddoxpkpq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lhonmphz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3lncywpsb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wwsbovse.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3elhlxgmk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yuwhizrs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ncnnwton.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tqhguuim.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lmtdpegz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dotcofrs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3fkakxloh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xpwwceux.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3uogvhxng.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3chczjiwf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3mincjyqe.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fizpbriz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3xbyenkfc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wotlcqmi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ycoxbixo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xusschmg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hdzcmunb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tcvrekgx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zkgebisv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3seprptdd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ymimstoj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vijmwenb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3igmgosxj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3enithaux.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rwxbajvo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ybvaxcvh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xosbkxjs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kqvxrhsp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3zkyejmje.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bdmmyfsk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3bifjxkde.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rohfnxox.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tjxnpgih.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3etmdvbln.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ahnniwbc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rgkevsou.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3lyavbdlx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iaahmqdk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gvnjmvth.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xrvploer.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eqeodunp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jioseygq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3zimmaesr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ewetaqwi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nurdkpxw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dpeddehd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xiwkqudt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3aoepokif.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3muzxmqab.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tesfvhux.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lvmzyrbj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3egkcvsrd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xacyoseg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kfqxyeom.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3acgbxcwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilsatjlo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3layglpsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sugrcyzp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bwudwwyx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3znsqiccs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jkhmykyd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmwlpvb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dfaseiic.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3muhslmjr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wndotway.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3cxvhaebs.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qklkebwc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oorbrxoi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3albigkmu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xierftkv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ofgqofax.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sazmkeha.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3imjcofml.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wmfhccnd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3bgudtdld.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3raseanvs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jqiiutll.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3waznrysg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xjpukiyf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ikdxyskk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3phwfbzhd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3sxpipzsw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hjzvfabc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ybtngtvc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tdywsexp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3afzzdbmc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3cllyokmq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xpjwuqyz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rvwcpmdq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yedgcopp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hjjoviwz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xpoqscdw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3rkbvxsdb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3orvpmafg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3tllaasls.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yggojjec.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3oalpagtp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jicqdzxd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxfgkefy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrwdwewx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lmclhhyj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3iszawdct.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zdmfukow.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qfglqjcj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3emgraqrr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3arcrdfid.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jgvlwyad.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hqkszklo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nszlrggc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nyqfyvpz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3voshecfq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jaxgqtqn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qodtbmrj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bytoxynf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kefiqobh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ichsompj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zvwkezug.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3diwgancu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hiodnwtp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3sdgafitf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3htelsnnc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xbqooimh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3iqywwnqb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wshhuyli.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kpyfmtpr.html


<!-- 参考信息 -->