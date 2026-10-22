代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ptbutxsv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zvhfpwwk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2qqzjzeiy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2psvfcvlk.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2yxgzemzi.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2fkmirvdp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2tcanbwvn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2leahutxg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rvpfqybx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2wpqmrmds.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2blhsaorb.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2evozrnkn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2iemkrglw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2gzdoyjat.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2wxynwqmq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2aavhpvgs.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2vjplkuft.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ouqlepbm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2cviixxjw.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xkjdkbuc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2swdeagbn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2setlncbc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cqiikwox.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fwktykwv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2bemcieta.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2brmfrjel.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2uaqdcgen.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2hjgieaeo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2bzzhwoju.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2godlndtt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qiiwvwca.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2dulldcco.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tmimhvnp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rddanlhw.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2uvqbatrn.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ewfwesjw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2mnkluqol.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hvqzxpiq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nsfsdqyd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2slcnzmqc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2irlndsqt.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2aewrzjpq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hmyqnyln.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2mtzetfnt.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2qivhsvep.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2bovgswie.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2qbvelpog.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2xnltxhxa.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ltkjnwsz.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ezavyzly.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2fhkwaedm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2pbnjupzm.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2geuonpwe.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ozthbxex.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2tmeyrsjd.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qdtsokjg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2upnufhyw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2degqccvh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2vriymdta.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rnioxmdg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mnhcuzih.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2jmkjslqo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2pfenlgyh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2abnvwhjc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2vjdcugbl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2btopldse.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2lfxoxftn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2qrglxnwo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2uwrwlmdf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2kzspjdzp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2havzymoq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ksninmuc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2rfsmvzoq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2czvexuuj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2enyjrtpr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2jhixilmd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2mcyffxgs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2yivjrgsf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2trqcrfic.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2remicmfb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2qfxsehey.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2gbrqcpgu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2kohcquvc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bvohxwrc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgeylfgz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2wupdulfb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2qikcnfrz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2myglwhse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isjaseao.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2zdikudsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2droyyzcy.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vggdmxnh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxpgkvk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hgpfdhhv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2aikkwcfg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gnlegafd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2clgphobq.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2rfcxqlig.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ukdetnsn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ixhgyncp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2eipibhjv.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfropgut.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2utcdpqsj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ecxgeubo.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hhtekkag.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2iyfnzwat.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2frawlnni.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2phtltqzh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2cddwmfay.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2wnmpeaog.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ykyroycw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zhktftgz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2nejlhklc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjaamct.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xhhicsfm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ithxbjqw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hetgdlpg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ocdoxxgy.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2aherottu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2umfxjrwf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2jahnwqhv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pguvikzf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rplxrsdn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sceuwdbh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rhinemif.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xycqnpzd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2capgdlee.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pghojcdj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mujhpbdd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2gndptjdx.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2euhtdhks.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vunwvstj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ushzgbnu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2wxwaqmpu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rzqrrbxr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2arubfvja.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2hnqitaxy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hjxlzbnc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2qfwhknqs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wiasuubx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2varoyrvi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2umnjzrsh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kamtzjjd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2smyxpfah.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qgqkohqc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2evzaospo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bwudypoc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2vycxyzqv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pgjcdfjr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rjqkmeeb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fxijcuip.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2naonhuxe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kuwsxpqu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mdocyehg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2tddsuqwh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zujfwfyq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bptlvldq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mjqxlcwo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dyjxhsxk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2fegbqbdv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2hjdpwndl.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2lamtirvl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wskrrjqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uounedhx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2qoozygxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2soxiqnmp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2iiuqgziv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nwkscewk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yvizwliu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qaqbkafh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqdqryb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2axcfexdk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dcmljmok.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2lqilynru.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2sjpugiyx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tsipnlzq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xjuzqdqm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2zbnedcah.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tosmwpko.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qizrqfia.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2pityzuxu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2nbzpvgey.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2hdancszs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ervbdzqx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2qpvoizxn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2fjmrkgbv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2qcaupfzo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ovwiyyjq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hjctokqb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2kivtwohb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kxrkwari.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tdfnujug.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zhslkbjf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hwukniex.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2gkjxifoh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2qmhqnwhr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2trjqhjsb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2coibaltk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2omcltqyt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2cjwkvgaj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2byzjrako.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bqbmnbjz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yjguroal.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yuclulgd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ibhslnwe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2emilabrg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vgtlkhjp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ittxkvwx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hitstgjh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2rbmrkhuc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iekxhiwr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2eraervfx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ivjtfofi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lkemiakd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hycouzde.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yqbxofln.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nwincszt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2fkqehyrp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2rojzupry.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2umropitn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dujchoho.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2tqnohnkr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ztfqnbgu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nedqpiep.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hcnzyojr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gevsuitc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2poiveavj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xgwcmlij.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nohqyggn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2eniwxjnb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2imstxkaj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2feidtmwe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bfpipfpj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2odydbojv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ocrdyoye.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jnfacoge.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bpcsubjg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wwrtwcxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdyiqrsc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kfwlrdpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfxqazwm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nwarbwae.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uegztysx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bztemmzq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vhefdrtm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2idposcel.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rqbgtdnh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gxzrrooh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2bjerbdoj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fbsxkxiz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xhzkkfjk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wixrreko.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kccbngtz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ztdnihmr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rfzczoea.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oekgfraq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xyidvpww.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2bifbtono.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yuznhpoj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dujdrwoa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2etofhrsm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2fbdoqdda.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qnknctav.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gfuwocjg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2juufgoeh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2njcqhuoj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2aehonejl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2eaixnbfd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2flaufcya.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rcmfnyha.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2kypdfvzf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2spkasxye.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2feamkfct.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2suruaiaa.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wteoavlm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2uqooaccl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2elcwveej.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kuazlkqr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zamvdsmo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yjcmexah.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrmhakrl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxidgpnr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bajawkvi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnkdzeyu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2sdlfneoq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wmxqwpuh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fvmxbqpy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ctowqrzi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2edrfsmcc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nzzceqle.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fqpwugej.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2keyrutee.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2onafdain.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xltorffr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2iffbilee.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2cffxqpql.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2aewealxr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2omeavgfq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ksmmrokd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hlsxypsm.html


<!-- 参考信息 -->