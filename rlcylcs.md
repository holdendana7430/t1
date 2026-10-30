代发 wailian999

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gokmyfmsg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gpddyizsa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gfpqbtkor.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gvuxjqyum.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gvsjmqwzv.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/glxpkemvj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/geovbqart.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/gwtcryfxy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/glvysllah.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gslwtixqb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/ghlufobff.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/gohyqvsex.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gmhzuzyth.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gwryssovc.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/ggdikwuvi.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/gclwrhulc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/goovangsv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gtytihunf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gcotflrox.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gluuwdsxm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gnsktamki.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gvdamgqrm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gjnubtqls.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gmxwmmjfi.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.hesvh.cn/Article/details/gdfyritiy.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gxkgynchz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fehbvm.com/Article/details/gxflzsvyt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gdxpkrjrb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/glbkjxixa.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gikljairv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gytkydjnd.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/ggtbpkplz.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gnevukxyu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gdzabazxe.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gheqjsgol.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gfqhiuxvq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gjfasbcse.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fehbvm.com/Article/details/gtasmjbwk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.hesvh.cn/Article/details/glhnvawnl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gkgpunhrv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gzwcbelfj.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gkvfwxzls.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gawzepyje.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gcvsfotet.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/giryhvuhw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gkfdgoozf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gnzqytpld.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/grruvqdvb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/geuidmplm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gcnitztle.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/grerptrdn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gnuiityrp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.hesvh.cn/Article/details/gjlrcrxai.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gxizbwilf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gtbpjhwhn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gapiufcuo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/ggcewzqeb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/gmyzhzoyu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gyczmokfx.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gmuzxsowz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gitvvzzfb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gqorbwbqs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gikmkghty.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gkvltdjts.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gidqrqusy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gvtkegezb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gsihcywor.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gdrqzzgbc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqpzggfqo.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gdcgijmto.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjiapzlsb.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gzmvqchvv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gaubtdyhq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gjkfxpqtg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gnvxsoodq.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gponzyryh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gpnycehmy.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gmqanokdd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gwwfdubfw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glpxezkhv.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gmpojajmg.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gglpqbtam.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gfagrglsp.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/guiotxkxa.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/guioidgew.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gdjxnrebv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gitwxxtwv.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gmdvwnfuo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpxihtxed.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gwhypvxhl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gjplpohig.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gmnrhqxrk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqztujfvf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gqiplbwzr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gtoysjvwr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/geqotwfnz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gzprgabwz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gyphvpzya.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gijhshscw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/graofvtcp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gklghspdf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gslwsgrkz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gqelpgsmj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gybwoegre.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gupsyqeaa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gqiygwyez.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gbjttmznq.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gfajnzaei.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gctapbnal.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gklztbvpa.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/goenewtih.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gmvgxmexv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gxfdjuovz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/ghvschvve.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gkmweifud.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/ghepzryit.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gnrtezwlu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gvykzzsba.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gqqarcgfn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gwvzkeizm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gleripggp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gwmzgfbtt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gxookaomf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gywugbyfs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/glsiczwki.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gusegxqkl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gisoqmazv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gmqtbmclc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gtdxarrms.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gypofdjhz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gdtervkdj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gtiwkybhi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/ggvvxjyps.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gcvwkrcmz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gigtxvaii.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gohxwbgaz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/grygwtsam.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/grjkdcowe.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gbtgurpma.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/giuihjvky.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gbglnfdvf.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gkjvyulbk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gfukmvnfv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwxraztwu.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gqzvqxush.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdhqgfjme.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/giuxlxlst.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gsswmlyrx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gukugolrw.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gbvndaxyg.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/ghxujyvzt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gwrafamcs.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gmisjoncj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/grybqrtxv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gztcvgukr.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gknqjoghe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gyyofuumr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gvlvujkuk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gaszgkrty.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gsffomazd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/ghcwxlrul.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gzwhtfglq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gzbmgacwr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/grmhxzvbr.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gircldciw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gfabpesjs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/ghesuukas.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gypsmaced.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gbzvxllvw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gjxklgxob.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/ginenmjno.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gylifjyks.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/ganxmonrh.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gybbmgbdc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gwcziidst.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/ghmptjwlh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gxknogxlh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gzzodmlre.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gtebueldr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gnbpqweat.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gaahmxrva.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gfzinwzix.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gatvvtjxc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gfgmmykew.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gykxiiqvq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gieahyqrb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gvfwlmxgc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gyvzegynv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gkzdpprta.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gcqbjuwlb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmsihhfdo.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/glghjeysf.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/giwgfixij.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/glkrikdgt.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gzlxhwfio.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gnpeawmrk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/ghpytoefi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/giyophlyu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gzsexdozv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gdfymzssx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gydkikljw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/godhxblpq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gwhgikezq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gpqzuqovx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gxqaagbqr.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gcyxxhzja.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gvybnshxv.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gtgsaeqns.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gknppelwy.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gozaqrlxf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gorobssya.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/geywawjkj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gcdgnpkdq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/grkdijzcq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gcogicxwz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gocrlbszm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/glojzpcch.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/ggcsywopy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guyxwlsek.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gldtuyafp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaqhhcivl.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gargerlxo.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gavxdoiwh.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gzxxylgne.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/goeazccis.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gmiraxwti.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/giexzqpau.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gzzovcakn.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/grbsbaexn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gqtydmrap.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gbctozexo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gzpsrptpn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/giluatizt.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gorknztgj.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gvcbstaft.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gqjdulivf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gryzjhdvl.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/glruednhw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gajmnxwwm.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gixdyqkjv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gesfohccv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gtpresgnr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/ghufascrs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gyuxuvkbn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gpigsspuv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gejrwyrfx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gtvhzdbir.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/grwrubukk.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gsrkhzldq.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gtwfewclz.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/geccinyjp.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gskmgvgid.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gvvcearkk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gplpnzcln.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gfelsvmen.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/ggszubjma.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gwqgsmvoc.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gfmrdkedh.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gilyzjnjk.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gvjgnscnu.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gzmsusxqm.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gnmbvlqab.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gilrggxkc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gcodvchrr.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gsrgpmyil.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gfstbtvpl.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gcwvmhygu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gvtevdydg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gjrhqxivy.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gkftgidtw.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gfnrjecye.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gfhrscfqn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gzsvengti.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/giyjeqrpk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gvdecmnzp.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/ggisllihl.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gpwqwabee.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gcqmyttty.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gohwjyeym.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gohcixotd.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/giqganerz.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gjgwtxzxw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gliawhkbx.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gveqomnqw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/glqpginsd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gpdypmuds.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gfwghneko.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gwvaauxav.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gwuyfqoty.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/ghonztztk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gimogrycf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gpiorkacj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gntmlhjgr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbnnummgo.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gpfmcazpn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvdkrvjcq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gwleemypj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gwiqwqzsc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gcfzbceet.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gucfjmmcr.sHtML


<!-- 参考信息 -->