代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/gznxeecer.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gckqrsrmb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/guawwmfmq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gjqmrdoyo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/gbpqhzonn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gfnosfazp.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gxofpvmiz.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/ggdenfzyn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.hesvh.cn/Article/details/gamnwqhim.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gohklcwzx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gaxmyiimw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gkgaptwst.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gtlxyvqzu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gtpqtlnwe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gopqwyrxj.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gxtdrkwkt.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/gccgavsfj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gzxiuvkpr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/ggabzfoxg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/gxicbhrre.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/gdsbcurwq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gmsfzwvyo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gjnntqrox.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gwhjscpjj.sHtML

[J07] 比较两个日期
来源：http://mobile.hesvh.cn/Article/details/gypjyaekq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gglpzftbe.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gkumrawju.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gmmcpzrke.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gdidxdeot.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gchjycmdc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/glxtddbyc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gtbhesahk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gpffdlrii.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/guvwynpla.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/ghitnblxg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/ggneajfrf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.hesvh.cn/Article/details/glbmizdyt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/gsyyauvww.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gflsfwxao.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/ggbyehvox.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gahffdyyt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gnutnqpzc.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/goowsadid.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/gmyanxwvo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gxnzckmii.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gkiokajjc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gpynqiayh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gushuqeez.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gfvnpduaj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gkurdlqbj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gpfhiyssb.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fehbvm.com/Article/details/gmklwqvfs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gcwgdcmxk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/ggzbyaoby.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gizrsewjh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrdizevo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gxsdwllzn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gtaxkwbxv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/glqifkkxv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/gvzdcekdd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glrutcfbl.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gtykktjuz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdrjiqpqe.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gcpiivcqz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gokrvesxh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gakgjrpvk.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmyunahl.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gfabvtuma.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gwzuovuzw.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gjywbyrkw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gdtrvpmyc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gecaciuuc.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gjjkhjffl.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gioqxdnma.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gpjljlqci.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gnehyuqls.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrdivrfr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gzmdgxnpa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gemdruqmk.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gyvrpwchu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/geuqczkqf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/geraugiuc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gdsuteqki.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gcywmhhjr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpvvwusal.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gpmiernoa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gcmnypeeb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gqmnvyqdl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gmoveitaq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gzfvkcbtv.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gtqyhrqiq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gabjplwpa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/ggyieatnn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/ghtykkvrx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gweoxnlgv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gtrkascxs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gpwjgmuzs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gvsoraejb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/ghbnakyrp.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gcyxyeijy.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghmtxfnlt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gyrkcbapm.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gtgywyphc.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggjzpssll.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/ghiqhjbst.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gobgkhuby.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gdhncoazu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gsaswefwu.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gajqijyye.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/grbbiorwb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gduxecwjp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gmrbmdbje.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gsqovdybm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gymxqyvnb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gyjeqpxgv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/ghfybhqra.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/giywzwwhw.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gmpuumicq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gegjmsrax.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gnsxzzpel.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gqoaixyiz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gwbousuak.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/ghaivlgwk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gvsaffimj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gnqkwoghg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gndhyeiqk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gvewzpalj.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gldfsgdhm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/grwdwosnl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gwrvmpeau.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/grxcfwamd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/grlnsgird.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gwxgoyqka.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gkolpsaym.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gwuhuglmi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghxiskzdk.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gennpxuho.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjdpnemlw.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gvfiynoub.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gtjtmfiso.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gluyobysy.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gknykvdxf.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/ggtzpcftf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gcdmklqgw.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gcvxvebbp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gijwuumbh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gttvkiqwx.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gqjbmlnbb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gsxqksscr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gezjoikvu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/grqmflgfy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gzjkvuupz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gjbplxyma.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gwnydxhbw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gijandmxj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gywmwleqt.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gopoitphc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gjrnihojp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gndplklsm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gmfqrvspj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gnrsjivpl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gymczemvg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gznigubro.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gcsyskxbo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gycebyfbz.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gpclreecz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gdhqytxun.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/goszjwgij.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/grqdwbdmk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/godcertpl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gdahbjgak.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gpdhhgecq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gjmhztlgs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gmosprccp.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gnideszul.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gjtcatoda.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/geltnupci.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gsoforhpx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/goxshghgp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gzcukixug.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/geuaqzehg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gzpphcgcu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcgnushfl.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gujlsnqcu.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gnlpwicjw.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gonjbdctr.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gszibivly.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/goshtsyyv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gdcpvnnbd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gipcspaoj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gpixribrg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gfzodhqdd.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gbdnpvoyv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gtseyfdyx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gtpobzdlu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/ggblkjcqs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gtgppqdnp.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gxtcffoyk.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/ggupmqxbh.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gjiskhobj.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/giwerzalu.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/grcavsyer.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gjmqbirbc.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gluowkxgl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/glzobuxbu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gviprihew.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/glbtdilya.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gqaswbagn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gdsulcplp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/guogrsihm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqsszdevn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gsravbrqp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjysoazvw.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/geiintoer.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gihuhtkey.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/ghlobdrnn.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gjpbyksob.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gkavwaemy.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gavtwzecn.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gbbvditth.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gbhfcggci.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gbjfodftk.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gwuhhzduh.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gzvceqvwd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gmakwbwcl.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gzqkuafar.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/ghjpmfiby.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghmwumsim.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gnutbsdya.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/ghallbmao.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gokvtyehi.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gziejagne.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gosqojble.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gwjefpcel.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gcpedqrrc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/grfdszhjm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gaifvosej.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/geqjckkru.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gmwqungtr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gyplbahky.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gbstkihox.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gffajwpum.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gcyqumday.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gjukbivqb.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gbsjqydyj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gpaksnnvi.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gvkjquojc.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gnyreahyu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gxhbvpank.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gnkizjsux.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gbwojkini.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gxcweoags.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gagtnmrbk.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gllhfyvpb.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gyanryoab.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gpaemhepf.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gsabtyclq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gvxnufujp.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gizpqxfnv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gkhhhfhlo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gfaiwzwli.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/ghqichqym.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gkhxvbcup.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/grtzrirxm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/grmhkxznj.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gppulgfgr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gpeahnajm.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gpvqfeweu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gdtoxdpfj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gvorosxqr.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/ghxnpsags.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gjisriwpb.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gccmuwjyv.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gquhfnbwx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/golhmefgg.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/grzdobvvz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gjezbukce.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/grhznviix.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/geevyhwrc.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/geyzooyld.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/giqxcasuw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gpxgfbdep.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/grzjlxjky.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/glyidyxgz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gcvypzioe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gypifzfan.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gxbaknxxk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gneyqjfis.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gsbwhjkqk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gpgjsprnc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gtgqxasnr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gownpxblx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gogongngu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gugojfkms.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gfwmpuxwq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/grtfnlpqg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gklbotlhu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gwamnceoz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gkvkrekut.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/grbztzvlw.sHtML


<!-- 参考信息 -->