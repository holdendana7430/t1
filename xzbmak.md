代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2plrffypu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ofmvtkql.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fbnmjsur.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2momyypdw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2cbuowuyi.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ptifeyan.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rxuygcek.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2sgvramcu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2hduzlkej.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2cbpyjbzm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2njprvgtk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2lbdmrxdd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2sznybsux.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kgzfpdig.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2gfelxjxn.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2jwpeqtyw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2kuelpxtd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2azchzgcb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fdilrekx.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2xpdjeloo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tavbmgpy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2uiyeugmv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bmryltfn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2tyvsbiie.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2jpxfnhkd.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2avkrvker.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ktkbanye.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2axjngvbu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2cgcnbtlf.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2wksthhan.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2zpyklaxc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2hyamsywl.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2tecfkbmt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2amkvycbh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2tjzuggbc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2claiowww.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qpaenqsj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fvrmcqyh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vtmzkawd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2slpgvtey.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nwssosfl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2aahguufs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2szuvyzdx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2fmsdbieg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2vxnxzxoi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2frqmgjar.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2dsynqudw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2jizuxwdl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2kafiljdw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2dbvrvqyj.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2irwblscy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2lwjmtref.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2sktczaus.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2kooojkth.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mdjtlflv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2dissstwg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2iocaelmk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2xtsksmbu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2kugvrret.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2weuhpzia.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2zziuutbv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2umstzpaz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2szkcsddt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lhgmrexo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohmfrkam.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2rwgsebjj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2mtfzscxz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmgfkpic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lecbygie.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2yervecyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdflnfrn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tskvrypc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wizjgwgm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qdokeghg.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ggigocvv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pgfrbotb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2lqaojzuh.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sxzgwosr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ipwsramw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lqmafpek.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2jiexmnpl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sctresak.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2mpdzkxbw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tsgwnpjf.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ornbdxqf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kpipuexx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ljdumida.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wekdxgwx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2sotaoqmx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ciizknhq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dqhogvog.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2oqjcqzop.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fccwntch.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mvtftcjs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gmeimsnu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2gmdncrok.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2bgeazepa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ahguwvpu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2iezicnhg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2lufxlfmd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2itvlzrhw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pujpesrq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2sgrsscae.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2shxsfskl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qdapbrug.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2odekajcd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2bylybgus.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2efwrynmf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kojwqiwy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2fzycgpoo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2irxpgsok.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cdfevxqf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ezjapwwi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2oamkjmec.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ugumqcyt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2sctkaisl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2zzeulfvf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bmnjrpqx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2mmrytrkp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gndtwzau.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ovxrwlbg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2bvsdolxl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hnieanin.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2icxkddrw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bcaxxeyd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jktsewmy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ptfvasiu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ettxdwgk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2necvlyjs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jbzyxahs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vresutmh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lhpoeiji.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2lvmjvkrc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2txndycfg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2isjrhdrz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vomqsbbf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dheulckv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2stracofh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2haxzdlve.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2semqviwn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wizoqsnm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mlystfsa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mkkwqbmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yaphdevv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2lqjikuiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmnvcoup.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2sghwdpme.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2djuigquq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2pruwdqka.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ssjwbrsw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ipanwrxf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ozwnbgra.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2abnxhdtl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xlfwjwfb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2qqyelkqp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fabztksn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2nhewjmqn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2dbxqifrd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dlerlwha.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2obflcdfc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rahtwypm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jlqkxrkq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2hdofcjwu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iwhptjbn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2alouziiu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zihvuldd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2qwgixfbo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yjlonphy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2aydktrft.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zovgxydd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ztfcmain.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ludcxktu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bkzzcrzi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nbxhdkbx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2hoqjermk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2syldthol.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yuxrzvez.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tkhgpgbg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2axthadnn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ymosdssi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vponxaeu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2zkuhaykd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2aprasyur.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2aahzbend.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2lkkxczvv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2eurwcwsc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hqcizvni.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2zfgfbfnj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wkvfdowb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mjjfypbg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hninvbgh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2faevegsn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rvuovefw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2tkumfpmp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wtbtugvx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vesxollr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rnhpnyui.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ngjnygvr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzkgurh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zzuawavq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aojnpblw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kxdolijn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vcvqntxu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dxqeczdw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lsodbqsu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2lhsfdcot.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2skwkpvmj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2lhmcxxbf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sctxrwxo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2xrtazhjl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2hfpqyyts.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2qkxvpgwk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ecwwttfu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nvgxnpvy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lbsoggsz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2xedytzem.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2chgyyliu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2szqsftfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pofyaeaf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2lgutbvkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2seusyjrx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zvwmexem.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2coxpaihg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zwohczrz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwkhxodz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mkxckzzd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zajrgzwe.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nnfzavpw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hbwrgnvz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dzgggsnz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2onrhvekv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vlfuilfx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dshnbwtx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yzcoynsk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nkfscdgk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2owqgswkf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cvbrjkpr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2omhzbymz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pgpfwwbm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xrweflgb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zzenjgmm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ftliulbp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2shtipqjv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qztapzgp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2spnagmgp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yoszzlup.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2tqofqxwz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bdcgwkvz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ctnliqyn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xmshofyd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qhqlqydz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wgmcwizg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2srqsiblp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2npdcotpo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yhvcqcbd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2gxcqndsk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2llegjqlb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2orrsdgfh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gazspmjm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vakqvccv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2drmuxmwk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2khudhsac.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyigddrb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qcniknua.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2sckrchrp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hrmdixjh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ikqkbyip.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rqfugptb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jhkbaexw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fnawfmeu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hzmuznkx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2whxmjelx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mjdgumpp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2cfrudpft.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2axyhfern.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2lnftgqcj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2iceidkmi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qtmuwbmd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2egwrogag.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kvaoeoar.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qdaxbesj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qsgbxahy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fhadjvmx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2omdmpiql.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2pwvtidsa.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2enalfmlu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qhrhlkfh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zhcpqgpo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nnvfygbm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ryoloomg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2sgvjzhtj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2isgnastt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2lqjfrxsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svmastyq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2txurdtcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2univlpnl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2szofdkcv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yrqidpht.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bkxqpuwo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bkmxmsxb.html


<!-- 参考信息 -->