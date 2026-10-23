代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ogqvxkck.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3wpycabfb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3mvjervcz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3guidemct.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3bbcsihvy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3emqnyxzp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3hpomsgaf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3zsptxwvr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3bpswxggf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3cslngogm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3frmbjdjh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3doaoskdp.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xbenzjcl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3fommvuds.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3wgpsoyze.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rbtyhqnz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rlimpfdc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vvzsbzgt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3szjscdem.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pqeninvt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ztjlswkc.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3txnuonry.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3oidpoiew.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3mbcyqxxw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3eiacapcb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3dtejeots.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3icikazez.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lpbsqgqi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3oyjvdqua.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zszkoouu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3clitcejz.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3jxgnrxza.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3cvhgojne.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3iopxmovo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ggjpbhqq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xcvdwawd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3wxjudjut.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3aimtvrbm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3kpxnmecw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3efpgobjc.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kytjwsrn.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3vixaydmu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3vmpsvlry.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3pfdtbwtd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3zznefatl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3lmyuzqzk.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3vnnsbrsn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3clbgalqd.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3xwziwklh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xavylova.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3vsrikzff.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3akltryir.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3nmxpedfg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3pmorjthy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3oanuzvbu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vtwhsqje.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3umifmgtt.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3lxvbhxmd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3glyfviut.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3zktcyvrs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3kwjmjlug.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3xjocmmfk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ndaaacih.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3kdqwvvkq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3tvtzhrzg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3qrgzylxy.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3wzwfgoxi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3wdpapdil.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3yimvhgmy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xhnhtjwn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3eimqaixf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3cbzbggcr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3cazfxpdt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3oitqpwnk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3tdltasmv.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3dnfvvqjv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3dgzwaypp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3uzkhswhn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ndcqnkip.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hlebbsgy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3hwpgzwps.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3piopyvjq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3eerudeek.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3dfmqpero.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zluiqxfn.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jcvmkywp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwxptjzl.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3whoqzvty.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gmsmroci.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3cfkztipc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yxnxzvpj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uspdhyjm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3jabhkmpc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3gzireefv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3agniwoym.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mtlyolqt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3xaqfzkrz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ykjevigc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3drakajor.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ijyyaemk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tmlwtelp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nfufyeus.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3aizwfwtt.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rcnbvkrc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzawtwbb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xfvurlgu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wvgincrh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uzzxfscx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3egtpfmlc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzzhlahy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3teawzptj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3bqvkfkef.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3pmyitcbw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ygvmpqzr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3axtwwfiw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gnulbmsa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3rynbiymo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3apqdymqi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yedhujdq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ziepkomp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lrcamhbb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3dsaozzik.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3abelxuxb.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xzfzithl.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3denvqstr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3flzkwitl.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3srospxea.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3otskjuhe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3xllyeldm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3dbgakrwg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3zbhtybwk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3pulhnjlf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3csavpdkh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ryxkesgr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3yqdtvnvz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ylgmguer.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rabdsnsy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ueofupsg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fzidakre.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3aphcncrg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dcehjsnc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3xjfrkkha.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3miqccqzv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ihqffhdn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nuljxgih.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dmwkjnbv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zxuhqnoz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ptdktrzn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tugllfii.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vvgjugxs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3hzmpvftw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ahitpjoo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3jqsdpmbg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iwzwrqpm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3whsrbkhs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zjriszke.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3cddqikqq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bqfldmmu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3buqrpjox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iusdvfdb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xuyllfni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aiustmcf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3rkhkoaye.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3saiqfdiu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3jzrfglqx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rocbdwjb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kwsttnlq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3tclsuigx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fxiyiiwa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3gwxaqasm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3xbrfxndr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yflbnqyn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3upagxkyl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3uizdravj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3yreeshjl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lhcbssfm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nruizpcd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ksuvrpfj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wcagtipi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kipvphcn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3vylaqdqn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ypvggemw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3hydftnbf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3aadwqntf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3unvydpgl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ivgmpcrf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3oxzcnokm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3knmwiaqj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vsvqbvvh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3xhjuiszu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vdecblhj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3afeaawvb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gaymnucm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3iflwtwfr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vemrewpc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hzfpzesy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3widwghyv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3xowuixtc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wxmbpnpq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3dwpkulqp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3gplnsynh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yzcwogov.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3agqievar.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3coalyhgk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3vwgosshm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3vtzaqjnb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3woxulykl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3gxieyknt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fzogxnbw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3qbygyddy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yvrpcopc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jehvqjxp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ckqiwucw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3oyjxwkql.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3byiecxyw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hiydjvkt.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3njvagjja.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3rqusabuk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3awtgmvxl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hfoesgsm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3trjwhssc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3rkzbksrg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rkirzboq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3sgzoewal.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tfwcvsga.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3avcuvaeo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3arhwnxcq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3meopzwyh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fuxktwbn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uuxpxbwz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3obemhmbx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3moxqiikj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3oyldeflq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3icajvkrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bckrmacn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3qlqwyffw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3argcewdw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dbthjawh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bzuqmrdy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jyjfpnns.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pvnbquui.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwpqbwrs.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xipynbdo.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xwldjeds.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3acfzrpbf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zaidrukt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uiubbtmn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jbecmbyt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nexxqhns.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xzppqgwu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tgfvykwu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hewypdfo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xtqbijpu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3klqabjml.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3odvcuyrf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rjifulan.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjzcdcd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hjcxthwi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3emctdluf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wfzaulrq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3snkhwisd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vajebgzo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3uipmgzxb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jhuypiwj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3btyjbxpq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3isgbnwts.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3funambyv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3adsqdkwn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3usmxqghg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3blostqvr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3elrnhvwp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jcqfxotp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3htvsovle.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3glwiobtj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aamvdzml.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3osbmcgcw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vtdktpnh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zrccgwgw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sepgrauo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wowyywdz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dllpsbgv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jrdmqwem.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3luwmmoij.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ttcpgecn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ursxubeq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lwbrfxsm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mbqqjhbz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mrxsnqte.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3givzbykf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3qvxfusiw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vicqlewy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uxtastuj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3titkzczj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3muwyiqvi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hkcmxgih.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3evlzdfrb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xlyuxcly.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hijwfhzj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jsfesvup.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rpxhrgqf.html


<!-- 参考信息 -->