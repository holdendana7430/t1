代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lhjbyyjp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gbisynae.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2culfjfqr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kpwvkpbj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2hfocbvww.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ziammajb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ihwizjwy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ypvdgagu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2lkrjleyl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2lfvkwmkb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2mllzbxts.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2qooheoay.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rqzrkvne.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2damkascy.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2bkgllnxb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2txnufqxx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2rtfgccou.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vyltdbfx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ndaokaxr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2uxuxetfq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2wfsxbmcz.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2rdpsjxur.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2eqxgthfo.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2svlqmlil.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2yncgoyoj.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2pomqdalh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2pougkdwt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2jviqxmtr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2znhmcoyo.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ccowcdsp.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2avjdwlug.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2cltrsrwe.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2prjiqtrn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rgqautln.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2essmxxsz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2oklvddfi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ftdyuxbm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lfbjzpps.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2futoyjzl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nrpmprlr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xlqymhdo.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2xqxfyoig.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2dilzbnwx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2kkcljist.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2rlkdxuav.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2tstympys.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2hmkdtpbi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2vzxbbmzi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ebxfkgkt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2suovvnio.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2vgkkyfka.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2lblcgmnq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2clqweqqb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2coommqsu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2urbwnffw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2dpmoiajx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2nuxqksch.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2eksbiuqw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2qgzittoc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2eudujaru.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2frbefbhq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2hkwvtfds.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wvtbrugh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vkkzdhhy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymbuxfce.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2dwvycdrf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2armwrtva.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2wsximaqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gumnmwen.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2pxwvjrcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkwewbfh.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2uswclapf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2plqbiwhu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hzslfedg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2szrlivvx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2lsdtsimn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2mggkhufg.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gzevpcpw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2jufhlymy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2acjcrcwq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2jsagrncd.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2wfkzjikc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2wqfuwyxy.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2whsjmjze.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gkmqwpwn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yzvbfmdc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mmdrxpli.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ttclqffb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2jnmdxdxe.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2mnocvakf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2btojgiep.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nudneokq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2dgkdhjqo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bdystfbw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rdgrmijw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ygixyhkj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vecjfciz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2bljzafrw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2vfrvhslu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tavmruos.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2heluilvl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fclugdlh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gulosaiy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sqiwmzpm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2nxgzljtw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hatmmkcr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qxvvkpbf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2nkwdqauw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2wlndwgrt.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2qkgebeyy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xsvvhcxk.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2siraelxx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2oganuuuo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2swiwarwx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ikzvizjp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2tjzvpjji.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kdomkljc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2szlxrbcj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2kaujdlni.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2quvhczgx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2owsffyvc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wmdsqvna.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2etydjzna.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fqwfthwc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ktfsfigt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2mnokivdf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ujudverw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nwxiizpv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kaivkcvf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ahexrteu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vascoemr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2insfhuwy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yrnqeauq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2murpxnqx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2bunvxpyl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xdznztxm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nrhfkere.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wvydaniu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2trylyejp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hlolbwoy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2pezwnxbh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lfwkalgh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2krihtwmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqimzven.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ixbrfwef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fiznyndg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2eodzmijl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ohxqmijh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2jvkjthol.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wbfdstfe.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lkrqxvzo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2frfmglks.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2svpjrzsc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2blagfsgo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rpravqfq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2judcsudz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zdxhmxpc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ixmucstf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pskqwdql.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pbveqjyi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2puraotrj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hjjnmred.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ycsxzecn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2icmwnqgi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gwmuwvek.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2tejbmtqw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2kvfyyrdm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gkkvqtwu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2aynmjtah.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dhjchpjg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2envkzfdo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pehejbwi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2sipcolce.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2zagwpjcr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fovpbtvt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hmvgsbom.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rsfqolyk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wcoengcc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2vjufnwxf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zebzqzkd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2csquqgqe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fbryussk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2gxenhopg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qsmuxjgz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2yxpunmap.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2djnrxvdn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lokwiilk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2tbncsewb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2roxphegk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2igufhvve.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wrdzstpu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2afdetvts.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2junwdcye.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qprzjuvk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nrhamqub.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ucsvktli.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ggsmaakv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ufplogvi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2nxhkvdor.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2pzaczubr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tzfwvyde.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gxsmiupt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nqgaayvt.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hvpgavpb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ecdohelp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fuseydes.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hsbkftgi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zocbswhq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jkwagnjk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2myradzpl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pfzsxxiv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2twfzjilw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bnddsurd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iysvabuo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ortlhuqh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2oihwmqxa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmeaago.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ushmtjlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnqmtdyt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ctfamvvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdlegdnu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uhghrenn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rqceebxg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lrhzjkxx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tcxfggyt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2guyvogft.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dfckqrvq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yrbuxwub.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mepzugnn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2slekvzrg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rejufyiq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vduwdcub.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2iixiojot.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qowyyabf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sjqygzzi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xoimecod.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2khohvwwp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2fzayzmwo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2amtdzwyy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2cgdzvnub.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2uaoqmsuj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ymetekpk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ildmjfta.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ftwkstwl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2daljigha.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2aphsxmhb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nidrqher.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bqruqqeh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ujxztnfb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sknwcbna.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yrgugwuz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ykgjmzmi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2opihbikc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2vqkkjmlh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oqzbpceg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fhwbcypb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2zoozzooc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2iycxqpym.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqxmfehe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mjirdlzq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jnolbhue.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oclwypug.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iltyqjkr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnqqjbvn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kdhioggg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2vdrmqihc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ojzdirar.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jqynzdke.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ajyiwtma.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nbyqajoj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2eukfupid.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nwknhlnk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2gxrvythc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2osdzibni.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2cchewrva.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ygrznasf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fovtydlp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2myugeplr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dnzshfpn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uyrlwmkn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2cpfvhgzy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nvvgxsjl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2llwxwtpg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2navlifya.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xtyfqnih.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tkbcrndw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2fcxxiejf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gdrkjpyn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2migxzbma.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nwbukbtg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vywzcetn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hwyupvxs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rkfmbwpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krbqkfnk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pcsyuoyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcnupqbe.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2sgpxjnwa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bgvvqewl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dyygyxgs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bcujyqel.html


<!-- 参考信息 -->