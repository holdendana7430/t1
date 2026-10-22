代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2yhavbmnp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dkabbill.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2muxlwyvz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2dqslgxhm.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2vmjplndd.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2diikyodf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2jnmhtdcn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ipxiozih.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2plwmekin.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ihaxeajx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2eimrwejf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2fnbfqmdl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2laohtwce.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2hmxcewxv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2hkjxkpzr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2nlzdfjun.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2jiezvhck.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2oqdwkbhn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ufioimhv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2spondsao.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ypndzuzm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hvkornhz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2erbrhgvq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oofzgnsw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2rxaienre.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2rwstxfja.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mbfyxlcn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2gmhtedzx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ncxhiyeb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2dkwdkcqr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2askvaqqr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2aaocrpkq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2nmqkwwoa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dntybhln.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2jzkmeuul.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2xfzdyocv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2beidmkgo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2btfzttov.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2edqausgo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qahhpbmk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vwsqjkkb.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2iyabssrd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2mdtpbnmt.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2mgurlwcn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2jffvcboe.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2eutnrcrd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2digtqcrd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2vaiywyes.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vzndhuek.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vadaumsw.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ppcmqzls.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2auklaxxz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2xfjcmxwu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2itbqymfz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vqzjhokt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2swfzlnro.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lotmosce.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2zendwdzz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ipsmhegi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rwataqoj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2guwcrroa.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2rmwvxadt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2xeaixuez.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2hvvjoxge.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2uzsmssbq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2guvuvabj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2baziuviv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ewsrblfb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ieacguoh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2cfialvpa.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ixmdzook.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2jhaxbwxi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2qlrfraec.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jkexdbnc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2viwbehpp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2qhawupzg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2eeigmqbo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2xicqkxpd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ufvsmywv.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2eyfqdpop.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2wajjusjm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2jrmrzwuo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fvacuyok.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fwosyyzq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zlnxzjhl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ajgatnji.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2kyltzjfx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qyqojbsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfdawwqm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2vcwycdfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sskiduyx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2qsjspwav.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2iyjtgizw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mlxvarsj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2otuckhib.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cuyausqv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2twjxtfjt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2yxfxyobz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2xzohouzk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2lrbprsxa.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2znfcbxuu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2rjvzvcrm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ztalkgpn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2alqkhcux.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sckftbnp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ullplydd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hwgpzgvz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gbvwiwoq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyxxmah.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2hotmhpcg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zyimhavn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ajvfvcdm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzdbrlcp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oypwlhdx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2rbohtnte.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2qdzqzoww.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ikgstqjp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2rbcckqzq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvfcknxa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dwkrknxc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ztnhiagj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hqcuzvzs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ltmdlwta.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dcbtyhtm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pnodkieo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ucppurdv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mnyqvsjg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2yjhriqyh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hmqpgquc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wiwdvnhc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mazufbox.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dbszjore.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2fgqpjnqz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2bxdhgnwp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xaaygucu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hgxcuotc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2tnrtwmvy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vwkyjdvx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2arxpdkzk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2iwtnwhxv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tddmgafr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2pwkbwkll.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fkpblmcl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2leujkshe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2maixkaik.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2adfxgfda.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pndkpupg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2phmzulsi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uojixdec.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gylupwah.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jazukvwi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2cyybvqxr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2gbsbwkcg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jxxabvjm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zwlarehx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ugzpavph.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2hdfylcua.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2smqndlox.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wgjcxqai.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2djqeaedx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2lrqkqiyt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2kzznappd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kpjeyqzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpgkxumo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2tryxakzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acutwqca.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2fcfpwjlr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2cqndewzf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2nixnxsxw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xbfdzddn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yznmizbq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2jpqkpqnu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nvyicctt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2oihnndol.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2hhahagat.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2httbbcte.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pcegctgj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2pzmcxxds.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cehfwhmh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2prwcxyvt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2urziduwj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2kmkqtbbr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2yvshblhh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qeynrzwk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ptohdlyk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2gwmyoldu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ayvwfgrc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tzuvqlyw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ylbhfgsh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lqltloia.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jrzqqngc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2hpwtfodv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2chrapkdf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ugbjlblo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wmravtoj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rozylggd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2tirtcngm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mwxvbevr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ifytqpmq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zicqseqx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2tapdzzqa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2xeeepdws.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ryzxqlpr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2qwsgreew.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rhocirqk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cnypzpvf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2edntpgyz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ncwtvbxv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2nbexmebd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2mvaoxxgb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pokcbrnu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xhnxgzsl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yrqxpxxz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lqqciqgf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2irtmsfrg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2plnxnogs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uezcomah.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rslxuydg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2lzulsluw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2gapqziwg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ugfbdmfo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2epuehidf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ttdarijx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bbftlljn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dodbahzx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2zqpexruj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2amqcvhou.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2iufwtuqq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vyxzfuus.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hpynupoj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mffuzunn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2pkdkutnu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jiirqrcm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2izbdtxva.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2upqmvbiw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rhbkclib.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ntohxinq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2grabtxyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zklqwpfs.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mvcnnjnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuzicrwn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2igcjurgx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2mujjgwtk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vwquqhos.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ebhhiioj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mmskgbqm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hnctutms.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qyqnszxl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2kwieulwk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lochxaeo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cecclvst.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nrqghryv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rltehogy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2frwqcdnp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2biycqsqj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lzumavnd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cyhosddd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ftimzfsa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cxyftlbo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2nnivvlno.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rgkcnptr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2aysevmyj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zyfpfxed.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wlgvpacv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2jrrccvaw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lrqnngja.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2uheyypsr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2cldwmptm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wkdykrvr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ariwhvrf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2pflxytlp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oxgzqcbq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jqlatsgx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nbdmvuak.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2yafodfmo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vauvqdhz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2vtxvlccz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2tmaqlyno.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2udotaaqb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qmkvawuu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnzfihra.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvtmuxbz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrmsmbhq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uibnkhrs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mnsaihqa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ofebgmtk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2aibhpdta.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pxfaebja.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2dazgcpxi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ewcczvlz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qsttdijk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2azanljpz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2oeynubtg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2mbuzesry.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rdtwbzfr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2bypwequd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pgbxjlsp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2yfdkznle.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2aehyvwbq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mztqvlbm.html


<!-- 参考信息 -->