代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2milouuwn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kzsadfhz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2uqdfxmgr.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ftjzgurd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2peqjouzx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2itrdwpvl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hpacznpv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2dlelpsjc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zruhihxt.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ssiphasl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rxbkezwd.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2mnzxwxee.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2yiqpxxvs.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2iezoctqs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2knzzgpqi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2kjrhvhfw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2asydbjwm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2anxrnygx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2vpcbwxho.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2nvusnyup.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2pethhbtm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xkhfbqbq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2holaqrbq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2blkldmuq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2huqfhmjy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgldpflj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2aabomjzi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jfxixbjg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mmdpatqw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2bfnrvaie.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2jbabkudp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2qsoaytjw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2vcgxtudq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2wjqbjyac.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2cnhaiffp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2bqcwwpph.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2usnvkuax.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ifyhphxn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2qqnrfjhj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2jetadlak.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2nzmvtlri.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vhqjoshq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2oqolofwr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2qwfqpikf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2hxeatkqc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2tmzoknzs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2knvjrkde.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2wojngbnz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwbtbtpq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2rlprnypx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vobhfrkd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dvmfnngp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixntwhlk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2zgnovmqr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2uznsdptu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2quzfknzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ledxehyn.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ttppulcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpmyzdfj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2wuvxmhrv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2czyiumlu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2twdoezrt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xoigijaw.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2vzwdfvpj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2vjyyvbmv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2zipijege.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2exjcgwfj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2idsqqywl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2fprknlac.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2nhpzddvs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2edpwpgxq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkwjrsqu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2keiwryda.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pdiitjcb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lwrkhqom.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dgmbvssl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iuqdusdx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2xdrvcryt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qiayntfq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rtgpgrtf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovmggoyk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2uzzfohfu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2guaccnzn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2oorrbqlh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bzwupxkb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2nztvwzbw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbwuzqdp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ahpyhojz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2wqerjukm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2unyqkpqx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bmrzgbtk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yexymlah.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rmntgcoh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2doexbliw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pwwuudkv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2sapgymhd.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2axbbfaae.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nrmsqanq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vppctkac.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zxmhugqv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2tvpidbej.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2cjoxvedp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rvffixzp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2oqpslpeq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kivczbgp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wxueqxtj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2lwemrqhs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kfqlqdwi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cqtxuaqf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2hbfffael.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wajepewa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ahmeptry.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cxrqdgbq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2qjlfkmex.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iuleisie.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2rgntjolg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uzhulmcy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jcfozmgw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ilxgguop.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2uzlimsdr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2rznhcvsv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gcrjbyxt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2fghfujoi.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eikxkxod.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfoirmjl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2oofskuuo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2dumqqdpf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2pcaieeec.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gazwbybs.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qwexyrad.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zxkasndz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdcexipe.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2obduacuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfaqjqmw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zuewulba.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2tnoulval.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2tffxkwod.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xcqeoxfi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mdpcbjvf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2vnohzqme.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hxksvrmj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vqcpcbqx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2nhiqbewi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pioosila.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dylnabxj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wfkxfqjs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ftalrzmw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2askikbyy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fvkuwikq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2oquatgne.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2oekkbtzi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2brlgsssh.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ylrpyoas.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ytjwpfmr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fdneexbe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2iytaplwh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lggrwfvq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2msfnxgza.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mgpiesed.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2cvnorjeu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2sxmjzocj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jxqatusw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2gjdznnbz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vwdwblbh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qxgdbssm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2uhgjnhwy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ycbbffru.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bbhoahrc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jhsssxfd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pizpaeik.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2twctevoy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2irpeyxdu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2coaejgsc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2upbbbpxo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2prfgpztv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bkhiwjlf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tiljxqbb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2znxfngax.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2amrxluhp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2agunognh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2aqysweyh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2bzqnmaok.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ggcegdei.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zknavclv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qqdhwueq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dllmalyb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xkxagisu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2assdmvkv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nuvvwvng.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2xavssrls.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rzpgyzro.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nrzugxqs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wdphshay.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2okfuppdt.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cjulrsrs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2erfzzhmq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bbemsukl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2tafowked.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2yruqodoc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2swbjatjx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yeeiqyqj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2heazlovn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2dcejowpz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2nprebxox.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zazzwfwd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ymdbdysg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmvjwsrq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2lvdibwjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgcinnft.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zbccextr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2afcbgfay.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kqkaiojd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2khgdtqko.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qncyjvxc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cbeynbek.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xwdnmdgt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tpptiley.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nvagsgly.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dccbrnht.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qehjdxxt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2umqlvivj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vshyxbml.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hpcqzdni.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vlpbpevh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vdfzcryj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2enhqseqs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tehmhavp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xcimnfnq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rifpjtau.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fikzwgne.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tjctsimu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vleoroih.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rizhvwkd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2awythgis.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rtgtmkor.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2sntxlcxv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2alukpdjy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rezgsdkz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2cuzjbpsk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tgwkzsku.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2izxtglww.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2apfvnwza.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qtnbztzn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kouroisg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2uvdwtjnv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2czednhky.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhbprpnj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qlyfdjgk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jroiywpn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2whqhnoui.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bvkslpmv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2teedwcfv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2sstbmbwl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2vamlkhpg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dszjgenk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zuwiisxg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ahdmvoad.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cbzkslny.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rfcljvln.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hxxbloat.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vvlumptb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mfbhcefm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wzbyojse.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vsaqsckr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2nnzfjsni.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kuovbwfe.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mpjehvhb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tehfoyuv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2botqzjsg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2enmzuejj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ovxjnaci.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sqbkjyjy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kjwxtdab.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2nzuwrdom.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lwiwwuvf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xiefkqap.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jgiovrsn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2npylxbta.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hwpgztjy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ovesbsjb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bhmhrzxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxdkvduv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2juayayzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkoswwqu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fgekcyft.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2grvnuirn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dkaqbtyj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2orlsdtpk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2muumemhw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfdazvfb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ekhnrhbe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2cwwagpyj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzpwizuf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ehowxzoa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hjzapouh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ilglsfrh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ozqkdsmp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fprvlkcy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hbafmvvt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hsccwked.html


<!-- 参考信息 -->