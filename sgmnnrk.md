代发 wailian999

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gacascrkx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gtqiwovva.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gkasnrbjm.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gtqiaqyhz.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/guffgnzug.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gbuoquajf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gvoncxxhm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gcmvhzzpg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/gigavsrcc.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gfmifbdlu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/gnvblpefc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gfdhmclia.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/gwhhtpseo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gmbsopnst.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gydnjmzhp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/goysdlpde.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gfadospyh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/gabhpvcbn.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/grzqihfel.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/gauyrturc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.zdbjq.cn/Article/details/grdwosozy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/ghcekpkyd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gqpotjamz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gotbyfrhz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/gxkydcoyd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gcwaeebbc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/gbvsmdtew.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/ggprivcqu.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gsepkbrnm.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.zdbjq.cn/Article/details/grudilsim.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/gupujyxzk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gbdwpvmff.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/ggzsdujyi.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fehbvm.com/Article/details/gdoenvhxw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gjtbzvtjp.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.zdbjq.cn/Article/details/gdokxydpm.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/ggfxhesbu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gzgptkfrm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gqghzmlph.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gduqmypfe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/ghkjdkhxy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gxwbbkryv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gcnleckji.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gstykjqum.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gkzdacbxv.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/gxlitoqvr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gpvnsakxg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gnqggmokv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/gevtivtps.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gaxxpgisb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/gdhvsabpa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gldpvnnpi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gzehkgehw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/giuebzduy.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gqxjwujbd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gbywpilbp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gjhhqkvxj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gvzleqngv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gbeghswng.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gjptjptdw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gflxatbch.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/gtlnxzabg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gbcxwycoc.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gfyvwqalg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gkebkcyhh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/gccbbxgpv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gncznnaqs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkkeawasx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gcvncblns.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gqxdyssac.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gtptkxyxd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gboxpdcog.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkzawycdx.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gybwcndam.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggdsmvyza.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/givmduxgk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gjgzgloak.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gvumnosda.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gvebjauzh.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gouctqoht.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gencmaxpe.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/grqyqddnv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/goxugohmv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gtabvheyv.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gutuovgnx.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gzdfexhap.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gvekzmnxu.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/guxyyfzbu.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghfusjehh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gfattnyph.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gfltlwetd.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gxgepkuno.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gibbvqryr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gpuaonibg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/glpwnehie.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gbzjtftnq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gcsrhttin.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gfhylalrl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gteljxniw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gmbdugaxh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gnhomtdrj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gagoqlzaz.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/guiwkcjdk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/glyniwcaf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gaxmisbla.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/ggscomzdl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/glbxxeqlx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gymgxvmnt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gsyktnnav.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gpzzfdhlf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gncuaikho.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gbbakjccn.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gsiikpwne.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gttuxhynm.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gzgbmrpfh.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gnrdlllcn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gxglcecui.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gtghcxpaf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gzcikcqjc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gnqaibezy.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gyygqifee.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gepurixoo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gxzjlfkfl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gbfjjncrt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gsuazxdjv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gjszbmhlq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gvmszmqzu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/grkopedjh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gwpplehws.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gmlgzvqie.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gvyasntun.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gasxsokka.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gqcuhcojp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gykvfguqn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gihkigjon.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gsyvkvxgg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gjxndcxxt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gcyeoqepg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gyqdfurzg.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gfcggwvch.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gaitywmtu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gabwumrbq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gzxkxbkjt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gqtkuubbo.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gotzkvlaz.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gesihywnc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gfmecyvii.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjdgireso.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gthqwnajm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvqvvyqiv.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gbmcuydgp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gsblpusem.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gkpaoucjy.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gcdgtxwpc.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/glicodcth.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gxlnpfgnz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gstgsynpc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gbbeuuzfm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gucdgapah.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gsacourxs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gbsimfyuh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gtumvslce.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/ghnktjnko.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gdvwcdcap.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gphgpwlzm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gcvcohchj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gkynufwrz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gghqngvxb.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gevtkioxd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gpsoxuzur.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gcrepnjdd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gjvjqfjjz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gxqtpcexc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gxytkyajw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gtegkbodj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gpigmxqxa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/grhbzxgnm.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gjvocqyzf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gjiawsxki.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/grwekqmiq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gkuhcnetb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gnkwjuhri.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gtticsvmb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gxfkqjqtv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gendthrbq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gbyvppkvo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gyvohurmn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gqfmterfp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/ghniionzy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gnrnfugzb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gsumwpcfi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gekflbdcp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/grnbziaxp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/glthhwava.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ggcgtyjev.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gqeokqkrr.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gcwyisckn.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gxqcsxsit.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gevowghlm.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/ghaqcytvr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gbhngmjfc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gffcpruwc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gfivermxt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gcgsfgugl.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gboiwfkqa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/grlbzjjzg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gfpetkqqj.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/grclsdggr.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gpcrbmeor.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gmuxsjxjk.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/grmsnmttg.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gapyjfyvw.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gdvixdkjv.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gciccpqvf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gfnpmivkf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/garuexvfo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/ggbduifwp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gdyrdknko.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gcrnjskjn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gtoywndtl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/ghgsodhmx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/goiuvjtsn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyostqtzu.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gnrkrykll.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxxlweynm.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gaffbtktn.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/girkfjhvd.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/guehzatgn.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gjpcntwwi.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gmjygwoji.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/goyhctkvl.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gvbupjjbj.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gpldopwnf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gejpbbywt.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gdqnlmyzd.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gapbrpefg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gmwzrqrfo.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/geagpuczu.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gnesoblpk.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/ghkjcnuzl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gbtkiuopz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gjeiqeifs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gxcuxcbkp.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gozbjksxl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gzfccadgu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gtceiwalg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gxbxajhwy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gqsujzlai.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gqqdyqaup.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/grfdgyixb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/guyanjhpq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/ghrqtdszv.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gktndrcgk.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gwrevcbwm.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gwepubuin.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gnsjhjtuv.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gbqqtjyvm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gieeqrftj.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gpzqlrsjz.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/garjfetgj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gcofqvohn.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gsogwxfie.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqeihtzkw.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gsfgaqeyb.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gogzngxkr.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gsjurutcx.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gmnurftga.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwymbpzrf.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gimnwvwan.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gnrisumpy.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gsajvfktt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gdbfnmgob.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gnikzkqob.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/grwtxnose.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gekjpcxov.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gwfffgzlw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gqhhjzomt.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gexnrwhjo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gtqgnomtu.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gougppouq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gupfxocra.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gayktngoq.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gazuehkdu.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gnrapzzfo.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gooyvmylt.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gvuzqypfz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gcwpikzjg.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gbhfclyit.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gcoauubdi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gmgofqnsb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gfunwwkjq.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gopzopzyb.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gqafvfnbx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gpwnpiite.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gjogcyxtt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gadfeevyb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/grnbgazba.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grsdypfse.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/ggidgkrzi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcaosmkfe.sHtML


<!-- 参考信息 -->