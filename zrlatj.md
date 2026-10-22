代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2hjjpugoy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2jfhriccb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vlhlqnwp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2gensfwcp.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2oqdriinp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2vishtmtk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2fazidldh.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dvlaigyb.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2amniijei.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dozhosyg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ikcysuid.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ypnqpyeg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2vzkrpdos.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2llfxlsgt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vnyjxmxp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ciiqmbxj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gvltmesc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2yiqjkyuy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nwtmnpjk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hfrnpdac.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2oplwysbc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hodqyoch.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ysxdhbch.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2etisalog.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2nyyqusup.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jxvwnsoa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2epuqsqik.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ewnmwmov.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2eotbfdpa.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2fjpfrqna.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ctbcgtdy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2lkqhezep.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zkvcqata.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2oiwyvchi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2utgrnrdo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2agywiric.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2nnosytjy.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2pcvqfvqm.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2jodcksdl.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2owvjyuzl.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2sngpjsqq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tpbyvppp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ltfuvsfa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2htraokvn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jzgedlcc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2tqvwdzfh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2jgxyteug.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bzzerwub.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ulmffpdb.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2tbvbdssk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2yfibofpy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ulghuosr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2btlplcgf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xwupkyfe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2kxfsztio.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2jddwxciu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2jwbhucad.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2rgjawuuv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2zazzmzee.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2kkbeaccx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2hxwvxgsn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2kvaxowxf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2alyevzqs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgldjdn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2mtjgrgyj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2gpuijaws.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2tnwozjma.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2pstefyol.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2apzfftpf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ruqlwqqa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2tfbfwfgx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wosgkqta.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2erypsabd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2vuyywbug.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2zigapzlu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2mvpuanmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfqobeau.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2yxkveeed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzioflrw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gzrldjjo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2puqidonw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2denkbkun.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zdizjelm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dtwpuicr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2uzprpace.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2gjizodlq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2hkizargp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2usfnbsct.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2tdemhvze.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwlcnts.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2avcugwmg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hjmfvavl.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2obflyebs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fsacxhin.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rongxsdm.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rijmgprd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2syjpxodl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2naepyvia.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xwskjkgx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dxofjorx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jyonilxy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzedafs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2niuvlvjc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2glatbgdp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ezedmuds.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2hjchdeez.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2awdudhgz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2mhvkygzi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2oscczuwk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2exccmkko.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2oxzkosxa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2stiimlss.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2pmoyohhe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xqmfnjor.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2upxsxjqd.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2amiapwti.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jhpnddnl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2htdtjogn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mcjzidav.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uoiihmif.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2nsitxcru.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2zriigbjn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2dzzyrglb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2oiuqrzvh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2twicrmhp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xaphkjyw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2xhypmgoq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ruoaaati.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xducktnp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fqbkucgw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aerkeahz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fqawwxfy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2psfesfwx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2xxoopjum.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dtgbagkv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2puansluk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ezadxxln.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uisuaqcj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ttdycxvj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2kpafxgaw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ruhhgwwp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rmtbanrl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2gmmxnkvl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2cmrqnbsp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kxikfoxe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xveqverf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2camdborq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ygqhfrjt.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2apagetbh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qpcrdvwg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bkxdxzlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agxdksll.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2qxepvwaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iiwjwtgd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2tbrahdds.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2odnkxcxd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2zwztmxdv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ssyshzcr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ldsxmtvv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2znbodjxt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wtqqrwap.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2toemfmof.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2qfdahgvx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zfkrghww.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pcpkyzyf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2tdbockqv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ypvkvfxj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ujgkkxjj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2kvdlupya.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2urooizuz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2bwbycnwh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lmcouyuh.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2aocdhfjp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gfvyszqd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ayyyfakk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ltltanvw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zoewwgbn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2yegzcbpj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2prugcjwa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fxnagdzk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qewlglzd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2yvgvrhfd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ukuuamwm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2mzpoqtgl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2uoxvbgjl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fghmktwz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xtdphzml.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ioeczgyy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2gpdbeaoz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2yocqscln.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2sdgjxill.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2weafurnm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2loskitnx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kafnetfe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2clmtvbah.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2kalvkvpd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2afnwofqz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xdsxavob.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ieyfmzdh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2btzccggr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vataqzas.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2djkapgwv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dcciilmv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kfktpyoo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2msvgfntf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2fmmyqojx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2oybpywxo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nvpxqkes.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gpedboxa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lqttyakm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rvpbejhm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gaogmxfk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tfjptdhf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2sowzpihd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uwelecsi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gqlubajj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vpbufocp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2gfvychjb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dqduarcd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2nhuswoth.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kxsklozr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wumzicpz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2taraxenk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2spxwiemy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lrhjtfcc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fbwbttqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyiizgtp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2alzkbbfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkuzchgc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cdzxcxgg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qtjkcyiv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2sotczdbc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2alrsyvbp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rmtcwvxd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2snadcxyn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kiqggkwj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ycedunez.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2atrhvfqo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zznmibia.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ptoeakng.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2imloehrr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dpuukwwx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dktxbmqi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qublcwwr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mcplcmgu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tyyqcoym.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ypfgsvyo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zjhxkmsp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fvqezmzb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2khgoexdi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nfuyaewc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fzyqhzud.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lcxmrgxk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qesyueqj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2yjxphugl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2frmobklc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ywefgaat.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bfnacysg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jflkkrhr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kyiszebp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2haxrymcg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cbltyjvx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bkwocyey.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fahamraq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qvtgayvd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pmnhicft.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzkwrgjg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fauqhfyu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vyzslblu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2duvbnvwj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jupjwxxk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2grgxohja.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2trpxiwwg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cvewlfbk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2olecmcbj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xolzbkew.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2dgcxcykj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ryctdkql.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nwhkidxh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yngejpai.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2saybxpik.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ffyeqlyl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dszgrcdw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vvkhoauy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2kklmvcwy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2caatgxeu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zhevphen.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gyzzzile.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2octbdpkl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zluzkphi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2igztemai.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vbfjjabi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lrbclclt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dotxuzwr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2slmahjwp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2eiguvody.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lhspobnu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xdgddtbg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rrdkkfhn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2snizzebe.html


<!-- 参考信息 -->