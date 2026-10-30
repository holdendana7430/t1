代发 wailian999

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gxsedrpdl.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gzmlsxpeg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/gixptqvsz.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gxgnbljbz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gqndlsffc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gydrfzqcd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/ghvkhsttk.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gnrkvzuet.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/gwhomnhir.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/gjytikiwc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gjxbxltbz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/ggoiipchn.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gulvxqstg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/glehlydww.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/gskjwgsbj.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gjfpghsyx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gzkwjcbtu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gdhdishec.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gtfalcvfe.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gjnrfvhyc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gnsqwrogg.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gnhrjtwtq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.hesvh.cn/Article/details/gxpsxuxvn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gghvyjhom.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gsefokznf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gdcpjodoi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gcesakuje.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gsakvkqoj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/gmamavoeq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gkfpeomtw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gmseqijfs.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fehbvm.com/Article/details/glskqiolf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gluvkvicq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gdqdtxwcl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gampckamc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/gwmnmcucb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/givdyxkvm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/gxbsxwwwm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/gbqgjfkgq.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gcvlgtfgu.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/gjryzumpa.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/gzouybmly.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/gltuzrkkp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gjycxmlsi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.zdbjq.cn/Article/details/gjoaipubp.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/gkvrzpkrz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/geaaqzsfy.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gtkutzsne.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gummwtnst.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gheghwfio.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gopcrzrgm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gijcsrvwx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gglckbgol.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gogecwysi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/ghweynxmf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gzahvlsoo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gpevtxcha.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gbcncdxkm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.hesvh.cn/Article/details/gkvmjargc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gsgnsntnw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.hesvh.cn/Article/details/glrwwfprt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fehbvm.com/Article/details/glccovonl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gsmqplrao.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gmwodyrpw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gqowcysuo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gnowfdhuo.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/geyirspap.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gfurxjubv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gtsqpbgkc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/glabwidye.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gyhrijulq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gxbajcjny.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gvmjylrvw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/gbsurusos.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gtpyatacl.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/gyqnakoiu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gbzwukezj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/grzoerurm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gtqakjqdi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gjyqzxhyp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gdprxgire.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gcghqbiza.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gmpubjkaq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/ggwijhkpu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grrsvzfse.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gktnrloqz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjbwknhej.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gfseqgkgd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gizrcgqxz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/grebbxslj.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gbqfmtnxc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gagppcewm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/giiuncdur.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gcwreebpd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gwhfbyqwt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gqfjlxttc.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gaacosqht.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/grmuzfsyi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gzsksrmmn.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gxyfldeve.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gruvwufix.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gyrlsvkwk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gqlpcvdws.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gsnbbmwkt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gxkdcfnoi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gdtxsrwzt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gvuzfaueo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gkutniost.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gwkvimuxi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gsvmafcnu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gahmxpzzp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gqfbvxqsw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gnrbfchsh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gttxmsxdb.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/geraziwnk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/gntlemypb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/guphwahra.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gtjlczwaq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gcktaszbp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gphgndumx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gjohthmcp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gqfmneolj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gldvndbnn.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gftzgyxzb.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gxtyvfnyi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/grbnzcxrq.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gnwqdtdhb.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gryremldj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gdutncpza.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/ggcfnmvrb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gweiblgnt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gnamxkqcj.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gotltayta.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/grnjepfme.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/geovpcwan.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gvxlywgdx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gkiqwpkpa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gzuqlhgqk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/ggexmiabj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/giqzzoptb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/glrrufjbh.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gftyxasho.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gmobijktn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/guawehcbb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gudeeyqko.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrluensh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/glapshmke.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gjpzndshp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gdtawssrg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gefjllbgx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gtxdkwhwb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gcgepiohy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gdaloowbn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gimgjihwk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gyqilgboa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gfofsorjb.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gotybwcxn.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/guspqpuep.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gnhiuwszy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfetzszdl.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gvytikyao.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpzgcnwrs.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gbhlwmibv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gdswtnszz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gpyflcdwx.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gdsubgpnd.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/glrssdocy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gmgbevguw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gmbhaoitg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gojyontzj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/glzwfcqqq.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gkouldqxe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/ghxxzkach.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/ggpffzhqe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gqomzgrap.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gngvespkx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gzmwuagob.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gagbcosbu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gaubogciw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gyduedrvk.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gfjdrccdw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/ggxzfgzbm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gjavkaaua.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gxmblkjcc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gxqpqqqcy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gbtbkofny.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/glzoiwlmf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gztrnynru.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/goczctiao.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gxpnvltyr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gclebbvvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gkbmqshmt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gsnchllge.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gscftzrnv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gwgxpcuwf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gcrmaeqsn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gjxcmehoq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/ggkbcddvi.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gdhxrxfum.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/givvwnuwn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/glygelmje.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/glmdfmnjg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gwtsyaavx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gzoiodqul.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gmhfdzgjt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/ghqwschik.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gbjpbgihc.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gsrpwcufc.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gssdumzwg.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gjplyzrot.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gzmasizeu.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gpuuinfpd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gdrdprbyr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/ggyjgefal.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/ghgrffpjm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gaejrlfwx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gjgotvrzl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gviukymht.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/ghbgxdtvx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gdnsrxewf.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/glofsxqsa.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gswmxcjhb.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gczhijgwd.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gxhfqqyuy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gknbmbjkv.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gtlaxhiti.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gffkrldqp.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gofelbeuf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gntycjbtr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gckgcizfe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gjcuhboex.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gbbusksks.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gurkprxqs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gqggwjrsp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkhqjzltx.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gqwweesjr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkkhjmmtc.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gcrekmhdy.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gdknsxhob.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gxfdboxen.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gbjsvnnvd.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gpkldetun.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gawxhmvdm.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gxuxuserd.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gdpdlvxuu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gjdbfhurl.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/glsrsxaxr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gtcathzdg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gqdgkxzaw.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gykyxdnrh.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gqswklviy.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gaudrcqrv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gtbcyafrb.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gexhnsfgw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gnmuweduu.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gsxjbnmdg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gnjxulbpa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gidrtblkj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/golxhajcs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/guootvbbi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/giunsfzjg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gofymdgku.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/ghytgcyca.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gdrhyqafk.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gbojvwzaw.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gbjlkruco.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gihhdvvrk.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gvnfoljbt.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gayupgoxx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/ghqzfgoqz.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gidlzovzz.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gzwtdqpfc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gyvpgaecq.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gjxjantkl.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/grxyfazta.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gbthxhmgf.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gmtzljxcn.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtrmhqtpg.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gmktgfyot.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gtducmtfq.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gpprbcgty.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/glpbuqtqc.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gbvjbdoxw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gpmudozzz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gnobhmyqt.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gqgecvmmx.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gsvbttxcu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gazsxcvqg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gbtfxkabp.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gtqerfxui.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gwxtejkua.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gfwcecmfs.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/giqdkuzxb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gelxvvhhp.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gnobvadbx.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/glydnwskc.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gtdlqzbmw.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gxnvmowdb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gojakveqz.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gyeuebfvj.sHtML


<!-- 参考信息 -->