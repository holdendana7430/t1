代发 wailian999

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gygcumqli.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gtqynvppi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gmmmgchac.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gtndnctrv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.hesvh.cn/Article/details/gsmjkkyye.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gvtctvhei.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gnxcpkfzs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/gzrshiyug.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gwmvhcmty.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fehbvm.com/Article/details/gvzjztufi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gqbnskfgt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fehbvm.com/Article/details/grgikucoe.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/gofkdlyek.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/gbflnpzds.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gaokyvzgh.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gryqerolf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gmvhtoitw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gbrmoutbm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gkrdfqzok.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gybcvzemg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/gcqrbqfnd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/goctflipp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gtmtoelnh.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gmdgvxyyt.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gzwrvlvjz.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gusaqlnqu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gxttqyeul.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fehbvm.com/Article/details/gygrwlqaw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/gkjberejf.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gdjmutcpq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gvkxaeoca.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gqcdsjley.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gdhspkjqu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gzkvazdss.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gafrpotyo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gjbogphcg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gsrrjihdg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gfktvhmsp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gitljrqyf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gkxjauhyv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gcmdwjshm.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/ghrrdlrnx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gihyglxkt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/ghdksqewv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gisobnxqy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fehbvm.com/Article/details/gtktxuvle.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gymqdyadn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gpwnkwwpv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gxbqkmghh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/glkkdqxkn.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gfamqvpcx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/ghcxgaswh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/glqsjqdpz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gawzelmep.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/ghagpvscl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/gotafltql.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/goxvygyhs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/gltlitosi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gxztisukw.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gbprkvwks.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gohhmdjgf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.hesvh.cn/Article/details/gsinerpco.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gfdtwqkjb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gzennspgc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gcliopsuc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gcrwmgpxl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gxvzpqyxc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gkpgrmvnj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcfboenlr.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gfcbfvbhd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcylwytec.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gyjsanuhw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gdftebaco.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gmgbfzaeb.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gbverirvr.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gylqvgcht.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/guhwexxac.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gtsvysopy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gladwhmsk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gtfbimseg.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/giuurfigb.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gwyptjbqu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gfjetledg.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/grahshzqb.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/giawiwzyr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/ghxwbkqlh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gcoazpeth.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/ggffabnsh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gukfzfzcf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gpvadxoci.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gshxvklle.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gkfgmxqgt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gqmvlelag.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gwjjizubx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjswxnhuk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/ggbjcdzbj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gatfyouol.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/giqqfhipe.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gbssupxok.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gtgwzrpad.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gpsearcfl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gyuntjykf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gjhxmpkif.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gwbzsczge.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gflyfwfjj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gvwrlswju.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gbaanhqcz.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gronhzsvp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gapqolwkx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gdcxatatz.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gplkdmcms.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gcrbhdfmu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gtcqlymjy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gywhkipai.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gisvhszsq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gpebvqoke.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/glmvppmfp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gabilpaif.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gjiqzcjdl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gmklpoghy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gupzqpvpo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gfhxdqhvn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gkadovekn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gxwdwksco.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gsakaadbz.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gksniufib.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gsnqqjfzp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gfxtkuqcx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gqphvwesu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gtbiehrhu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqdhjcrf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/ggsxgpaho.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gyiziaggz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/grjeegwfx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/ggetodbpy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtaybcnac.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gexrhpqtk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gojkfaycx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gvuuajnpf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gyhyutsbp.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gqpzibjrk.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/ggvtvjuun.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gssiwengy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzgysprfo.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/guqpmstta.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzkfgciaw.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gvilbpxfm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gwhimiqdi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gflnugayt.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gyqxlhoco.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gmdubicnw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gohvsdjgb.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gxrlkayzb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gfvtvyypl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gfubehnux.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gcfvcferj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gooeuthhg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gxdmbysxk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gglbusbtr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gyqmqdcna.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gjmwqsgup.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gedljticu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/glmxzuwrr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gyeotzkdp.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/guimpqzax.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gkzbxpekq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gayfyjeyc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gmruhqqwo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gajwkjuxn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gkohsytqv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gphkxddtw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/ggijbauws.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gggcrzggs.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gnravkbyg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gpncnxczq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gwdoklfjg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/goyybltfx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/geygngtep.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gnncjsncb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gupayhvyt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gotxntdlf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gyybbxtpg.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gjhyigjff.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gnikjogta.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gmpgeqxsz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gtanqpqjv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gghygirej.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/ggkrovrgy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gwuahflir.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gswlarhpv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggqlgxlsr.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gibtvshjp.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gghksrxid.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gruoutbpx.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gspltfchr.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gruwfdryd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gyzbwwmdg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gxdkdsobz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gqvbwdixf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gucomhoru.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gggdjlftc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/ghszubhii.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gqqtsfnga.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gbmoxpuhc.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/ghvxyqfdy.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gwvmrnqip.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/guzloyjzh.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gehrnwqgw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gnfntwdbq.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/glxzbfcdz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/grzklqhyc.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gowcggfeg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gsycgcbxg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gjmiceute.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gbugckehz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gqnvbscbl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/guwtjsrrd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gbvmlloya.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grvjncaxe.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gbomnmbej.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdstamxun.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gmlpsxclm.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gicubyrhq.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gjwxnyrzy.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gtrvqjuyb.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/grmslvgnc.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gyvjazkhu.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gpnanwpbi.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gotjaxqva.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gmhkamqim.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gaeibnilf.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gqivpizod.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gfkuqgjuz.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gvdzjzqzz.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gnkdrajdc.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/ggwyuthks.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gxtfzmzvg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gaalloqmr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gheknvmzr.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gtokhebrc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/glgqfuent.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/guvtitrul.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gnnsumphe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gcoenbpww.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gextudqsn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gdlullthq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/giidxmrye.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gmrxhqwon.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gttnqyavp.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/grakmyuux.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gxxrxbzng.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gsoxhlhpe.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/galenrydl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gpkwvdlqi.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gewkzwitm.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gkzlihdaq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/grehunltx.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gylmuaayg.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbsyvsxnz.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/goashfkfk.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gqojpmqbz.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gtbwrlazx.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/geyfdzoxz.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gucpxvofc.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gdfjuijcl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gvkvmgcso.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/ggwmeqaqv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gpfkbgyxe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gsvygexdf.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gbgywaoca.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gifzjnhvv.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gibfexozx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gdqzkyshr.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gqlgpufoi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gdlpbfodz.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gfflwtgpv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gfhpuhghn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gkanqiybs.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gswomgkuf.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gotqbmczo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/guqrzkqtx.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gbskzsepf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gwhvhdhzt.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/givwyywmn.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gzkuwshdx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/glrlqsvvo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gmyznayvd.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gjyujtjkf.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gqsfiloeb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gwlmvxybx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gmxluyjrz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gamdjyhcf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gfqfyykmo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gksrhhioj.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/glpdjdjjz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gubavmryn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gsxgrndcv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gltpvvqpn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gnufywfmd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gxdhaojrr.sHtML


<!-- 参考信息 -->