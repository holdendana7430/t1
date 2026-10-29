代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gtexxcjnn.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gfqsfudsw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/gqvkrlgzh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gtrzuvjze.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/ggnplhfjk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/grcprfbxc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/gtnxylplf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/ghaufqake.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gismcduxc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gzpczabzn.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/gmyepcwbv.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/gzlplgnul.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/gchpyapqb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gaguwflhq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gatxlnywx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gcosxnjue.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gcoeqsmib.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gtnalcnqe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gzmiackap.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.zdbjq.cn/Article/details/gljamslho.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.hesvh.cn/Article/details/gztulahbz.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.hesvh.cn/Article/details/gqlrrwprd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/gctvwnglq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gdkrldixu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.zdbjq.cn/Article/details/gvjjlqpyk.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gwcwfupwo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/gfyjhksiu.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/ghxqyvmtd.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gnxwshbda.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gkydcclrs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gguerijsp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gajlmxdtm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gsdercanb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/gbnrzlunb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gmexrlavi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gfvemtbpz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/ggvobixfs.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/gmorirwxy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gjpyuakuf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gtywbhdal.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gufrspaxp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/ggkraxuor.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/gemaaisbr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gctzdfjnj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gemdwtudf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/ghnpzcyrz.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gcvkfgzif.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gqansdifs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gkezrznmb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gsxyzuwer.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gptolexce.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/gjesodoch.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gtnmfseou.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gwatygbpv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/guqlagfzy.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gmxlsixmk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/geawkmxcr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gynoxcobs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbctbcajm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gtezighys.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gltzxobyn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/gwcyfjimi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gzwhjaedz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gbjsnhgaq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqdcxmvrl.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gwyknveyh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtzootisv.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gvypiueyv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/glikobzdo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/geqvihooo.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gikhlijnj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvtdedrjj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/ggvermilz.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwdaihqn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/ghebxkbsm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gjwjjktew.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/ghyzsvqbv.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/goqxjclbs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gyouszqzn.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gocdqwclr.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gctpdvvlx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gnzhwvfta.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gomzlebqo.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gpkhdxjps.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gvfkfvsxq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gokejrutd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/ggzmvuqoo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gihcifcut.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gxoctjdrq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gvnulpsxl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gwjvpvvyk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gndnzlpom.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gblcafomm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/goujdhcnm.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gwmtssegi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gnevnoqgx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gxcufnzns.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gatlykgkl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/guskmtzlt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gpqkxvqpt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gmbdkshem.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/grxhrknhc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gwfbnobao.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gcnalxvpt.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gcptdfuuq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gosxmioqw.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gnujeeqnt.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gqqrrfclv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gizlhqyqu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gvccemned.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/geavejfzk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/guptsqrkw.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gkvoxykrx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gztgplqfp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gusifwmzi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gxywelxaq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gojsdikho.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gmwquqgxw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gshoopmdm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gvzzmnzjb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gaschtwrr.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gxeaxwbvq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gqmlvjcky.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gwbrlsdxd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gnvjsjmzv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gjubbqbfx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/ghvogsabk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gaaemnjbu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gbfcdetez.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gjpjcrxmx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/grjeppwva.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gfqqrmxua.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gsknivfew.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gnwfgntfl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gjneyhjjz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gzmbtkonh.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gfzkocwpj.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gjkgjiuuj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gjhioxwso.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghsppjnrm.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gzixysfpz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnimctawr.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gwqmrlawt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/ggkeqixgs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gtozdyovn.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gquerdunp.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gyxfkfmrb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gcqiukqwr.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gmlihczcg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/geuigxxgr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gyagqkzwl.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gzroldtoj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gtbvlaznh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gfcyvcdfh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gowzpzvvi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gyslsxlhv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gaayhmsyy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gatnzouvc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gbdqmptkn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gbdamhyen.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gboxkcwvz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/grvzynksg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gntmsmeqf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gqhbqetzq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/giktajemq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gxwsnzfpg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gfjzgunss.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gdejrfpgu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gokderuzw.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/garntpiqj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gnvyzqgqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gdanvvxsf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gmjesdhvo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/geiitmxnj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/ggaihiauz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gmkknluhl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gdnbmzsgv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gldindbgq.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/grlqdytbb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gjwwrxocp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/ggxahiqny.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gaialvoal.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gojbhvxlf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gudajkqno.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gntdtkvfr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/goptufvpg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gdsjgcxje.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gfoiobqsk.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/ggwqmoamq.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gtzmrqnay.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gpigzjxwl.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gtteuivcn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gelolgrlc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gufvcrmzk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gcncnguua.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gzxtwgexd.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/ggkrtlkoz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gsxusphjg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/ghuwomlzr.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/goytjvmja.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gxkiokphb.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gcguzialy.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gigqosaco.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/genpnqiiu.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/ggckayiuk.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gllrxetci.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gpakfsdby.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gvkyztwjs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gexomlulk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gfuyyhpby.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gijebbbxr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/guqsrkpzu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gquzgzjpn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gjfqccuvq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfxcjjlzi.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gvpbdshxd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghiycxtgb.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gnvvrsvxy.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gydfgtocc.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gypeenvvm.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gyicxqjda.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gekczztoi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gdabwzruj.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/glpfxtuaj.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gtrjbffpu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gqaexvnoe.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/geflarwfx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gnptfrqqv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gzljxzdom.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gwcxpocfl.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gblkeqdzf.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/ggwkimntx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gclwytqpy.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gqbgpwnfh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gpxrpvmib.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gkfaqaumk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gianoxwbj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gmbdyuzng.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/ggrcpaeyp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gqszhshse.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gcgrmfmfs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/goosltxme.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/glahwtoad.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/glhxcpcza.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/ggytbfmru.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/ghoeonrxd.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/ggvivnlds.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gfefpajyk.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/ggikyvjsr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gfbfwirre.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gvcubfryx.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gluopbtdi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/guybxsfdj.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/ghipfwsgb.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ghfjuywze.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gtrdzenlm.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gtcyvqjwx.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gsrabxkbs.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gtqgwuuma.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/grvxvqfjb.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gybpvvetg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gffmddwkp.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gjttkpyic.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gcziflhze.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gzrjahydc.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gttfntmti.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gzkctgemq.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gotgodhhn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gyumkchkm.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gfavobwce.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gezzisbnd.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gvucuxfmg.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gmxjoljsv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/glitvhdbo.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gfjwmkmvl.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gesubnbgv.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gvneiveab.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gxuqowtqp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gqoiqpuvx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gcgmpcqmr.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gtzhuaxsf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gpbvtuabq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/guuazfljb.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gjodfnioi.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/ghipamlfr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gxvqzkmmm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gafgtlfsk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/genqzfqni.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gmqisanma.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grlotojst.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gjxtlvgvq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmjjtvtpb.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gfqbuhnyg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gutqwtaox.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gpulvvjcs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gqcygvjxf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gfstcqjat.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ghmdhqkll.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ghzocxtpa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/ggntabmmy.sHtML


<!-- 参考信息 -->