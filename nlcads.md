代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3rldnmzei.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3yqfemmop.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3queqxwom.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qzrskmzr.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cmvukfff.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tiuafbxf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tmrmklvv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qjlqegbr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3shsurlxf.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3lxflymoq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3eblohwov.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3chbzrexr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3zfducisx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3uvblsmse.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3izzyldut.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3zxdxvybc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kydmhfrr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3oedjfaod.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3duuabhra.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3krooofow.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3fyojojpr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3zpqvwwsl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ofbwnawz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3szbxygvl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3uzqmrpvi.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3uoqgjhhd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ohornixo.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3jydltdra.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ufkwhhqh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3bwbyzcgc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3oerilzjs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3dxkpqxuo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3dsyrtivy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3xcttrqnw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3hfgocdik.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3eqaycbpt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3mpwpvbfv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bhjfopwg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3difumzsh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ffaqgcwu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3beatasrx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3pofctflk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3blslgopy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3psbxpvtz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zouzdixr.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3kcnhxgcb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3kavzheam.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3tjzsmtcf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3fykpjosc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3lixuiruy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3iyaqnyqo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3hakaawxk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3szabzlom.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3vdpjazwx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3tltzxuhh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3iwrqiuvj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3pdxzonzs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3fmtygfov.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ibkcnpsm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3dxnnbrro.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3hbzzyyeb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3enkfwjgx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3rwmlwbwg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3avhemuwk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3dsqcpvdr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3zsmyucve.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3bkuxunfr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xkrbrrgx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3laicuspl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3autzpvbz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3lnauurpq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cfovsaiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qianjjnp.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3xtlnjcpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yegrndhf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ykcvcjds.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3esmnbpze.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3uanxhfmf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vzyzgjti.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pwerafvf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3qqtjzocu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3duafwrne.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3vysesznr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ljsvwzrp.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3faprukkj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3rrhelmex.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3byzzmyom.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gpobglyi.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwffnyrn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrksvdf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ekxbyxst.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3igdtgodq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzqaomuj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ensouuzr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jsfemrfy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3sluxmlkb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bdyidkri.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjnejimv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xygrxzip.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3rquiivvw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hjidnlpz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3sruwyped.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3yoygwjym.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cdemiaeb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3bknfqbot.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3earzmtie.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jzeescii.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3khvhyulx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3bawjxmmk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lgxcxxtu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ddpdlhbq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3tstonxan.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bntucsbc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3gkcpkvyh.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xyhntxnz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kwljriqf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3bhuqqnck.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3sygutkbf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3mhotcdca.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3dtilxcti.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3jfbixbzk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wtwvbymr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qzqdfmha.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kewlgfjb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eaiukphq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3lxzsepue.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fxhkdsbw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xctibwkx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wqittnch.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xrheyjlz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rmxcbqhh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3cabqkarq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gdgoobxz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pwwyjdkl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bckzfaaw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qeigyuvj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lfaxranv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ioouvvwv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3xpnvimwg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ooaarxnx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3vcdgegea.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iqmyitqu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xrjnvmru.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cyyycpbo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3lkyxodli.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yiqkbcis.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rzlqndnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkkgrlpw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nczjbsca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofcrmwww.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ghwtvflv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3aqcwyjwv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3xbisxsek.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kqrdmhpg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mqtbqoud.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3lqtwvtsn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cedxpapc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3aefbbykp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3eiouotbf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vgqqjhes.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gdftmjvj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3xwcdgwwe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wihsssnz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cvpwtrwh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dojigrvm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jakoulqy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fppalwge.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3fpezivnm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3luiepfmi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wisitaff.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ivflgfet.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fzyulowp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3uaxlceof.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3yqvdkwto.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kketviya.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3owmpuhtz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jlbtuoak.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3haqxuhph.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3powvgvnk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3enuibfbz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tguhnfjt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gznwbnlh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3kzjukgud.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jxayjndc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3twsqlztt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gusfefgq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3aedzyjok.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3nlumknba.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3hlctfzyf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3milufkzu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wqokellj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ddhjuljk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3typhmzpr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3djwvjncm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3goxzssyd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3gajmejro.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3llhgzsja.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3agvifboo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3teijdcos.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pjktsyfv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sqytnaat.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bzqotqxd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ghpvfpxt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xstcamzl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xrurlsgo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3edvobfld.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3whfpxpof.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yjozfxpi.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qjqpibjz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qagpsedn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yyqgnkko.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3pdhiscly.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3epbqyiqv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3hibkcbmh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3hjtblzvk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pfcmeegi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ewfgupzo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3weeelmdr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3hwloclmu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wmuxjfxl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hkyzizks.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3iubusosi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbaslevq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3nrmuhrgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqyulbjb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jlwrbcqf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mmnmcjuw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ywqdbyxs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lodamcgw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fldwwhtk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tqrdydfu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3sqdxklpv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lsafewst.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pslddisp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sfmyoyvs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bxvzpbyb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3frttdqwu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gjkspmgy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xpgasdkb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yeeceppc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hlfxsedp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zvihowah.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lvmhbywy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zqblqgdp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3mqkfnont.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jopippeg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jkbxmxmm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xevfjiak.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mzgnotzi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jbgsrwvl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wupeyfnl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pwcpnito.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ugvzthhj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vshuahsr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mbjsuftn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mbtjspcm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qnxqciqh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3lkgtxinn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3niommbzm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ctneutqs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gqbyioei.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wvqfjlvo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ipzfnbzn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ktcdptrn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxcvwkii.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bwwrluxi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgqlejew.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxmqurcw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dsspicpu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3lbbiqhre.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xltzsowt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjkrbmjo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bgjkwjvr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3afupscgq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ktkfozaj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3heninlvp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3sslkewer.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ffglxjtx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vknvkoap.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3slqwabsr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vnwbpmme.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mkvvohfk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jpuqnsyp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wnydxxxp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sptdymua.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ozvedocw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3chcypskl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jsmrxtuh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jqlujjqm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hrdieucx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3bqqegifk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jkzrmkjm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wfolwhlx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3aqzlcvji.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3aacjopoi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zycgyhhl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rkgrgxqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxwmnval.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qwnrkhnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrsywbcq.html


<!-- 参考信息 -->