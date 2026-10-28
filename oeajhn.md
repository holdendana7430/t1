代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuxming.cn/gtxbiljqxo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangkeji.top/gtifgsuzje.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sweek.top/gtxswgjbak.html

================================================================================
来源：http://hz.havefunace.top/gtomotpqgi.html

J. 日期与时间
来源：http://hz.zdqjudy.top/gtscwvqjxp.html

================================================================================
来源：http://hz.dianchejie.cn/gtitnbhpuj.html

[J01] 获取当前时间
来源：http://hz.cqqwz.cn/gtjbxplhoa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.redwolf501.top/gtmxtfjfln.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hywenlv.cn/gtynhhjste.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtkqhkbpyt.html

TS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtgzjtlyaq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sysykeji.top/gteyqzprjo.html

Go:   time.Now()
来源：http://hz.ydzc1.top/gtkipxalxo.html

Ruby: Time.now
来源：http://hz.yuxming.cn/gtcdxaguki.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhixingplan.top/gtlhhmijte.html

[J02] 格式化输出
来源：http://hz.52xcode.cn/gtjczbsvbg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtmroexddm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtxvnpcjbn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnxiangtu.top/gtbgscvldb.html

TS:   d.toISOString()
来源：http://hz.jianghu66.top/gtmrvuplic.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aizwys.cn/gtabxlsnam.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtwspboznw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gtirwnhdrz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenjidiqi.icu/gtlwsogpsn.html

[J03] 字符串解析为日期
来源：http://hz.andypj.xyz/gtbqexgwxk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtmsoutsmh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigufen.top/gtievsbifq.html

JS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtcvamjave.html

TS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtvlnhgtpm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtryrvdxwh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hnqzz.top/gtdvfsiklb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtpexfrlig.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.dashuyun.cn/gticeticgq.html

[J04] 时间戳与日期互转
来源：http://hz.jyoumei.cn/gtggzpofpl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.feifeiyinyue.top/gttmhfpsqp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuetiantiany.cn/gtvzgrxwne.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shuidangran.top/gtzniscaxo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cucudq.cn/gtzuohiedg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.birdmap.top/gtnzzdwmbc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.guowangkeji.top/gthgjicinf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtjkldsath.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tianlin.xyz/gtwldexgrw.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gtqakiqtdf.html

Py:   now + timedelta(days=7)
来源：http://hz.aibaodan.cn/gtvzfjswxj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xinyue.icu/gtkhakpmpd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtgqtlpqnp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtbnbdqfkw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sysykeji.top/gtnbbevuad.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gogol.net.cn/gtfmrhiuwf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.316326.xyz/gtgtcljbvb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.havefunace.top/gtmbzgzegr.html

[J06] 计算两时间之差
来源：http://hz.cdnleiting.top/gthmrbzzsd.html

Py:   (end - start).total_seconds()
来源：http://hz.jinghuilouyu.cn/gtlcufkwvt.html

PHP:  $end->diff($start)->days;
来源：http://hz.0kj1m.cn/gtvpjkmiql.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtipfqoplr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj202588.top/gtgcuurjlg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shzxlz.cn/gtclwhqckn.html

Go:   end.Sub(start).Hours()
来源：http://hz.c1oappe.top/gtornrlxiz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhaomingkeji.xyz/gtgdfmwypb.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258888.top/gtuabypiow.html

[J07] 比较两个日期
来源：http://hz.pycfn.com/gtmualbndc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtsehmixyt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shuidangran.top/gtjciewowq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtxmhgpums.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtmjpqowqj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.feifeiyinyue.top/gtbtyhcbmw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangkeji.top/gtrbusffeh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtwlqhjxnp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtewsejysx.html

[J08] 提取年月日与星期
来源：http://hz.chenlongwang.top/gtsqnxxwty.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gogol.net.cn/gtjuqhhpzn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shuidangran.top/gtnodhrolz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jiagoushi.top/gtccyubwem.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jianghu66.top/gtqmhnrszv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nanxuanxn.top/gtqsgvutkj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yongpay.top/gtlghtlvgx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258888.top/gtgbnzgdkz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.iojbl.cn/gtksfgpfnf.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtpfgarstk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.feifeiyinyue.top/gthyhnhbza.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.c1oappe.top/gtqukkebde.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gaohongyu789.top/gtcswlyfzy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtaefmdotg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tanke756.top/gtgavzatyz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.c1oappe.top/gtqufdrfbu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ivvv.top/gthqmcuhvz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aibaodan.cn/gtxyzanpmu.html

[J10] 取今天 / 本月第一天
来源：http://hz.shangyingyoupin.top/gtccljytol.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cashguo.top/gtiesqapby.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtpulxtfqu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gthgrnkgkx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtpapkucih.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guowangkeji.top/gtrbssuyez.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhaomingkeji.xyz/gtiwcrykpw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jiagoushi.top/gtphajshim.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.snrcjt.cn/gtoartmdvt.html

================================================================================
来源：http://hz.yj20258.top/gtoatofhki.html

K. JSON 与序列化
来源：http://hz.316326.xyz/gtrqqlqcad.html

================================================================================
来源：http://hz.pycfn.com/gtkjfjclso.html

[K01] 对象转 JSON 字符串
来源：http://hz.feifeiyinyue.top/gtkqrvwgyg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtunfpaizl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtyprbgbtn.html

JS:   JSON.stringify(obj)
来源：http://hz.fzhhl.top/gtuyqpefcq.html

TS:   JSON.stringify(obj)
来源：http://hz.hfpthk.cn/gtlxnehgrw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.feifeiyinyue.top/gtjyilduii.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258.top/gtywsayamz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtghwvopnk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hammf.cn/gtfavaaisw.html

[K02] JSON 字符串转对象
来源：http://hz.cdnleiting.top/gtcyybjxti.html

Py:   json.loads(s)
来源：http://hz.nanxuanxn.top/gtfzcigdar.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.svipenyu.cn/gtswcfoteq.html

JS:   JSON.parse(s)
来源：http://hz.hammf.cn/gtdpyinoag.html

TS:   JSON.parse(s)
来源：http://hz.iojbl.cn/gtpdootnhs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.andypj.xyz/gtkbmqqsbp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gtkvkrungl.html

Ruby: JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtkfbkmggl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtsldumiti.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtksfbxpdv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.316326.xyz/gtczhowewf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtsanomnai.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gtbwutixxd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtxdxuqlte.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.mhx1999.top/gtnbvsmqcj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tianlin.xyz/gtntpwwolm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxuanxn.top/gthtltdhub.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtvwgcshil.html

[K04] 读取 JSON 文件
来源：http://hz.yuxming.cn/gtdasodldy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gtnkjelbyj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.0kj1m.cn/gtebrobpgo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtlhdnordu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gtartbutjc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhixingplan.top/gtczwtvdlv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gtnnesokak.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yongpay.top/gtzzollyvr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tianlin.xyz/gtkmqcnreh.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtkklwiwoo.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtmkgeskzl.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangtech.top/gtthppcmbs.html

JS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtyzgcigil.html

TS:   structuredClone(obj)
来源：http://hz.zhengqikj.top/gtisyeorqk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.feifeiyinyue.top/gtegybcqcm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtqqrfcviu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhiwuduotai.top/gtetjiumdz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shangyingyoupin.top/gtftkjimbh.html

[K06] 解析 URL 查询串
来源：http://hz.tian-w.cn/gtqumclscw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhongyouzk.top/gtfzhgvnxu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gtszrptyol.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gthwikkbxt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.quarkkingdee.top/gtwjvybhga.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhoulong.xyz/gtsxvtixqk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.pengpengdd.cyou/gtnayazvla.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxinkj.top/gtzliqloxj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zycfv.cn/gtpkbrzmwp.html

[K07] 进制转换
来源：http://hz.zhiwuduotai.top/gtzotrwqsh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gtdsbpkvkj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.iojbl.cn/gtqbtlcqyp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtehmloinf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtmesfttci.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtsrbvepxg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtkrgaseqp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.52xcode.cn/gtbebxbrfj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgufenzy.top/gtdzptbwcf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jiagoushi.top/gtndshsiag.html

Py:   pickle.dumps(obj)
来源：http://hz.cashguo.top/gtqlpxmlks.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pengpengdd.cyou/gtvudtdgvk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtqzagdfuy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtepfgextn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgufenzy.top/gtgtatgzri.html

Go:   encoding/gob
来源：http://hz.fengsongda.top/gtgwuekzfg.html

Ruby: Marshal.dump(obj)
来源：http://hz.wangshuangyany.cn/gthumrqfkr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxuanxn.top/gtzceqgvbh.html

================================================================================
来源：http://hz.iojbl.cn/gtfwjlmofb.html

L. 网络请求
来源：http://hz.xinyue.icu/gtqiuficwx.html

================================================================================
来源：http://hz.andypj.xyz/gtmwqdhlmz.html

[L01] 发送 GET 请求
来源：http://hz.fzhhl.top/gtszxxjeaz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jlsjyb.cn/gtldjsgfup.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.bjfxy.top/gtjghupglu.html

JS:   await fetch(url)
来源：http://hz.tanke756.top/gtgmguvxoz.html

TS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtbzziyctc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xingfuxueyuan.xyz/gtsgxyljhl.html

Go:   resp, err := http.Get(url)
来源：http://hz.dianchejie.cn/gtguyyzysg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xylfe.cn/gtrhqqkmmj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtboiqhedt.html

[L02] 发送 POST JSON
来源：http://hz.andypj.xyz/gtvlbhleqd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydzc1.top/gtjdbbfwpw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aizwys.cn/gtzvixfufz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtbjekxebl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.kuanghao11.cn/gtpteebcab.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nwbrower.top/gteuvmzewk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gaohongyu789.top/gtknqldcrv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cheryme.top/gtzemzdxua.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cashguo.top/gtqdmwbpwx.html

[L03] 设置自定义请求头
来源：http://hz.zycfv.cn/gtpzyqrqpp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tianlin.xyz/gtjntfudzm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gogol.net.cn/gtzpbdkovi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtogfnzumm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.svipenyu.cn/gtqbasnkuv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gaohongyu789.top/gtfueuzaqu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nwbrower.top/gtpbbagxpi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gzhubu.top/gttpfjbufs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tianlin.xyz/gteajxsjgk.html

[L04] 设置超时
来源：http://hz.cheryme.top/gtqgzmympd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gtnszfnuoi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cdnleiting.top/gtkxtbtddv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gtdaeikhqn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtjldnhjiu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhixingplan.top/gtwesuwghr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuxming.cn/gtgndkefbl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuanzx.com/gtngguoazy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinghuilouyu.cn/gtdvqvlrwv.html

[L05] 上传文件（multipart）
来源：http://hz.jqgfzy.top/gtwuneekbv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.haohaochexian.top/gtohmrqwsh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yonumen.top/gtgbqgkekm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtrfztvvyx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtxilqxpcg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yangfankeji.com/gtfhvmtgvg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.0kj1m.cn/gteoqyltmi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigufen.top/gtagwubswj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.pengpengdd.cyou/gtmilnkctz.html

[L06] 解析响应为 JSON
来源：http://hz.snrcjt.cn/gtuxjnqasw.html

Py:   resp.json()
来源：http://hz.guowangkeji.top/gtxseuojua.html

PHP:  json_decode($body, true);
来源：http://hz.kuanghao11.cn/gtxptyxxys.html

JS:   await resp.json()
来源：http://hz.haohaochexian.top/gtmsuulckf.html

TS:   await resp.json()
来源：http://hz.tian-w.cn/gtsxgqoatr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258888.top/gtfpumeigj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj202588.top/gtkmhnsmes.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj202588.top/gttinkwsqb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zdqjudy.top/gtjdgkqvlm.html

[L07] 处理 HTTP 状态码
来源：http://hz.yongpay.top/gtlnsohbvi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.bjfxy.top/gtuskkzari.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jianghu66.top/gtsvdewdzr.html

JS:   resp.ok;  resp.status
来源：http://hz.yonumen.top/gtyiaxzlfb.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtbriqeekm.html

Java: resp.statusCode()
来源：http://hz.vqdsnc.cn/gtlajnmnti.html

Go:   resp.StatusCode
来源：http://hz.dianchejie.cn/gtuaehgoyb.html

Ruby: resp.code.to_i
来源：http://hz.ybcxt.top/gtugevwmva.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxuanxn.top/gturfftdyk.html

[L08] 并发请求多个地址
来源：http://hz.jinqigfzy.top/gtteouldti.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shzxlz.cn/gtpjylvzui.html

PHP:  curl_multi_init() 系列
来源：http://hz.smart0.xyz/gtpxefsphb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gttacqxjrx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtrretuwjh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydjk.org.cn/gteqmvhgwv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinghuilouyu.cn/gtaxuchori.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shangyingyoupin.top/gthmljvsbr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.aizwys.cn/gtqsfogauh.html

================================================================================
来源：http://hz.hammf.cn/gtkngijcoo.html

M. 命令行 / 进程 / 环境
来源：http://hz.xziqi.cn/gtrfdqzmrb.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtkqiafhhb.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtctlemnvb.html

Py:   sys.argv[1:]
来源：http://hz.9152youxi.cn/gtyglnpjkx.html

PHP:  $argv;  $argc;
来源：http://hz.jqgfzy.top/gtgvjzxpia.html

JS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtcrqggdtb.html

TS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtuvcawruj.html

Java: args 数组（main 方法参数）
来源：http://hz.cashguo.top/gtucztzude.html

Go:   os.Args[1:]
来源：http://hz.jinqigfzy.top/gthymqvzke.html

Ruby: ARGV
来源：http://hz.shanyushiyangtech.top/gtsgdvbseu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtsfhckhhf.html

[M02] 读取环境变量
来源：http://hz.haohaochexian.top/gthzunacep.html

Py:   os.environ.get("HOME")
来源：http://hz.shanyushiyangkeji.top/gtzkgokrzd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.svipenyu.cn/gtyhrkjpjv.html

JS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtqnhzikqm.html

TS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtpmogaphq.html

Java: System.getenv("HOME")
来源：http://hz.aizwys.cn/gtxjnhlyhu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtmummrifx.html

Ruby: ENV["HOME"]
来源：http://hz.hnxiangtu.top/gtcvnyqxku.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangdashe.top/gtyxusrovd.html

[M03] 执行外部命令
来源：http://hz.yongpay.top/gtjxwrbsli.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hnxiangtu.top/gtzkbbavcl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zycfv.cn/gtjzkstddp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtthpdnrqs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtonevtmpt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhixingplan.top/gthvqpzbfk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ydzc1.top/gtytulsyxn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.kuanghao11.cn/gtndmkynao.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zdqjudy.top/gtdfhmiodm.html

[M04] 获取当前工作目录
来源：http://hz.cucudq.cn/gtbgjuiwtu.html

Py:   os.getcwd()
来源：http://hz.zhongyouzk.top/gthqwvpuzs.html

PHP:  getcwd();
来源：http://hz.cheryme.top/gtkfxaosdy.html

JS:   process.cwd()
来源：http://hz.haohaochexian.top/gtwdfhgcwy.html

TS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtupqzzrqn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenjidiqi.icu/gthrfjvdhu.html

Go:   os.Getwd()
来源：http://hz.zdqjudy.top/gtxrzomulb.html

Ruby: Dir.pwd
来源：http://hz.dianchejie.cn/gtqoebjobi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhongyouzk.top/gtjciedofi.html

[M05] 设置退出码
来源：http://hz.svipenyu.cn/gtepbqlgya.html

Py:   sys.exit(1)
来源：http://hz.tianlin.xyz/gtchznjvpz.html

PHP:  exit(1);
来源：http://hz.bjfxy.top/gtravyfbha.html

JS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtweftklft.html

TS:   process.exit(1)
来源：http://hz.yj202588.top/gtkfdzklfj.html

Java: System.exit(1)
来源：http://hz.hysaishi.cn/gttokqmlsl.html

Go:   os.Exit(1)
来源：http://hz.ppjwa.cn/gtmgoasqbw.html

Ruby: exit 1
来源：http://hz.wangshuangyany.cn/gtcxaaxxfn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nwbrower.top/gtirnpawza.html

[M06] 向标准错误输出
来源：http://hz.andypj.xyz/gtlaxazzdz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.fzhhl.top/gtatobskkt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fengsongda.top/gtqflnpjsy.html

JS:   console.error("err")
来源：http://hz.jqgfzy.top/gttvtvqxrb.html

TS:   console.error("err")
来源：http://hz.yj202588.top/gtryssrczw.html

Java: System.err.println("err")
来源：http://hz.shangyingyoupin.top/gtriaxbhig.html


<!-- 参考信息 -->