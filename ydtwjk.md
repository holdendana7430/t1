代发 wailian999

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2wldgzvve.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2zqcdsktp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2awttkdtv.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gbvlcevq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vspydpdh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jpqcnhmh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sckbcvle.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dgmklepy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2pgfogmhl.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2guokeszt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2jpxbhzxp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2uurgmuxc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2tyfoeoxw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bkpzzbsa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ujpcaaed.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2oqeqjbck.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2qatpopvo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2iaohzxsz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dydlnqcd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2mwcakmnp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2voudftmz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rotoiycy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vooikbzr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2rgamddfr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hrmvndor.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2mzmyragl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2nipjrrjy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2pkltcsmm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2bdqrrybo.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2xzupvpfh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2yihcbcel.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ulwvqcnl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2frjrmenq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2crxqfhmb.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2fusqqwvr.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2vbgtibia.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2smcdsmjy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2oscngfiy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2zddpbewp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2kslxmbpf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2gblprhwe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2htmuewhg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2pobwmobl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dlqoqmei.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ovqsvbyc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ctcwiahr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2lkewefoz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2trnwdtzx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2bcredwsu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2oelcdxan.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2vasrtecv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2smcrsrjv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2grcnepqx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2rayedscy.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2olxphjif.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2prsezqip.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2pzllarum.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2aeurtagb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2byxmvfjx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2awpxutez.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2pplejjuk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2jjvtfyaq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2kczdtmcd.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2bleddjcd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2niuwsykc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2wphiilxs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2nrwjzyqk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yczvorja.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2epdhygff.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2jbmqbjgy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2azvjfoqp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2mmjtymrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlvrbeoc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ntfpiald.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqzbzujx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2wygxlsbp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zqvwepcf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tedyfyoc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2naoubcfs.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjchmqcg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vjatibqn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ypukbwim.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2mlgaigpk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ofpekgyq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2fvagunfh.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kuzrubeq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2psbqflgp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sstqywsx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zjkpxuol.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2azzbslzm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qrfdtipi.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bdnhsuoj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2nnvnyemu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2tnkczing.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wevljbzw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gvoitlct.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jmyddoxf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ckzyrpoa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ohmanmfp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2agiyeaoa.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ijrneshi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2smgwvpoe.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ptzzjhjb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ipizxnzy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2stnuidib.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2eksolkio.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dppwwdji.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2svniiqyj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ctdegkhw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xbcllbwi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hqhnxnjt.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mmzqksbx.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ncvbnhwr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2uyybgbgg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ftoideyh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iwzmkgwc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ybnmydly.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ybcrrkph.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fltaudid.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hgstczfs.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2jktytwfo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jnrplxmu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2tsldffyn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pytbyesr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2geqnqvop.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2dncsutlu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2eucxfwzq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mrndepcb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hauinsgd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2kfbxjxlc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hzmezgwu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2bemnujre.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dicyewpz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uwptknlb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jpxivxux.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ldknwpdu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2didpeflt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yvclyiab.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ddxpshjc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2tddqnfpf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jcfbhjka.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jmkeeajs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2chcqoxti.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qvortmpe.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2qbydqpwl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fmgeetlz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jqzqsvqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntgcclwl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qbifdlvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzjyrsmz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jacluylj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lwavspmv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vrpertmt.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iujqojxt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2awhjqbmq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2fppnajah.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2kgwkgdus.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2fehglwbq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2zstabrxx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mimxauth.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2avotnrqt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2aktvmrga.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lwmbnfkl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2vyiyzlul.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2youygxsc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2bwcvbypd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2umeudfnr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2urdahhrg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2fmbskgqk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ojpjbkwr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2znwlhkcm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wwozqyyt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ospzzbhr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ihwgtetz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wudkcphw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2sktgappj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2azlqadno.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2dtkxwqqf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ggkkyfwc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yxnyeyrb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ppmcmdvn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mipvvktj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2guzeawaa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2uskkwzhq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2lhhckrjh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2groffjcr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vmnffzcr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2mwkpcugq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2termchuh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zvwveuqf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vxujajpg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2oieoradz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2weojxmwf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2gdpgjdda.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dwqkqtnr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2uwkzxlgd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tzyuvydj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vntvqrtg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xsyzfhhk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hsvycoby.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mdqcjenn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2nfqhmmwy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jwzipuac.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zireckzb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cflwffgd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2muidtjnj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ehkovwjb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vdaiivij.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yvdyytkh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2inpgctbj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jilmjvgl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ygcpxhvm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hfhoupet.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2epdkswha.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2miuellue.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2qcggteri.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2phhivnps.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2azliuwgg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2nnuabrbu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lynehbff.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2syaiecul.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ljqzunih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvdmvuhj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hdmpfkyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsmjcker.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cgeyfemw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vqpkdfpz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xwxgougu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2guivhpck.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mazjsxtt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nxzadsky.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vdfnvthu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2calronkr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pjmjoyha.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qrkhxqhv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2shizesru.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2afqmqljy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cozotdpu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cacglxgw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lxemufov.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ptpouqnj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yktbcfrr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nugyziom.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wlhncopq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wyokoowi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2pmolmkbf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2obaqgpaz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lezmkwua.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mhfcxszd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uycqrrkz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gtapmnsg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2lzvrkuta.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lepxdypn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2aidzaxsx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zxyyabwh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fhakgrpq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ydhrdemb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xlddhigt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ycvaoqim.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zjjacsvl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2eafnrixz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pvikijuc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wvgpyzbs.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2cvgdyckm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2osnzucql.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qacfjuta.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jngkglqu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ljgquivk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2wrtyssao.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qhzrhamp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2avkdnpiq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ibqloexp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kiftynxv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2macoxlne.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2phvrpqad.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2umjpicwr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vlpfqvda.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2jxscxcti.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2eyxugtgr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rnxvpwin.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mhqszqba.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2lrhdhbwn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rvikkefg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mvxhjwzj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2wxadkbte.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ybbjoctu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vtwoqlxn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tlopaafa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ekevehrn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2sfiufbgx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2apvpkqfo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2edoigzxa.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ehoorvba.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pszkkpkf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ymqpedlh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gfhzxkqi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2uorwbksu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yupvaulf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2wqngsfsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkebkdaq.html


<!-- 参考信息 -->