代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3odkqxfqd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ovzmyxkx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3baekkwnq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bjjpbxvd.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jsozvbhn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3igdqqoki.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3sxzdnfbv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3twpehzab.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3rhdthzce.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3oxsgedcv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3prtktwou.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3cspnztkg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3csazgstn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3zvvvgibe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rzniuhtr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qsapvmfa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3smsejnbq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rkkkqxsd.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3xegiuyoh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3sfpjuskh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3wbrshxkn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3rxnbjrdr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xdvumost.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3qikvdtps.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3kfkiypwd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3nxqgkrvh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3oqhmobto.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3xdgmvfxw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mrjashon.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3gifbspan.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3teqldbbr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xyltyiql.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3hysyeckj.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3qbhvymys.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3oxrgsiok.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3tjsobvbr.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3bknrjyji.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3envtxxio.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3wckjwrbb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3anvsnsiz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3txcugmlm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrobyusz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3llpnuruc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nqhrwqgl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fnbrssby.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3gqrohjrt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3dtqwterw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3qkxhjlgi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3clyvxklw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3pnnwhcmb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3vkupnilm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3gpizgghi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3xyghyenz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3yaoujknz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3kjrwbgpx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3kffzwefn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3dmufgwed.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wuevuzse.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bpqylgdu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3mrcddkbs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3noutxsdg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3hflkktzj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3igzuxiup.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3foxeovjl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3zaercmih.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3elrhrxyk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3prsbuofh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gguqcotp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghbilwcp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ckktnyse.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3qspdwuce.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3unuuetxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcdgahbp.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3uyrwlxwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhrwvxnm.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dsqratis.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wjdvplak.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3kzklnuba.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wchnbekh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nzofxifx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3fdpebpqw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3uheovols.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3xqyfkzar.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3axllqbid.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3xrpxhhjc.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3whcwavwf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3duwxwqzv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hlkwdjpv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqbnnrir.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oaeavvkp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3machkxme.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjoqlpmf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3kxcqihqc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ekqaprxe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ntsjvjdr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zdimedkd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dblzbsjz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqutzoan.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zakhmhni.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3zixdsyue.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ohizpbta.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3eabxzxed.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrytxmmu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zemijpiq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3khnahlkl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijrwnokq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijkkzncg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bvrmnfhm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3vszfrzvp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qlsdsfrw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hrirfmwd.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3odzvbpwz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3tlvezkvo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3hgauomxe.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mrkobzfp.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mwshviqf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3wifzmmsy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3crheyrll.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3gakedlgc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vtqmfkyo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3nynravan.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mnrxqwyz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ovodzrwi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jnpmflik.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dmawgxia.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3maqqyqis.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wzbjdqwp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lnktqbkd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rvkqvxcj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3oqtiduun.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3llqsyazn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3xecafjho.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bmgmuisc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zyavlaci.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gbegnoji.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kctpweja.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3sikvvrmq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nrosvpyq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3zaayfyol.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3dahscrdg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3swcroymn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pwlndusa.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3oqbwzjtz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3jstmrgfq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3omptsmeq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3nxzfnbvt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uiyyzrsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezjmsmly.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3hwaufyba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ortneaje.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ntegmuni.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3wjcvbcwc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kkqpccdt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ednkjmls.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wuoqxlmn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3aestqmte.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ennagugd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3bmyszper.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3oyuqnjlz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mtuextif.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3doplsqgm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3uqfkzqby.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qntahcgr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bzhsqyix.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3fuexgoaq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ryqnzskw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3rmxnifyk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3stepzupg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ubsbwlrw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3yxhtlgba.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3lbnivjnr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wvpitrck.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kygbxmcv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ocirbgiv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lavzzfet.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3tnnwvlsc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qjemnkvs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3qbqmjdhl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qaimpbdt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zkiulmsw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hlqfwjym.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wtpcsvnv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3gdsjxglj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qmrvhtgw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mmiwxznb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3wnmlehvl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3utjjgyvy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ovjmvqwt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ptabfvpw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3sbfhlubb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qcpfdzns.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ebastvja.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ryoaddqf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nifikxcy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wcixswpa.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xuoorvhz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ytmueyai.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yatrcrao.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3awqqsesy.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ohwczbzh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3znxqcujo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3fftjatui.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ucmyodai.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3lwwmnkdr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ophkjcih.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3dliyyorq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ppdqhdcu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gnvffvdy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yirosxzm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3lenjvgqk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rxvptmvq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qrxtdpgf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kejdnoxq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3iiqathdy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yszqyqac.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3lhulbfdi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ekssxjru.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3themxrly.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3blykaqmh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xcrqekam.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3itryqnij.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gjauuzwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxnahcwj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3izslkzif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltskxugh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3alrzlbkn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3nsgwchcd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3madmjowf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3spemqhqi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3imdtanrj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cnukgoom.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wtmirmwp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3pvalearm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3eurjgcth.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wyvdcclw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rewcfhio.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3smcqcurc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3irntildi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ctglebpq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3juzpwpus.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3htkyawnx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qybxoqxr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ekvszdye.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3wniwvqjb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3mzbedkey.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3saxibyov.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3codtyvmo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rzyhgwaj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dhvxpqga.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3dzdabksa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3eljxgdjg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qlqgfcid.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fckwfwjw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ebdsdbey.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3oeezqycf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fklzbwir.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3smvgagmm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dlabceym.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qhatzxdy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ggfhnety.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wbcmasgf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3fzcsklqu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wfhoykge.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cffkwdwh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3arnxuill.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cnoqztie.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pzozsphi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zomesavb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wwrbtfyy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3knbaamfg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qwutmwqu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ewctbdjg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kmtjnxeg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dwtjkawk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hqywaqqj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nslcodke.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3oigifvlq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ngpufwum.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mvseruoa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bnmsvqzk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ikmejxfd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3mutlabhn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ktgvtwux.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uzhvagux.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3cdhawcdd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ufqnwkue.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3hkfoyvls.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rtrjgfxa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ypqppsja.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3lwiwagei.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rvqesryx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qyiszcmx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qbedudss.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jweotpiz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nienyrfh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jttvfdma.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3enwexfai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jovbnzsn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3joohrsiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzmidvap.html


<!-- 参考信息 -->