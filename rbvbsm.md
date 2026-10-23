代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3gxwirdop.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3dcqipfal.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3jbxcygjt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3hsdtglqi.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3uwjuywcr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3efywflgs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3peneugwq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ajucmdpt.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gzeekoly.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ownxlddx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3omgafqxm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3koxzfnjv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3lassgkwo.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3wizjunrb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kebzhthz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3wseiflci.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3yfyutoby.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3qnyqxkbq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3viunpatj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3urqzoumd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3alljorfz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gpgmibim.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3yrrsztkt.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3rnhjciox.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3iawebckv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3efxehmwm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vfdzatee.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rtndadbu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mquspbij.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3vitjabou.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mnyhzkge.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ekisobvv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cvuuiwkv.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3eggkpmil.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3sqocweyh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3kmgosuxm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qclvunzy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ebpwyqcd.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ozjkpwuu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3aatdyqru.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ohpnscxn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qlynjmcw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3yqnibxgu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3juzekfjc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3peqdrvjz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3toktubrr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3rikllxre.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bpbwgntp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dcahsvmw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3pwrivtrb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3zqcdpfku.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3gpxhjkzv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3dftzldgd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3mciotysm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3mogdjzcm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qyxyunab.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ziveipsx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3lftngydg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3brtadnsa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3xeytyrvj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3itumfmpk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qahlgwnn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jtbydeez.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3eeqvmpkl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3chksjssm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ovsgagfc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3pyefplox.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3xttskxki.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3mjddxvsr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3rrhhvtbu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3lwghqsoj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lhfbqkqp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gbhztzmi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ropebpmc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ihrobvfc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yloksoac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhznmegx.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3aekxsfhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svnseeam.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3eeiijolx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ocqpsfjv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ntqnlhmw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jmwskjvb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mcvecbfv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ocugnrwa.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oqzdozpa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3smsozmfi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3bwtiwgpu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ygphfpzu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fmvaqyue.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ghvgzftr.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3njqafupe.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vecqmmli.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zidaylbr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hczyndkh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mwbmdegy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ietcvcav.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3awvpaldw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zqjucgkq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ksagwhqr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zaqbzgkg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fmbdcwdg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gybqgbww.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3gtjgxfqj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3svdluinz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3psojwuvz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3koyzpjsz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3djekafdl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3xrfwesmw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tyzuiyak.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3svreladp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ndcaryxv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3uocirizz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3deslfnha.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3czuzexzx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3buqxnzmi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cyxascwj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3tbvmfali.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3epmzoijv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pbxmpgsp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3tghgxqbn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3asnwlgzd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ujxxtnno.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3pkhbfpto.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3mdnexdfl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lqnsywdr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3femtstks.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eosjrfhk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yubrqdxq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vihhhqno.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mxkqvier.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ettrxvzu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dbblcmzi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3qyufupvk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3efaiicml.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gccbodiz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hwacimay.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lgywjjly.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhvvkhi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3coxwburz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3qcqyerpq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3apmrwfiy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3zktfuasf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3itgmflfq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3qypirwau.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ejenflly.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ojenchuw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3foxrkwec.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kgsrugap.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3amdgtxpj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yvqkkdhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umcuzadi.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3gwqmnwpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3foeherje.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3oclyqamj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3yklpdgjh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3iuzyilfx.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bzlffmlf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xxpmwtst.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ghdndjqn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rhnhzuoq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3tfvxdnyi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3vwnjnjca.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mgapchob.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qvrjapqs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3rlnpoqmb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jrrbxmeq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ynmzakrb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zffihovp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3rofyatzw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3yusflvvd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mueehnut.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3gnmyvpip.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jttotjks.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3wzrvlwrg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ilfcdvoj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tvhkuvth.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3kdhxspuv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xcectbfe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dbxybenw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3srgqaqmv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zymoxndw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3lozplxsj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mlttdzdf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gemjwevx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lelohmud.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ztvphkbn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qcxfjday.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xkwvfewy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wvsupdzz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3omtfjtth.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fwrjvstf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rryiuxcq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ovxefbld.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yqwkkipo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ptkqsweu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3lrcoqkor.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3loayncyn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3redtfxti.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3omezxict.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tosikxzw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jjnyzhte.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lfueymvs.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jkhpkzlg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3btiyojde.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3pjcjngsb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3obvftaen.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3yxvlhcdo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aqwahzcu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xcdhqxnt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lhdcltnd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cetqekry.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wzqjwhsm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3rtxaiiah.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cikhlxze.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cohhurxb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3icvibpru.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3bctisvtj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ywmukzdw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3sqztpdbw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wzvbeawk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fosbldoy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bpauvyel.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wjoybyah.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uuthqcet.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3stwixpcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wattnson.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3epgfspqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyrybgpn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3crwvrxeq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3npomjrar.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rxlvuczb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dffdmalj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jqhdplsb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wqbrupbg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kgbwmdrm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dzifephp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rgeuynni.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbfsqxfe.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3htxavzxg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fdymzcll.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kaivgggp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wsccdtav.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uhpujsvg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xcnxgrkn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3cpasbtdl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iqkaivgf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3kbzfdhkj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3edkxlwkw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ubkhqdkd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3msrfbukc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qxyrlvqq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hgfkucnp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ewcaszst.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ldmfxser.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3quqapeaw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3pazxgkjw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gakxqglz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xoigdcol.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gdqwcwgm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rwztsfax.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3tmsjrxij.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3axaoxnax.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3blkyrgva.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dzmfcysy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3eqvphzzr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cngykjou.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ompccxxp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aawiibyx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3trvnosqb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nppipvhk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3klwtprwn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xhuqjwrl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lebcggbi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kickxbur.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3myillpmt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gebzbovo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3prkwjqso.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ospjvvyf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cerimpyn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3isifkluy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qyhzaunt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nhcuugtk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3viuoegod.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kxpkynbp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xbuxgith.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kmbsagxu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ndfmgplc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ncaozxph.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wtilbmkv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3undimolv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zhcqymjo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vxdgslov.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3eibaijva.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3yynzkyis.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mxajdsij.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pgzpkmfm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3eeltyitf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3bmsixfhs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zsdozxdn.html


<!-- 参考信息 -->