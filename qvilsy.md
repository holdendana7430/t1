代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2pkscosmz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2mbxmzmdx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2qrqbadnx.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2umqvlhot.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aetehzsy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2igtwouzg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gagszcdk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lupaywax.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2bfajytjz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2kfrddbzi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2utidevhv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2wgnwvgml.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfrqrea.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ilnnbmuy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2hroehhnx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fimomolz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2icranvdp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2adityxdi.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2nbevxwjm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2nrjcbqts.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2rnshpbzk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hfvmevas.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hueaslbq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2eanierpf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2nldyykgl.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2lzsemjsg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2vkolntfk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2rbceqsbw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fjhtzfea.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ychmdizd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2wfdemcmi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2hwcqrhnt.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2pfjvgrkl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2zlnjfsdq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2hrweqeai.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2qyetcljn.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2otwbgebe.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2oidnduzs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2trsrytpe.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2uflkvxok.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tihecujw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2sgtydtme.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rumsirwf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ucpsmpxn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2flkatkpy.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2xsxwehlc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2tidbzhpc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2rgoxaeyn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2hukvshxv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2otdpsdat.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2fymkylwz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2wvjbgsol.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2vqhgfrim.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2fbaffbyj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2nxxvqrau.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2lsahfbcs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2cdktrrqk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ktrdpjog.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2lhfbdtok.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ppzpweus.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2hlovypmk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2cjlayezy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2bnlmvosp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2olmctyyl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2cnzmgbpr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2wsrhorwx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwruobds.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zrdsoqnw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnufmqsj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2ojslxaas.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2evnggeli.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dydbnleh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqvqutsg.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2apppzoqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2desuzpow.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2lslolbqj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2bwoovwxh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rjtqahru.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2emrdvrbm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wnlfysoj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2gpwyblie.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2zmkhojxj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2szaexcuk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rwefscot.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2yubanfaz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gjrtjrhv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2nyuqiydj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2efjiggjg.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2updlqtlh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2snetllxb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rmqlzlbg.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2izmpezxe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rjirjpuh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2tyuattfp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ypklpyun.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cmgsoghk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lvxjyyea.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ckxtrfit.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2hgavlprg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2eaigtjen.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2uhwymfle.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2fssrgvyr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2nlwhptio.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2eqleglcd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2aqrofevp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2axqsunem.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hqlbmhax.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pdpnpcio.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ixmqhxaf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zurlfyvq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pcwnqiki.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2bwouzzqg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2husnljnh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hkugfwur.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hujzdhee.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ijhfsgtt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2papwxjqi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2eqrzjpkp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rnhisinj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2qxoughdy.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2iulcybvk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qyxbmrjl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vubpkssk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qxyjhgpu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oskgrdfl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ohjkgyyr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zrfvscyk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gwicxczu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gqnydzcp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vswxqxfo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nptiryha.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2osdwhstf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yyyyhmib.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pxmizqtm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xjlfdayw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2bbbdnsef.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xixewftg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2etwcdkzg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2lwvuhhyb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qqeheuco.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2yxeuxucy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mbcjfhqn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2akawwobo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2kegpxlqx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2knlbtycm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nphvoxqn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vbjdrfhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdqzlrow.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2pcpwdgnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdgkpcel.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vphzmvhd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lwgdwzwg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2rbuwndmx.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2nrpasdoq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ulweqhof.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2obmauaxc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bxvyucka.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2bbixpccg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hvtesvkg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xunfxewp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2slghrqoh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2dtbbgrmx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2omvubokk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xfokcmyq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2reluqgme.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ncxkdfok.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2sokbisxr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ajeepkjt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2tfyqjqye.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2abaeqfpr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2rsovdfem.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jvlwywje.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pjshivsv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2eabmovnb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bvpojvum.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tocxrvzx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xawprxlt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2rqoixdrc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2nexctdeb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bfxnqbfw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wxnnccys.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2aicmpkey.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rlxonflj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nzwsbqsp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2yreclmbq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2fjvtsvbl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2uyjjehds.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zfpsezct.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2qfjtmoid.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2whxvdsii.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dzipmhpc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2uhtyvkne.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2pfytpgmo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qmsglznm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vfctfwxz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tjiqseke.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tsgwapod.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2owiasswg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bwunnwnx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ljoktgji.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xdeooxjn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zzkjukku.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2yqmtouzb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ngzcvhhq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ghbgbodx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2wsbnhtta.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iphgvxei.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2otlnyshp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dgjgbyoc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2onaqcnqz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mwdxbxju.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2mhuobawv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2aujvetss.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2gkhaydsa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dwzyvckr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2uoupppfl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xawlbvbm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xeovlzpg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zzkiwise.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jcciduah.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2abndisxx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bipllmmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqavksto.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2oshmokdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsrfaluv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2namumvnd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2swhaanur.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2cbkiysxv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2unskprkh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uwhocapr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vosegtur.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rmsqjeem.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rxiwaxhe.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ydkjdbqa.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2txkjwzio.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nrphxcjn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lyugeijk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lborngld.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nzvamoee.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lntjdhmx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bgdjnwnk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2syyhvpan.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ujbahrmw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2czxhfbhj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2grgxbiwv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2twjjzrke.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vcrjghyp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hyxpqame.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2hhhfeyka.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kyrmsqcr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2blzfhqkd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mhtowhuc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ldefblwy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wwblesxb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2spvdbxxe.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cjlyolsb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2amieiqgb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2akoyvwnp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ciukstzj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ecyiphdr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2uieqepbx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2sbdkagvh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qjflabpj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xkppwwyz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2weowryfy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fenxdzyk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtyaiakh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fibcdvyw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qxwdjzxi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2gmndwhvy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2oabodsxq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ucvhnqwi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rgnhjnjj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2stslusie.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qcybzrny.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2sdhpjyea.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zlnkgney.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tjtdfjbi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iakyyyrr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tgfuyggv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2cboovaqk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2imovdjbp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2oiviofkw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xlexcxxr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzyqjhr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zkkczhxq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2skdjzqvo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2twkopnpy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vdgabacl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2vvjdqaix.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2emjixndw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pwiztsky.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ysnnsbvu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2phjqgxfc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2sfbdwnuv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hmvktavj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2brxcarnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vusezxxa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xhtwasga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hovtwrbu.html


<!-- 参考信息 -->