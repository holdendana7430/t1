代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gjmyhcahj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gsryzzwst.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/ggdryejiw.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gryfvevyx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/gyjpfxqnl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gfrfyrgfp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/ggorngltu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/gqdfwjvox.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gatdubmxo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gmprvwhim.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gkakgputt.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gtdozvver.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gjlcqiawc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gewkigipf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/gpmtyqnpa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gaunzskse.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gisjzfmvc.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/glfsbuylf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/govjfodwf.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gjezrgvds.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/gaxamenmr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gqokzehnj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gclczazjf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gzyoqwrid.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gnhomnvcd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/gcthewiie.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gxmnvdkgq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/glvhaaxeu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/ggugbtfoq.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gypzfeptg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gipsurlie.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/ggvxlutpa.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gpebkfogh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gkwnrkzel.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gzsuqwyba.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gcxmjljbd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/gfwslqfrv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gtqtsptzc.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gzzqiposm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gcjlirlfm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gynhgkejm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gnadmfcji.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gkhzpzjrr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gzqgcqnnz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.zdbjq.cn/Article/details/gkvaeffwm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gmzyqxzix.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fehbvm.com/Article/details/gmdzmzpfj.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/ghzvqvoea.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gyymihtat.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gtgtwsbmx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gafpydael.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gimpeiirt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gxseiupad.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gmfmrryas.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gbhtbyrpv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gdlndvjrv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjcrrllss.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gwbdqvjor.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwjmjqxyd.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gmimzlztu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gabpjlvuw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gmflbyirh.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gxipfsqjn.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gdtrorcks.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gjldoldih.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gpjajijqq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gfmptudnu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmkbpseac.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gzcsadelc.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gonvciizo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gyzdpgycg.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gzyupgtrk.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gfqulroro.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/ggrlgqete.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtoshdde.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gzbqzwotq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gkuzrqpes.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gxtpyfthu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gdntppitq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gzocuknyi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwtaegsub.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gntdptbpf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/giaveyfns.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gceulmiap.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gzhuqilrt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gpthxbzvt.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gkuumpqqv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gjegyuwbt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gqrnamtvv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gmxhwnopf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/grnmmvhia.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gcgytujcc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gbfzjggev.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/goegxutyp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gxztbqwgw.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/ghcequfmc.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gldodbuid.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gujpmyezl.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gqvmszfyi.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gknigfhdb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/ghcvvvmoa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gdogftcph.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gjswxgxze.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gllbzzptm.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/grbrmkmvo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/glvcvbohf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/giurghhey.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/glnhagvuh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gopbtbqxc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gwjbnsmen.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gbvcfcytp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gzkwbbvak.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/galworiqw.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gmrhptciw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gtlsxmlof.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gwjqpmalm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/grpatjlvp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gmkwyzfho.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/godmvpaoc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gmpatloap.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gyhvvvlej.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gwpapcelm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gfxtdsaaq.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gipssypkx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gsoynbbrf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gchvpjaaa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gvmctwloy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gdmxqrodq.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/ghbjboowo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxmkyjbzm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/ggtdrwhgh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwkslhjep.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gbpulctme.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnnvcotyv.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gefsgydyw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gvjvkzmdb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gumucrsks.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gffetxiui.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gziybrvjo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/goxkuaxwb.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gugmpvxom.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gkouhcenu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gcxbjiijd.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/girngdlii.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gdkrmobpd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/guwekbawk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gipjpunxj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gfmywyyya.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gzdhecorn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gwtcfzzfz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gxkpolexf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gplxknsis.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/ghmlukkvx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gkuqmbkgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gxawnqxaz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gixagwjhm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gwfdchblq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/guqoynson.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gspohosjd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gkmistnlr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gtokcncpd.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gvppravlq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gzbqaajsg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gnpvbqsvn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/ghggonqab.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/glgtqlzbm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gbzjbjiwh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gjgqfwsbv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gdeoxlvwa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/geepkizhb.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/godzazysu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gghsfmssy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gfcsqllqt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gahcolgyi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gzqsostnu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gunswiypl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gofhctikf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gpzhwlvfk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gryfgmnbb.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/godvxwhhn.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gjokkgeys.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gdmrkcqlx.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gfrlptfnd.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gptrrsdgc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gyhxbswap.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/glafrdhpc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/ggpjydqfj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gibhinrwv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gwzccuktp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gydhlhhyf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gabfkzoqk.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gfjpuofwb.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/granshkvh.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/grrruozwj.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/guarukesu.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/grujzreuy.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gqtuiyenx.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gmasuhfeo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gozismgwk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gwmiimclv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gvbytginw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gsrocwkwq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/ghstccdnk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/ggzgrxdro.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gafcyuopr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/ghwlisbll.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmutnstys.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/guqrzqkyl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guirudfhs.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gstgllkgy.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/guwfxrrdg.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gjaibpkda.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gqbznkhfn.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gclgyvhsz.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gazxkmfrk.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gjcveriwn.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gwgsytfvb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gzkjnjhfn.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/ghebxtyeq.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gqhimghbf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gbhsolvta.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/ggcybcgit.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gufgrqrtj.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gnjbjhxru.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/grxjqwcrr.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/ggrfpybiy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gqfaqwldz.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/ghftpgrjo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gbxgjnqyg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gfdqvtzfo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gzjhycbfg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gevkgngly.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/guyjifteu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gahvjacjv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gwdbigsys.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/ggusyklxp.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/goymkmrdv.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gwsklolmm.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gxudsavbv.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/glzmeylyd.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/ghuuymrwp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gbclvpazw.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/giomiwvkg.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gbflkelit.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gptdzzhkn.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gkrgwmqdw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/grofnkwse.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gyrcveyqf.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gamcbqdnu.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gxpbgjvrd.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gotqbduvm.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/ghmdvkrap.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gabwkbqii.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gcmgmaiyc.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gfbfkvwja.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gpvzhrmyk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gyrixqyle.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/grspykeqz.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gsrfudjpk.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gnmvifupf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gdurxbkgl.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gcapzayvm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gdjhrdfpw.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gfjomcqyi.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gsfmwentn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gsyvctgzy.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gxkiflkua.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gpixbbkne.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gnykvkvgm.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gicqsztpy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/grmtvqfbp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gmaosmzff.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gcngeljro.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gzakpqxbd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gqmhlbxpk.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gnonfmumo.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gnzypcixi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gbeakdesj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/ghjasrvoh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gatgxodsr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gsvcexnkx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxdkvplaz.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gozknczym.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzrlyabth.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gugkxtixm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gjcqmhfji.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtontdvwn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gitlrqwmy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gezrpingg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gxlkzofnm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gaejuyvst.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gafwwswlt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/ghmzqnzrb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gutbwrrxi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/glppffmei.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gxxgcwjtz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gvzydxlqo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gkzfvfdzx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gpksusptm.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gjfborckw.sHtML


<!-- 参考信息 -->