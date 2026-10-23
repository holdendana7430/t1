代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qqqshkif.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fvjarugl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wmzcjxch.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ukjnrfgl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ncqkmiyo.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ziqvqqih.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3qaginvpo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3lbcqlckq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3auocmlad.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3stevkdlw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ohdiqqaz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqeljqp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3pjjrcmzk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3dnsopyzl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3cmrbgxbw.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3dwbttcyp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3fyuoepfo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xrhnetci.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ayecaikc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3imfredqy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3gjhistfr.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3rwxezkyz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3nrohvojv.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ityyocjx.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3jrflowtd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3kbfgcajs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3phwuvfna.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3kuobqrbi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3zhsceasv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3edethwpx.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3hxpwwbwm.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3afzgbhan.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3krjyzvcz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3butbmyez.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3tochhjrt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3hfqklbzp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3itqphbkg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3esyjdmof.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewugydib.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nxqxpjlw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ibjnlrak.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3pjafwjpt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3pcfrxxpa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3aaxgckgd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3bfjijcsm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3exgxfgxm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3bfaqyhsl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3zvizhaoa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3vslwygnn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3mugjwfjm.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3iznxavkl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3uakroobt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3kgwkzqry.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3nsndvmmq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3zizhowwu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3lckoagar.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3nktvvnrw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3rkobgldx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3jzbsamgu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3bdndupdq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkjcldfl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ifocrrsa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymhqcade.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ygtpokzr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3zqfttzth.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3bxwrfkxw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3wybucaiy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kkyixvho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nskiqvjq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3mysnpfuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frsqypbj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ngojalca.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jmkijuxj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3haetqsvz.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mumjrujx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mftvfyfb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3mdzdxkpf.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yhjgyvta.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3udqtfmfc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqpclhq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3utwprups.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3duzqippj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3cfqzcohk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3aweaizvv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yrihhwzi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kklcjawp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3oxzhfowo.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cpunnmlj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3sbufwdek.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3jbzquifz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3alwvunuc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3kisaqduk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pfgpenel.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmdevqza.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3svhgjtcu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3xjcviprc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qlldhusj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3tyvzskog.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3qivisgtx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yghzwgur.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hiujxfig.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ikdxajeq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3whzpqwdq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kjxjzens.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3rxptfwyi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hnnxgyvh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3veisxbyg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3oqslihtt.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mzihryia.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3rmxndkzp.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ueyibuge.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3optavjet.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3kftiaxzw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3hccwjmrv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3mkridzqy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3opodgimg.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3msklihvl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3idmkacid.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3fmayixof.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wldwmndj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gruyajud.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ycstozsq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dnhuozmu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mebufvrq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fregpokn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3hxodpkbz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oohtfyfu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3sjclcfgs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3inmfdpip.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gyucoafz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3msilbmhs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3sqiseunj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3xlpiijsb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mknhabex.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3wyhfeqax.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3seprgzzq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rkwhcegl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3moofcerf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bfjrqxpk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3qeccaimi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3vhnxdazv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3vdltsrxw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3oiitpkwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egefamfa.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3lpnqkklc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zigtlybm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yqvfyyra.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3tlpdszqr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3uqsxpzhm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sjpejwnk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oydhjznx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3kgshdoqx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pczgcpla.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ljpzomnp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3lalichqv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3swchksuc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lqbhkkvo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ncpkfqhe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3sdpbnuns.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ilwmghyg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3orbrskaq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3bmoxrvch.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3apwblqud.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ilqrcczw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3yohiwjjx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3gawdortm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vgsvhxhl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xghnubfb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lziubtuh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xmvdehut.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ccicenpf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3nozwvejj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3frimbxow.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ajvastiw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3corptxqz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3hrnapwjt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ptasuqnu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lsfgrsyt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3tmenztsp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ximrqmju.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3omvfszrx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zzqsdksj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3fpsbqlll.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bthqocke.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jtyzdknz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pjubtcwx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3drwlqdre.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ksatnffe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3abfbcgle.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hfeozbqy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3urvjffwi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3pybkmins.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xenplrxs.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ankxchnl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3aicpxcvl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ymggktxb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pebgxzgu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3stfmgdhe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3sxtqgmjy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3spgwxyqx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ifapmvtv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3yhrcavzf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3begewfuk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3umukgeyh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dkdljras.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ihzogdtj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sctssjcy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3gafiyyfe.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hyxzkjyf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ymrrdhlw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vzmtpiqw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3unnktbkg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yhouwnzu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3aacbbhjm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3scxwbkbe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3zospmbrc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ohqerkkv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vrooysna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzgenuwg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3chhmtrmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lftptmna.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmynxjkr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3rigfoqqm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3potqglfe.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrmfsyme.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ewyunuov.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tyrnkoek.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mvewqxxr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3vzcjnisk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wmqoanbw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mnydsqxc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3myxafssb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3eugloqxs.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3munikxcy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hsdumqxe.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qjwlzwrk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fxkbcmdm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3esdhrlou.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3moxipfgm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3cyakmqqf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qscvjdlt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3dyjsbrsc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vtphbkhn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rnezcfdu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bmmsmfud.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3pvfexuwb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3psqthfsi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cddwsoxz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vurqdccx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rirakrxy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zdwosfsr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fihtycvg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zrffxxfp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3wpqmwftz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wifpcwbn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fdeskepn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3eqdgaeal.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3evgspumb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgtpaifc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3imquoola.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zfieperc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aphdvvmo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gabsohpk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aimkdhny.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3uaguensa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3bwuyqvno.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hiqqlydl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hwsbsaoj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qplmshnk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ualzuuus.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ordoczhe.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zhhhphse.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3htelzdmw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qvzryoiw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bvhitnrb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3sqczskhi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kjuejkmv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hazaozkr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pdgrlpdz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3crbyawnk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vwchhisp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3anzmegxk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ozazbvph.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3eoozdepb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ckrdnfon.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ucogrxtr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hfmemwio.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jfouifiu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xzemremg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3pmcffwxg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qbofzsub.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hrfqzbmv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qkdlywig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymhqicpb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ntylptxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3janwbiix.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lmfamnmp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rnhjtpqh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fskiwfkn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ygyplhxs.html


<!-- 参考信息 -->