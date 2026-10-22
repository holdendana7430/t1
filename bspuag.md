代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uylcnydh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wvxcalwe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2umzjwcgg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gulhmwpg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2erlfixqp.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2trfuyoqq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tecvlhag.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2pfstdpxz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2iqkporxs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2appygtks.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mfnjblaq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gcycizvk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2eyokxbmg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2zskfwevt.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2aebiiupa.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ufesdyld.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2obtxrort.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2gngrgktn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2tvsvxzvc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tucpxodd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2vxgzcuic.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2euskkmjm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2mycwocja.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2cxskwrjp.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2bvutcjuk.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2mwlntkcq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2jdvfgfvv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2lxeocnfu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ffwvfbxi.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2txudhpnv.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2udfwbesh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2iytfzthg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ysthohpk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2auwhbmjl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2qlrxptpk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nqppbmry.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ckjsklsk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2gzouclku.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vdczekrp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lfkmorre.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2buwfewvg.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2qfckpvxb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2igokafri.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2newosgtl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2imighjyx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2amfuhpet.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2sipxoiaj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2zgbhxvjq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2pvnxdkbn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2hwtoynhz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2izooorli.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2vdoloowe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2napbtivz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fjzwvwby.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2buldeits.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2xaxjrmci.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2dzdzyzrq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2jmregovl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2cfopcmfg.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2pcpxpfir.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2uaycjybd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2geyxfxkl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2zxszizsb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zxzdssuf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2mxrxsjpc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2caumqlxk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2nbbjbdzj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxxyjveh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebmgcsyt.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2rmeiyzwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vaegcyuc.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2fdmhvxsf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zwyjfqky.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2auomhvqd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2uygoinhu.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lpivicvi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2htgxmvmi.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2lcxclxtj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2biwapntv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2hthuvlac.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ceiruqrg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hitvhvom.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2raaicjyo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tqkgbtzh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhhbrmsa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ptfgxsnd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2gjxutims.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aixcbvum.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfwhpwev.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2llaqbvux.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tlnvlscu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hmdhuvcz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewoqticl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jikvbzrg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ojufxfkk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2scszecdd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2vprszlmz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2gfecjhyh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkavukmk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2wswigxoq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2jnhepzqp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zjpzbzaf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jfvosytk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pxmetnym.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jjqzcmzc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wbnfeevg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rjxlncln.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2invphboi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ktdkuahf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rvkehlss.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qsifwcop.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2clxgajkv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2bpieygej.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2xvtjvxfr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jxemsmfh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2wkrewzyv.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vdspaqlf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zzyojiyv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2qjfpdfnw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ckwwgqbc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tlpshhgd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ovtdmkyx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2phjjtxbv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rycvxpiu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2erineeep.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2knmxctze.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yzofaits.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2saqdrezk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ybkjiwal.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xvkzyxah.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yguzltow.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ytgrqfrj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vgoodcdi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ofkboecr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2prmgwajn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mzyuripe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2swujicju.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qnotgtzj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ccslesrk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2pahucwey.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ssconfak.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tyjgezpl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2myphezfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbaevtih.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ugtvrrdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hbqvfjqd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jonlrabe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xjbafwer.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ozabyhxd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2szfvdcfq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cnywsger.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2fjretaza.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ipngtnue.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dsdcgwdo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2iiszdjbx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hfazimrj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tgvtoggz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xfkonelc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xtpmqpaw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hutvpulc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jignoksj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2akgmvtko.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2uqjkhgsf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kjeprovp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2awweeiug.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qrykvirg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ztogmvvk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ojxotszh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2obtakezl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2uhdnokts.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dzqhdgdb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ijjzdlum.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nsqkrnrz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2izsgrkvb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ktbidfvq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vthfsckk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2apcltxvi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dsdyoihk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2irjhdbwo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2fdtawovl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mboprvwu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2nxxmcdtu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2sgebqufs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2lgwmrkep.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2oevchsom.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uehbbtvu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2iknhqohq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ovsaqitp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2cvvnbfcu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2etyxhpob.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mdybxsgm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zhppzztn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oclmauix.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uileqmog.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qbxmuszn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qhkcdduc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zndvtoqx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dhtxhqnf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2pdyhgpnu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2umcvkccp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2svjmrlif.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qfilskla.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mewzcozu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bqwpvdtx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rcpckgcn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vpknvmgw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tnklbsws.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2rwawgwui.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ielkfjty.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dhesuhhc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2botzwjrx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2mayvmrra.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lkqudgzb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oqsuppml.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2gxfdczbi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2nyswyzok.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pvqriuqr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2jzbytimi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chtvbmpo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2azaeibjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gofvtcgv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rsswqucz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ufrkfofu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ufjbntuv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2shkgjwqy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgkzkgpq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ymgmvejh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2igtsidra.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vpywxdnn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vaghlyxu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2txwgyesg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lhsrvzyq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tpdxdmax.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2igozmhrq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wyscbtnd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oydfcljp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2szquywla.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ifzyjwgc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2workrgkc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2iscwdepo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2aypfybrv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wksljonm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kmqgumen.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bdvsmwuv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tticfcbb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ekqonito.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2znrwdjpx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vqrkfxlj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2arqqcgfa.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tbljofue.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2slplijek.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oggbncoi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2krgbxdpe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dbivjmrg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2futwtlie.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ercgciap.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2czutqwup.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2yfvfqsxp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vsacqyor.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rimcstyf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztmvsodz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ptsryqkx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jwnhgykn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgvovyc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ptdwwksz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jtwhylso.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2tgzcvghf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yocdzlyf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xuavsgno.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iopnyjyw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cndnxdxk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ppjexbls.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2qwmbfqcu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ipbsgvwu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uampdnoz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2odqmzmxl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wvfzkkzi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ggjljpvw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ynpyyowi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ggdlrjel.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mijmpadj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zeczftiq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2iliwiftl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vorqwuzo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ldgktytd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ztefknty.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dszrqyav.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nrozgkch.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wfurtmje.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2rofbjpmt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2esppfzvg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rvinqhax.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2naokyiiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxxkqiuh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cedgdfuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drilwktj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2prkmsnmb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jfyyrsoh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fprlwxnk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xoonnnck.html


<!-- 参考信息 -->