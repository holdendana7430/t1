代发 wailian999

Go:   time.Now()
来源：http://hz.ppjwa.cn/gtmfdheoxc.html

Ruby: Time.now
来源：http://hz.jlsjyb.cn/gtyexyuixz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.smart0.xyz/gtikeiinaw.html

[J02] 格式化输出
来源：http://hz.gotoacloud.top/gtwoepzaqt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtlbkqqaqs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtjprggmum.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xziqi.cn/gtqtwwdzxi.html

TS:   d.toISOString()
来源：http://hz.yj20258888.top/gtmnxtjjxl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenlongwang.top/gtkfbrcpnw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.mhx1999.top/gtgharqcto.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtldrlalos.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj202588.top/gtrcfsjogf.html

[J03] 字符串解析为日期
来源：http://hz.kuanghao11.cn/gtjbdcndac.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuanzx.com/gtzsdqfooy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.wangdashe.top/gtulujrncy.html

JS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtbdbolfqf.html

TS:   new Date("2024-01-02")
来源：http://hz.jqgfzy.top/gtjfdhkuhm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtvyzbajzo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hongshengwenyu.top/gtghjsgzcl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtpamlzppc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gzhubu.top/gtvdvcbvus.html

[J04] 时间戳与日期互转
来源：http://hz.kuanghao11.cn/gtntrxusil.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sysykeji.top/gtelcaiblq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daria6918.cn/gtkmohpbid.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sxryk.cn/gtssusqmfg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gttxxxpumm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xziqi.cn/gtzopwyfla.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.316326.xyz/gtdnxaylgc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hysaishi.cn/gtdadcurud.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.svipenyu.cn/gtwbgiaata.html

[J05] 时间加减（加 7 天）
来源：http://hz.smart0.xyz/gtnmmevvrn.html

Py:   now + timedelta(days=7)
来源：http://hz.yuxming.cn/gtkbjptfqr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhoulong.xyz/gtwdyxcgfj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtaxqxcnea.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtyponxnug.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xinyue.icu/gtknfcxyvv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydjk.org.cn/gttlgbckty.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yueranfly.top/gtyfxfssyp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.9152youxi.cn/gteuhrfzuv.html

[J06] 计算两时间之差
来源：http://hz.pycfn.com/gthzwnqryv.html

Py:   (end - start).total_seconds()
来源：http://hz.meibo888.top/gtpnnviqii.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuetiantiany.cn/gtnzlugtrv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yuanzhike.top/gtjupjsxsc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shzxlz.cn/gtadfsmsju.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dashuyun.cn/gtqsixxkeq.html

Go:   end.Sub(start).Hours()
来源：http://hz.xylfe.cn/gtjyyeorig.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gtvieljrgw.html

C#:   (end - start).TotalSeconds
来源：http://hz.dashuyun.cn/gtowyjiepq.html

[J07] 比较两个日期
来源：http://hz.hywenlv.cn/gtxlwdxdwp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtcrdxlznd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtsdzrkpcb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.redwolf501.top/gtmuacakgi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtaivcxuiz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.0kj1m.cn/gtwrjqzyaa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhaomingkeji.xyz/gtrfacojzh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtekftbgig.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtmxvqkfgk.html

[J08] 提取年月日与星期
来源：http://hz.aizwys.cn/gtpjkcmxgr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gtahnvvrtq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guannengcc.top/gtauofuxfo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.feifeiyinyue.top/gttyrjjnrd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hfpthk.cn/gtcgdxmzvp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.feifeiyinyue.top/gtefvcawkp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.redwolf501.top/gtsjhvaagu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.wangdashe.top/gtdyvevecn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gtoruwyyri.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtbmtoxigh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgufenzy.top/gtetcxhwcv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhaomingkeji.xyz/gtiywiymbn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtiuxrqbtt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aizwys.cn/gtgqwnfpbo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dianchejie.cn/gttnygldym.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pycfn.com/gtawmdtzau.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhengqikj.top/gtosezuyej.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ivvv.top/gtvchwqrvn.html

[J10] 取今天 / 本月第一天
来源：http://hz.pengpengdd.cyou/gtbdfmnjkn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenjidiqi.icu/gtjriboqty.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.bjfxy.top/gtrmjgxmkz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangtech.top/gtytnqbdrx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hongshengwenyu.top/gthzratdza.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.dashuyun.cn/gtqcjxparb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.kuanghao11.cn/gtfrkokamg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ivvv.top/gtmnswavtk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gaohongyu789.top/gteklygwkx.html

================================================================================
来源：http://hz.jlsjyb.cn/gtwchipbyl.html

K. JSON 与序列化
来源：http://hz.yj20258.top/gttahzdvrm.html

================================================================================
来源：http://hz.zycfv.cn/gtyxhcamvh.html

[K01] 对象转 JSON 字符串
来源：http://hz.meibo888.top/gtikpirqws.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtyqsyvbld.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtthuwyiju.html

JS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtshzezkor.html

TS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gteqmzwrkd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.0kj1m.cn/gtpewhehkc.html

Go:   json.Marshal(obj)
来源：http://hz.kuanghao11.cn/gtqocvdabk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258.top/gtrxijgmbl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yvedp.cn/gtegszzqhh.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtjnrsjcoc.html

Py:   json.loads(s)
来源：http://hz.tian-w.cn/gtsanyfdal.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hammf.cn/gtjogwzgqb.html

JS:   JSON.parse(s)
来源：http://hz.iojbl.cn/gtsxnssyse.html

TS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtttnegpaz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cashguo.top/gtbfwhgqtn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtnbyngdby.html

Ruby: JSON.parse(s)
来源：http://hz.gogol.net.cn/gtmgtboghy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.meibo888.top/gtlozfbnjy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nwbrower.top/gteaswyzxt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtycbwxcdt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhijiandao.cn/gtxztfovkf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtjeizexha.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtnmncdegq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zycfv.cn/gtjtrsqjcc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgfzy.top/gttgfpmlbu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yanxiufei.cn/gthlukajpz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.quarkkingdee.top/gtssccybog.html

[K04] 读取 JSON 文件
来源：http://hz.cheryme.top/gtkuoolbwl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jiagoushi.top/gtjjuutfrg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shangyingyoupin.top/gtarhlsanc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtqbujrioe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtwbdaynqo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.bjfxy.top/gtxuqyrbge.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ydjk.org.cn/gtzynskpve.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ivvv.top/gtvdkpvuri.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangtech.top/gtvugelrzy.html

[K05] 深拷贝对象
来源：http://hz.shuidangran.top/gtjcdwksna.html

Py:   copy.deepcopy(obj)
来源：http://hz.meibo888.top/gtrihswfqe.html

PHP:  unserialize(serialize($obj));
来源：http://hz.wangdashe.top/gtrpgohuvp.html

JS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtmwyckhvk.html

TS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gthusgorbe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guannengcc.top/gtbinsbmqu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cucudq.cn/gtcsgeeerb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hnxiangtu.top/gtjyiawuoc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinghuilouyu.cn/gtjonxmvci.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gttazpcuvv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hywenlv.cn/gtguzjncid.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zycfv.cn/gtaswyjryx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtuszqhgas.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtspacxzqw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sweek.top/gtuhzwyiih.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xinyue.icu/gtktlsclfz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.svipenyu.cn/gtgyhqqqjq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zycfv.cn/gtgfhcdwjz.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtyyxcnjon.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aibaodan.cn/gtmiabqxnn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dianchejie.cn/gtanoizkxs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtnjqhfjva.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtsvtmrdeo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtruuaiwcz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigfzy.top/gtnfmnhsqc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenzaomai.com/gtspnzvwsk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pycfn.com/gtcjeshxkq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shzxlz.cn/gtrpstjcmd.html

Py:   pickle.dumps(obj)
来源：http://hz.chenlongwang.top/gtiaiswfje.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenjidiqi.icu/gtzafyddxn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtkjkkrdwm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtcrzjnryo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yonumen.top/gthazjuuas.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gtxxpkvbwy.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258888.top/gtmmtlxtkn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zycfv.cn/gtotgjfzvl.html

================================================================================
来源：http://hz.quarkkingdee.top/gtjzhxmkgh.html

L. 网络请求
来源：http://hz.yuxming.cn/gtwzusxaml.html

================================================================================
来源：http://hz.aizwys.cn/gtmdsfopgh.html

[L01] 发送 GET 请求
来源：http://hz.ydjk.org.cn/gtvklhlfck.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tianlin.xyz/gtigvhdnpi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgfzy.top/gtnejlfjxc.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtfjexyipb.html

TS:   await fetch(url)
来源：http://hz.xziqi.cn/gtgsehndge.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigfzy.top/gtvpajqdac.html

Go:   resp, err := http.Get(url)
来源：http://hz.xziqi.cn/gtxknvsffy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.birdmap.top/gtwgpzutww.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xinyue.icu/gtirnbbvwr.html

[L02] 发送 POST JSON
来源：http://hz.hongshengwenyu.top/gtlaizimuh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gttabvvipc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.9152youxi.cn/gtzazhhfmb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtgmgainzy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtowusqfpi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtgystmpyx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.kuanghao11.cn/gtvsdmndtd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yonumen.top/gtyrdottpb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.bjfxy.top/gtuajkqtqa.html

[L03] 设置自定义请求头
来源：http://hz.havefunace.top/gtqhwocpic.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zycfv.cn/gtlrnfunsd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xingfuxueyuan.xyz/gtlkoczibf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gthrqmqgax.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtrlddynvx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cqqwz.cn/gtqdkkjvsc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtowlewxgh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.svipenyu.cn/gthhfbfgkj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtttfjyxkk.html

[L04] 设置超时
来源：http://hz.shangyingyoupin.top/gtkmhxhita.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xingfuxueyuan.xyz/gtifjyhqbm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fzhhl.top/gtegffbjtg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gtzvhviyko.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gtcmnlqzxr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.0kj1m.cn/gtccevdsmh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.dianchejie.cn/gtahwtqiyg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuetiantiany.cn/gtyxkazwfr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tian-w.cn/gthhwyclgj.html

[L05] 上传文件（multipart）
来源：http://hz.dianchejie.cn/gtpfuwpdgp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangkeji.top/gtbzqihrav.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hfpthk.cn/gttaqjvqdz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtjacwfjip.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtoikgxzlt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hysaishi.cn/gtgieikicg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gzhubu.top/gtlorwueef.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.c1oappe.top/gtqqgkrazn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhijiandao.cn/gtihnyrllx.html

[L06] 解析响应为 JSON
来源：http://hz.haohaochexian.top/gtbdycqmjh.html

Py:   resp.json()
来源：http://hz.xziqi.cn/gtbqaryedl.html

PHP:  json_decode($body, true);
来源：http://hz.havefunace.top/gtqykhjgou.html

JS:   await resp.json()
来源：http://hz.zycfv.cn/gtzhlftgit.html

TS:   await resp.json()
来源：http://hz.wangdashe.top/gtbfbvuqyq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guannengcc.top/gtlcsumawr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xuetiantiany.cn/gttbxobnrp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xingfuxueyuan.xyz/gtbffpualv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fzhhl.top/gtzvttclmi.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhongyouzk.top/gteksgzznl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.guowangkeji.top/gtgjalttcm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangdashe.top/gttfyomxia.html

JS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtizflraow.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtatbrxxxd.html

Java: resp.statusCode()
来源：http://hz.jqgufenzy.top/gtvvgybyjq.html

Go:   resp.StatusCode
来源：http://hz.sysykeji.top/gtnczqfxac.html

Ruby: resp.code.to_i
来源：http://hz.andypj.xyz/gtplhovasj.html

C#:   (int)resp.StatusCode
来源：http://hz.316326.xyz/gtodfkldde.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangtech.top/gticvbrofj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgfzy.top/gtqhvuljzo.html

PHP:  curl_multi_init() 系列
来源：http://hz.xingfuxueyuan.xyz/gtdntsvjsg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtuxwmpddx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtoxwecgyk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinyuanbaomall.cn/gtqutkarqh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhoulong.xyz/gtcnyyvldo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hysaishi.cn/gtlumkttba.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtmmbiqwgy.html

================================================================================
来源：http://hz.zhoulong.xyz/gtptrvwnlr.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gtstugfeej.html

================================================================================
来源：http://hz.xuanzx.com/gtmxyndnnz.html

[M01] 读取命令行参数
来源：http://hz.52xcode.cn/gtwrpezylm.html

Py:   sys.argv[1:]
来源：http://hz.chenzaomai.com/gtqijevxsr.html

PHP:  $argv;  $argc;
来源：http://hz.vqdsnc.cn/gtbjtpuyip.html

JS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gthljmypwb.html

TS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtzhxhzier.html

Java: args 数组（main 方法参数）
来源：http://hz.dianchejie.cn/gtatzrbxkk.html

Go:   os.Args[1:]
来源：http://hz.redwolf501.top/gtemwsjodi.html

Ruby: ARGV
来源：http://hz.9152youxi.cn/gtrdaeaddp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtqdvwaewl.html

[M02] 读取环境变量
来源：http://hz.ywan-chungtsiang.top/gtcihlbhpr.html

Py:   os.environ.get("HOME")
来源：http://hz.gaohongyu789.top/gtetmbttpx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenjidiqi.icu/gtkrvognjq.html

JS:   process.env.HOME
来源：http://hz.yongpay.top/gtuckmfsho.html

TS:   process.env.HOME
来源：http://hz.sxryk.cn/gtyjipiqyl.html

Java: System.getenv("HOME")
来源：http://hz.redwolf501.top/gteloqqzai.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtivsigsoj.html

Ruby: ENV["HOME"]
来源：http://hz.nwbrower.top/gtspbcurlx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.redwolf501.top/gtqvuyuhdj.html

[M03] 执行外部命令
来源：http://hz.iojbl.cn/gtwpdzomex.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtzqpszaim.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.0kj1m.cn/gtappnydsn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gtpcnmxguj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gtawngvbon.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenlongwang.top/gtdaexqimz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.smart0.xyz/gtytshnfil.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sxryk.cn/gtxdzfvqod.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jiagoushi.top/gtmrmbccqi.html

[M04] 获取当前工作目录
来源：http://hz.wangdashe.top/gtqinrlqvm.html

Py:   os.getcwd()
来源：http://hz.ivvv.top/gtatvlgypk.html

PHP:  getcwd();
来源：http://hz.yj20258.top/gtzoohhlvn.html

JS:   process.cwd()
来源：http://hz.shzxlz.cn/gtwidssuik.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gtncxcxfyc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dashuyun.cn/gtsdysyevk.html

Go:   os.Getwd()
来源：http://hz.bjfxy.top/gtjbbxeddz.html

Ruby: Dir.pwd
来源：http://hz.chenlongwang.top/gtydvqkkgz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgfzy.top/gtmldydudg.html

[M05] 设置退出码
来源：http://hz.ydzc1.top/gtrkwsarbp.html

Py:   sys.exit(1)
来源：http://hz.wangdashe.top/gtboogjeqq.html

PHP:  exit(1);
来源：http://hz.fengsongda.top/gtyeyfzkfi.html

JS:   process.exit(1)
来源：http://hz.aizwys.cn/gtedzwutkb.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtybdbktqi.html

Java: System.exit(1)
来源：http://hz.316326.xyz/gtqvtrpjte.html

Go:   os.Exit(1)
来源：http://hz.xuetiantiany.cn/gtgrkypbdz.html

Ruby: exit 1
来源：http://hz.hnqzz.top/gtdsyplvek.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yueranfly.top/gtdprburxo.html

[M06] 向标准错误输出
来源：http://hz.pengpengdd.cyou/gtmabgjnkh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gtnnwdginm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtpaqyqoxl.html

JS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtbxdhadxr.html

TS:   console.error("err")
来源：http://hz.jianghu66.top/gthuptmria.html

Java: System.err.println("err")
来源：http://hz.hongshengwenyu.top/gtmakqssvq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhijiandao.cn/gthnakokys.html

Ruby: warn "err"
来源：http://hz.mhx1999.top/gthufuvbkm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtzpprqrmk.html

[M07] 判断是否为主入口
来源：http://hz.shangyingyoupin.top/gtdficbfdo.html

Py:   if __name__ == "__main__":
来源：http://hz.daxiang520.top/gtamyerypp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.mhx1999.top/gtaoybildk.html

JS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtxiszxlbe.html

TS:   require.main === module
来源：http://hz.fzhhl.top/gtcvlsymwb.html

Java: public static void main(String[] args)
来源：http://hz.hfpthk.cn/gtsscirfhd.html

Go:   func main()
来源：http://hz.redwolf501.top/gtikrtkeab.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xylfe.cn/gtzrcsplwn.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258.top/gtipkbpjrt.html


<!-- 参考信息 -->