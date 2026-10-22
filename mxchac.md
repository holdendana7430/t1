代发 wailian999

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2wuaafylp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2rzihjphi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2xgkzxbas.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cwqkwcle.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tiktuhdy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hhhofztj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lxkgacdb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wbqmkhng.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2vtmvfyxx.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2cjohugxh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mlflwgdw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2pxiyygcb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2mvjzogwr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2wbzjsrwr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2aqmrbmes.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ceagvjbr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgsmwxc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2zpgjefjk.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2uxlnxvdo.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2khrqixzn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ncqjusku.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dxfoorda.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2cziwumpa.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mnnkdbbe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2afmnlmsa.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2uclgyvwx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2zbmyqxoc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2lshdgnxw.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2inyxzyzb.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2yyapyaef.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2wezzqvbh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ypvzgjue.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2epnirynw.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vabykvii.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ylwbofix.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2nvrwwdxi.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2fvrkaxau.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fdiontmt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2hlzvvdla.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ecrexdzq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2cqilshzg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2hzpuhjpu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rymcqvrb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ajeyvcoo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2uppcauvw.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2feoogcyz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2onkzdvzw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2uqkitzao.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2emiuiynl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2mvnvpboh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2lbofrgin.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2nwuaydvs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ctvljvnk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2nyqnulbe.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2veeuqzpa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2nvekgpua.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ysjgfddq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2pfdabjut.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2wbpwbnjy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2eeinugxp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ddseryfh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2cnkskeea.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2dzgznara.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ejygpdre.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnyvhnxk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2gxdmgfnk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2lajzmqlb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vwnpxdvu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2axfvkzpq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ltnzfrih.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2bfzpbqqm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2krmepstt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsbqwxqm.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2sefllmjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvthizgy.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ncgelqvj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2lisctljj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ugrvyacy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2piibrkcp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rohggovm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2xxjamxmo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2xdkvwvce.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ksfbrpkv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jslawmua.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2fvpdmncq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ewrnskhr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2mqaaljhe.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bgpspzhh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkqlpccc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2firlihmn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2eopbmhmm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2syjkmrvx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2wlvxumfz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2aobhtwju.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gmrlydwe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2shehxzbt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktchjzhw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bubttizp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fesxslnn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2itcemjaz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rmsrxedo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2xpqawnoy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2wmdrbgoz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2crmhovik.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2sjfyptnk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yxuhinqa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ijcipdvj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tzgdyxjg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rqxedpfa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ckdvagcs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hwehmfcr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2isnqlhos.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bsjqrmml.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zitytrev.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2actzajma.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nflewqva.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2byfdvdsz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2hxfemwec.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2odulcbne.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tkiyttbu.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rxcncosf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rcchghdu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2lnaokasy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tfunjeik.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jwwbrqcl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2jekmdhib.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gtfaxqfm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qaijtxos.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fzamazft.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2uteigkjh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rolmzlve.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ncmhytbc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vwicitnw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ogshfbrv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iygoobcu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2pkflupwx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hawwbgdy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jehdhuxv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2tjjkwkgd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xlibvssc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2iamshunz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kzwzcxwa.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2udogvrlo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2tvndbvxv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2zflorxlo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2suiwlxrz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vmqydrsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngryafrm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2rtpfbxsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlmcuhwk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ucgfwkpb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ufvmnfiz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lirydbzz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jsmliggz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lgupdjlv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2lvltwkhi.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2lcwjfyev.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ammahboh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iyzkclcc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2faqxuair.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rwzuvgiw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2zzohqnjs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qrebhjza.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2talhvawt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vdhvgvqu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2rronyzqr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2iiyjnriv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2btqjelix.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2clrrhvcc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2eihcdeue.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jjolfwnj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2enctjkfw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2htvdzvvs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2rzskjfwt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pwuddhwq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tgbirvoe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2haxmmqey.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jcsustmu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ccxyomhi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zggiaplu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rcaimcxt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nbwjvipa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rnkeitow.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2himhvpio.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zznnzjjj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pdjlvcqz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2pofmtmrb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kxvvpost.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymwdittl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sbtnsubf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bkosmfxs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2kpmawmxy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2yxhubljd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2idiujnqw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zibgdkny.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xtazqobh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mhjfeicc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ekusmrjl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2knmgzgmn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jvocapgb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2chqfdlgm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2wehqdghj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2aornbcrk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2svdcbzrc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ajbxgexg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2tfmzrkja.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kvwlprbl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rivsungh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ydhsyclz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2plegzjph.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fwoctbbt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2tsinfggf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2eqitdfmf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2euvxppfs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hgnyghxh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hicpqiwk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iujjchaq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ujbihedy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2uhogxlpw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mlxwlifs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jatccyby.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fffyosqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyfrjkdx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vsubjgwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbiwatqn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ttqpwrqa.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uzogrgxn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wmikkzvb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vfhitnqi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tuvmzvem.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ozmtgxtf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ivkjbvmc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fgskcfvu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2aubrqiaw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tgxofxff.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vszcebrc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nifljslq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2oqabobqr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qnminvuq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2esraxrrq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ltjzkocw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2bnputrmg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2khflhoxe.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zdlyeghi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2agdqorrw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2sxxvawtt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hujktgfd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mpuajduw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gfwlfqsr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hhoepvql.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qxmjwmis.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2baifjius.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2spddqveh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rtbkgssw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qgtoitgk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2habbsnmj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nubxzlve.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tkzgyblh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2sbdltebu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2uzukfkjw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2bvkrvbkq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wqlnshtf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uqemwrcx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lznhytws.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pkvuqkjt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffmszvvc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bqkpnqcx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ieqbohgp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jpebxvxs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2lxumywqx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uktizabq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2usisgylg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ojmvljdi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tbzdzais.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2legyeazv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vkozxzyc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yyavibtc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tjerxmcs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lgdkldmd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ezfcgopm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vkkaiolz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gcnusjdj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lsspiwbt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wyzarecl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bxfwzphn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xmhzywog.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lmytnpmq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yeappgoi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hhfxdlpq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lfupiulv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vexqzsur.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pkoesabn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sxbiucun.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tvyrosnj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2hamghqgr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2lcgqqajy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2fyycfvvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgwvnres.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2rgepwxtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhrlvmav.html


<!-- 参考信息 -->