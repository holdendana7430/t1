代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fyuofqsb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tvvowdmf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2odykncku.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ikvdhtab.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2jogwyhxh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2qjwphvvn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fifsbudo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2znwhofvv.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2kqzpxqtk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2jipzjxdy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2xxmrjqsy.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hrfdvtxn.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2slpvcztq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gpkbqpzb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2datgsgvv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2etosvjdz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2jvhqwwmo.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2gxmynuab.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2vulefoqx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2cqdjemth.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2balcodun.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ojdbquxf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2sgaqchys.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2fjlhceiu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ejtgjtys.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2wazummno.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2drpjxozh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2vwtsoomz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2fnjesaul.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2yzfxbxes.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ikqwucth.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fsdrrrhl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2cskwiwmd.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2elwbupuo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2smbohdvu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2myhoywah.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lraxvrrp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2zuumpmph.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2iggazflm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2jpkeilxa.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2uudoerxe.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jywbgsbm.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ncpntxeg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2bdurdpip.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2vujkvlwc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pqqcossb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2raqlhdfk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2jlywzppq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2orljoixd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujrhgpql.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctnxwzpz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2imwwkpkj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ylgtsjef.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2txmsoshy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2lfezgmcq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2grmpgklq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2dofkdqij.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2pgqrzavl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2vplhlubl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2wzfrpryo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2gplvywpl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2nvnlfxmn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2rqbggesz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2hccbwtvw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2kqdfaukv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pwsyixwu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2uwccfbfc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2vpssqvrg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2umwvxfjb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2dtedvgaz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ygurkftm.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2gdlozqes.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivcjlwnk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2fbazamjo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2giflzmrk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zzjbrquc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2wrvmoqbo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2uawkdhen.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2pwjpoeux.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2qeixeete.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auhfowpq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qfiltbez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pggpciit.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2qrdamrxz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tgxmgglp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kqwhqkfq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ffxvqoid.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kiprxjld.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2hsxkngzd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2mdwmroba.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2xoomvnhf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2epvfzigg.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ygybpufa.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xslzkudd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2pfsmtgpr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wuoyroxe.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2crnpnlla.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bcnixsbi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xnoztmld.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xiwpjhda.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2rbddctbr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2zpzszyep.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wliakelv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2oeuroclo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yaqdtppn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uevszzup.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cntqkxzf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2xzbgxafj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2rtqkxwfz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2xhcqxpjr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ilhpkrll.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xvyvnmxy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2tbmrcevf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2oafgzfle.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ngxxfqyq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jitsxwjt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hveisxyt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yjfagies.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dyzyyksg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2dkksthtd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dzztcycc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2glfptved.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2feivojwl.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fyrzffrk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2tnntqqim.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2jftkmezi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2opotjftr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ufcvlfrg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2qtvrttki.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tftaewjb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jehlvtye.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2undeablo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2muoxpnqn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ouckixwc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cnjptilc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2eaukoefc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ogvbwdcd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2bxtbobmd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mvbbekvg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hcemdkwa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wuuptomk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ndcxtgkn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tdyrrymt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nhvcwrvs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wrpqngxt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2flnackjn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zvcztgyl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2dqnajclh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2mrcgwlyc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2idsnsjoy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2itunvyfz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2xzhwjepv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2jtabvfio.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qlozrigy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tvcqzcqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wagbcfmz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2txlzuqst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hifwnhnm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2remmfegh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2nxbaxseu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qxybhokn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yskczhtu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iigxctii.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2hqgacehx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nyyjncoe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2kswkslmm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qhcyqxgb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2oqemofqe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2atvukmyw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2haijdaav.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2abhglkzz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2edjhomzu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lhvjeqxt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2svsutkbm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2eebkpetw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zztibosi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xbgcsxls.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2yxcakzni.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2goztejoh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lbbtwuhv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jblzxrvk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dynbdril.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bmnbrfwt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ilbditxj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2whjsnnhy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2mucizlfo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xmxojuba.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ojmodpwx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2obqwyirt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cuildgff.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gmizgxtz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dbhuvuua.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2nuiyddpm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xsxedeco.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2tvboecks.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ivqavsqx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2fdfpncbe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tqysvwrs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ahoczhis.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2gelnnrzm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ifvddmff.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2mkhatryj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tkhlgwwj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2izldbsfu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2naawgamc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xazkaqey.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oheubjyr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zfvuybki.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nkurorxn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ujrpknzi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jeizwfpo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vbdmqnme.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xgpdauyu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2balsaves.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2icfljbna.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mbkneore.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jqosqazi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xxahginq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ygffzesd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2obdlvszx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2deqolcfi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tzvwxkbn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2xkbjvlpu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2yefhstac.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pwqaxfqe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2artmqlvk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tkssmwfq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2suszvmjx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbcorvm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2abzzymfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ioivqdxk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jxzfgkxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keymfiny.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ygcvordh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bodyytdo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2czodvtrt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fourpfrl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yvvcqgak.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2efuyjtyh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jnkryauk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bshxerse.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qwjumypz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ubhzrlvi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2egcfbtvm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cskqnrwa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2adizsthr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ziplaizv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dlnhktck.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tnnrpvpe.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ohibdtyb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2frcwbiaw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2krixdnyl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ulthulho.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pikyuxdx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tshvrpwi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eypyxoiz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2cducnluf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kopofoxt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jlhqjbob.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2kuhcpclp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2atpdqtbl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jnhrooje.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mzztmyzz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kigxnwrm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dtuqwwjf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yqxiptpu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2undsmhvb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ejxevpkq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2eamohndf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tjwayqcz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vkslrrwg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2yjyrpbwn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2opnqicyu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rtzzljdq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2brwdiade.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pphppejy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tnoyjraz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lsahehyy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pkqiajgy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2knhjlnkh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mmifqilt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kiamvltb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2utbzndko.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pknnqfzh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vrrtrvbs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2axjkkobl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ylfravhg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2keamfwnj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2mykuycxl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ocstzold.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uzcfnxpz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ntvabzlj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nyiprnub.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2utxzrdga.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2radswjfw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2umbjbpst.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tshgcibx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2baunhgsk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2alsfmass.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wwmpnary.html


<!-- 参考信息 -->