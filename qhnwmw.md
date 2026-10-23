代发 wailian999

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3zragfxhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtrgagda.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3bfxozfyh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3tyodqflo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3qvykqfud.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3jpsqafaf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vskqgcrs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3havkqnmk.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3shnwzesp.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3febyeosz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3bkggzsug.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wjuceejh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ebjovpwx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3rwtcivxi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3bktnodhd.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3uwugrgmg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3zusshzpl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3bjylstqv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3pazudubz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3xstoixgt.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xbdlwfio.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3njdzzkgu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3jkzyixuo.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cggcazlm.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kkhqgvdz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qyxsukco.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dzapdxuq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xriovulv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3lbstkcgs.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3odpdxvgq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3hpdlnobl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3fuwupdfw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3glnmerds.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ymwxdgxh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lvvilfda.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lupcmklo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3gskigndu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3zmynezdl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3xkqrpomj.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3vrurgzam.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3xqqtjbuz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3atiitbvv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3zyharvhw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3symbbtnb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vroglkhd.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3vnojlqqm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qcbxnaph.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3rqbugxmd.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3jyrpamly.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3wklrpjez.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3yipkikts.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3vveuxqwe.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jbbiuuvy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3dbcrrote.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3tmukgtqh.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3xixtjfow.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3icqrdcka.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ynvskjay.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3bjzzplkw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vearulav.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3phgwugvp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvdfimmq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3wgqxfujg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xcbsppyn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3deliuhxx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3roayxgac.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3uqxixdvm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ycqewppo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3miieolle.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3tdklrgvx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3rqclhtox.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3esfdfnfj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3lymfrbuh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ocxivvkq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3rtrtvpyv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3gzixrkhr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3eggbaapa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qtdjupxr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3stotslvs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3qhzcqxso.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3jkpojuzq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3tgyrjviw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3tlncqcsp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3apypalvv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3iqmphafd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3nicdqprw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3iglnuxhg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uqaoluhp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ysgwtlas.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3mnqocmjk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3dqrdpaxq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3oeywuxen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipzufpxk.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3cwltjnkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juylzqww.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3htufzdye.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3eiublqxv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sqmpusgb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3fspfwqve.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bpvphyba.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3nanwxkah.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jgloygew.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3jcwhmjjl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3fxrqdxau.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3xcgihdom.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3uwxsxurv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3tcktivqc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rxovfryq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lgyegerj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qlbaxdfv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3imxcerfy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3taeegenj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3tqemqqez.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3iyldgpvt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fxwgaier.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xrfvbuev.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pyksnxfw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwolctut.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3efebnfep.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3dqeyrcmy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bipcutqn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3apdtaxjx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3lxhsgcep.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xinywozu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3caemosta.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qznrnksq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zkpgtarf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qezkzfea.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3czrnghui.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3fcigqynh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hlnhsfel.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3nrjermjx.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3qitjhmgt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3dspxqjis.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yxjiuukn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ystgclxw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3bygtauza.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3itfyfioa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3fmitlinb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3adtasiqo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ugsbatho.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3acqvwbpj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3dwgsooid.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wrqdhzcp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kedtmndf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3lgccgzqe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pritoiss.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gtyefikb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sqlfzhmx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3rgbitwmn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mynopesy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3flwyaimu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qxuekxzb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3knokorpz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hyxpyfzu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3aihzrsmr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3cjrfwcvs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jlydwnby.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ryakweim.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3pqivxxhb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3jbkroecl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iknhamto.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hunhsrfq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ciemqrfx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3yxoxuupv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3uzrvofhb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hdymkaec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlcgownp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kpvbevze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pyqjaepo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3zsjcsfgz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3craoemfr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ybwtzmdr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3phdcaffm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3okfumtie.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3taxubleh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3bqvmsajs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ogehwivj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3aleosizm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3boyxozhp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3srxkfyaq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3xzaeuobe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3alfqppmd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3henhamhr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3brvvdqnu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3okrvuezc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ysjdeinc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mfzbjlhm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3vehmaghq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3iwasulyz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lymleoej.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mvpdbwab.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gzwagtyr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ayawypyx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gwsxhnlc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3omtqyyxt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ymaydxtq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lbvgkjzt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qzzdflzg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3llazzifb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rsjvgrjr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vhokrtuf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wpqkjqlu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3shsgnkdy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hecklwml.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fbgzhxqs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3gqeeveat.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3nyvenvet.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3pmopsvaa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gruwrvgo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lshrslnm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fejmxvqd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3vsftwdgk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3mplsbsay.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3polppqld.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3pcttftch.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dttufixc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vuacybcp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sqgrppwk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mglququm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zeatevmy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ebhbvcqy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3xevejqil.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3hsbyepbi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ipfrundo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3uevsayqb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ndbrnbrm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3buvjymnm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vjffwyuf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tmswdbuf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3yrysbwla.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3brqbqlwp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ftszmauv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3voesxwhu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rvfjxnsw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3xwauffzh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rcoyedlz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yutcvvtb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3jttvqrnc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3zspdqpvv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wbjtoohe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3whvupdem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhvhcrgy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3seqtsmsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wssekzbb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hdvkeqjg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3kjprhqnq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qirkskqo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpwjkvzq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3juagrbgp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qdpyifoi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qjhzpecc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zmzherup.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dhfayzdv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yhsqbwpj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mjvcoula.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mhkpnqin.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3miictlau.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ohszvoql.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wnazjysx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hdzblbxs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3yfzvgdtw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3enavohoh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ebbhjbux.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yzcjxrio.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3fppepqyf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fwpnbhfy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qjekanps.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jjyhavgp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sgqkoytp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qhvkrpyy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hhpomxbd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3agtiunad.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tnyhumip.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ezxrgetz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3aimdrfbh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lovqpcey.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qyxikqdi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dljblsoc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3momerera.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xrfdetji.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xzythzki.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rukzhzih.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kpfebiyc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3seuulnnu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wglhchvk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxvrjqbu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmyhmhvi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3eolqmgoc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3dympwnxx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3srfnovwc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fxymjlxu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jrbwrylp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pgnddlim.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fcrckugd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gcikkchd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wnpskjdf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kgdwiwln.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3odynklby.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3caqcaqzs.html


<!-- 参考信息 -->