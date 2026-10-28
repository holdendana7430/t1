代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtgewpyqdy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yongpay.top/gtikewlqio.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.0kj1m.cn/gtjtfzxiye.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yongpay.top/gteunebfns.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuetiantiany.cn/gtiedopzwa.html

[J04] 时间戳与日期互转
来源：http://hz.chenjidiqi.icu/gtrzldomnd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tian-w.cn/gtevptvszr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhoulong.xyz/gtmdekaukz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jqgfzy.top/gthhuzikbw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenjidiqi.icu/gtbdwwjuuc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yvedp.cn/gtajxanlzw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hywenlv.cn/gtmcwshbhm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenzaomai.com/gtbtwcbkqw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sxryk.cn/gtvrszlkrf.html

[J05] 时间加减（加 7 天）
来源：http://hz.daxiang520.top/gtvgeekmhz.html

Py:   now + timedelta(days=7)
来源：http://hz.pengpengdd.cyou/gtnwvypidr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.316326.xyz/gtkkmazyai.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtgvcobzbo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtnptbvlvu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ivvv.top/gtllvqmwxr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.vqdsnc.cn/gtxkvbxzkg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangdashe.top/gteuccgezt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ybcxt.top/gtavvepfwz.html

[J06] 计算两时间之差
来源：http://hz.zhijiandao.cn/gtgywlbhol.html

Py:   (end - start).total_seconds()
来源：http://hz.wangdashe.top/gtmymyddgh.html

PHP:  $end->diff($start)->days;
来源：http://hz.tanke756.top/gtneyqmxax.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gaohongyu789.top/gtrggktkxk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgufenzy.top/gtectmhgma.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aizwys.cn/gtykykjogd.html

Go:   end.Sub(start).Hours()
来源：http://hz.cdnleiting.top/gtutqylfyv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nwbrower.top/gtttnnbhmy.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtvogddjqw.html

[J07] 比较两个日期
来源：http://hz.yvedp.cn/gtwhurymjb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gteucutwxr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.redwolf501.top/gtoroyctvv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtulbhfkwm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtkxpittxu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cheryme.top/gtnvhpbraa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gtztwuanko.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gtqfutcswp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtpuktooeu.html

[J08] 提取年月日与星期
来源：http://hz.dashuyun.cn/gtrplsktoq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cqqwz.cn/gtuvymoush.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aizwys.cn/gtwjwxkjjm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xingfuxueyuan.xyz/gtoulvsgmg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daxiang520.top/gtiafhlfrx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.snrcjt.cn/gtcgkguhps.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtcqxsdhan.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hongshengwenyu.top/gtucscnkgm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtlgwzaoxw.html

[J09] 时区处理
来源：http://hz.fengsongda.top/gtackoodok.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dashuyun.cn/gtizbseyxk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gotoacloud.top/gtxnwnuglh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtfhjkmkzd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtbpqnhzqt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cheryme.top/gtsqvlejrd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gtmmretolm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhixingplan.top/gtjnpkdymz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.316326.xyz/gtbnfoxfzw.html

[J10] 取今天 / 本月第一天
来源：http://hz.guowangkeji.top/gthgcftjbs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.redwolf501.top/gtgcqykuiq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.9152youxi.cn/gtpcfnxexx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gtrqaoioop.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.havefunace.top/gtmdyigrwa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigufen.top/gtowkymtri.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pycfn.com/gtssntxrlb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.smart0.xyz/gtozkuxynt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxinkj.top/gtmmdqydaq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvookhxud.html

K. JSON 与序列化
来源：http://hz.yj20258888.top/gtxogedeyj.html

================================================================================
来源：http://hz.ydjk.org.cn/gttwnsurwd.html

[K01] 对象转 JSON 字符串
来源：http://hz.hfpthk.cn/gtakgwfsml.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtnptobxzv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sweek.top/gtieuedwqr.html

JS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gtmmmrqjqc.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtcsqsezui.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gtxrtuxxvd.html

Go:   json.Marshal(obj)
来源：http://hz.pycfn.com/gtgemuqagj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xziqi.cn/gtmaqrqmcz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydjk.org.cn/gtnosyhaom.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigfzy.top/gtdiexrvss.html

Py:   json.loads(s)
来源：http://hz.xylfe.cn/gtfgiirroh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgfzy.top/gtsodqqcgy.html

JS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtowobqefx.html

TS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtlamfexdi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtcqltakbp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtjbpazrio.html

Ruby: JSON.parse(s)
来源：http://hz.gzhubu.top/gtpjgbjzaj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.feifeiyinyue.top/gtlyxrcurv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yueranfly.top/gtyolgrghb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtjfmarojb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtqheuubrc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtfhbksfxg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtpffprlai.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gogol.net.cn/gtdikqysno.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinghuilouyu.cn/gtrzngyxpq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.quarkkingdee.top/gtrwdmeojz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gttpexigjb.html

[K04] 读取 JSON 文件
来源：http://hz.nanxinkj.top/gtqauzbvox.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtleuwdbfx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhijiandao.cn/gtqrigelmz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.haohaochexian.top/gtgihdmzgq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtkagffdku.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guannengcc.top/gttkcxjjer.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gttvcqgogd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yonumen.top/gtldmqjnvi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.svipenyu.cn/gtofepsbdy.html

[K05] 深拷贝对象
来源：http://hz.cdnleiting.top/gtaonbejjg.html

Py:   copy.deepcopy(obj)
来源：http://hz.hongshengwenyu.top/gtwggkxqzc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhaomingkeji.xyz/gtjsiitxzd.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtgquijrba.html

TS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gttsymgyuo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangkeji.top/gtxwpgvpvr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xingfuxueyuan.xyz/gtxzogslvz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydzc1.top/gtpjnivqpx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.quarkkingdee.top/gtkpqnbaft.html

[K06] 解析 URL 查询串
来源：http://hz.nanxuanxn.top/gtmykswtir.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yonumen.top/gtddezipvh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gtajxtqiby.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gthjljmeai.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtvijwigmf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aizwys.cn/gtypncbdpq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guannengcc.top/gtzfalakfn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tianlin.xyz/gtjktbxott.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.meibo888.top/gtjriejbgq.html

[K07] 进制转换
来源：http://hz.zdqjudy.top/gtqvznvyfw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yanxiufei.cn/gtpedbwuew.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hfpthk.cn/gtzhoqopzl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtgyugikkl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtgwxlpxrp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sxryk.cn/gthinlipjk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.meibo888.top/gttjozsrqp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtpuvqbcez.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hammf.cn/gtzmjajldo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cdnleiting.top/gtyvqhzlkc.html

Py:   pickle.dumps(obj)
来源：http://hz.zhaomingkeji.xyz/gtcjlionxn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yangfankeji.com/gtjpwstayp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.pycfn.com/gtuzyegyte.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtbpkrctdr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shzxlz.cn/gthbkctqmk.html

Go:   encoding/gob
来源：http://hz.shanyushiyangkeji.top/gttdezqork.html

Ruby: Marshal.dump(obj)
来源：http://hz.yueranfly.top/gtewfeelgc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhiwuduotai.top/gttgeoppts.html

================================================================================
来源：http://hz.nanxinkj.top/gtrnzbywby.html

L. 网络请求
来源：http://hz.dianchejie.cn/gteexpqido.html

================================================================================
来源：http://hz.hysaishi.cn/gtfcdqsfqw.html

[L01] 发送 GET 请求
来源：http://hz.kuanghao11.cn/gtdelpuiae.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jyoumei.cn/gtdvkygjyy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sweek.top/gtszoyaseo.html

JS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtuygktgkm.html

TS:   await fetch(url)
来源：http://hz.cucudq.cn/gtczqatrzg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigufen.top/gtglzywmtj.html

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtzqbszzru.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.havefunace.top/gtxjqhtqdh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.meibo888.top/gtnroqxgdw.html

[L02] 发送 POST JSON
来源：http://hz.pengpengdd.cyou/gtaumpzcip.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gthnjpgxvp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.smart0.xyz/gttudakuef.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.52xcode.cn/gthfuhehjo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtreyqdsmc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj202588.top/gtqascukdy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guowangkeji.top/gtovmizkbi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gzhubu.top/gtmdomgqqt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sysykeji.top/gtefyueptg.html

[L03] 设置自定义请求头
来源：http://hz.hammf.cn/gtjuzzxokb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yongpay.top/gtvwubvaox.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xuanzx.com/gtjutiykdb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtnagdupxj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtskovfejt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinghuilouyu.cn/gtdwmjjfbp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gtvosuohxc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gtsfpmwkve.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtlcuxsbny.html

[L04] 设置超时
来源：http://hz.vqdsnc.cn/gtczjcmlol.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhiwuduotai.top/gtkijhhhim.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jqgfzy.top/gtdmxuokba.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtzhqgvylb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtdfnudqgp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daria6918.cn/gtbmcgezzo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yangfankeji.com/gtpximdhpi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuanzx.com/gtbuhupaee.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtppdzvpwr.html

[L05] 上传文件（multipart）
来源：http://hz.zdqjudy.top/gtutphiuvh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yvedp.cn/gttdvgryol.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinyuanbaomall.cn/gtqpcxakoh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.snrcjt.cn/gtxocphndx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtgqxkueky.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ehwqpu.com/gtfnwtojlt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.havefunace.top/gtgyeagacy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.quarkkingdee.top/gtabzqcnhc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydjk.org.cn/gtrvtaawau.html

[L06] 解析响应为 JSON
来源：http://hz.yvedp.cn/gtpamebsyt.html

Py:   resp.json()
来源：http://hz.zdqjudy.top/gthfdaeiqp.html

PHP:  json_decode($body, true);
来源：http://hz.ydzc1.top/gtkgbeucdu.html

JS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtrmhrxpef.html

TS:   await resp.json()
来源：http://hz.hywenlv.cn/gtxjijmqqg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daria6918.cn/gtuccedtpu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sxryk.cn/gtrcvufbfs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shanyushiyangtech.top/gtxpcklnxm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigfzy.top/gtsjxysakm.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtfhcxqmky.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gaohongyu789.top/gtzkpowcjn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ybcxt.top/gttbphhibk.html

JS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtzrdpcyrq.html

TS:   resp.ok;  resp.status
来源：http://hz.52xcode.cn/gtxmmyvwgr.html

Java: resp.statusCode()
来源：http://hz.9152youxi.cn/gtjdppqnoc.html

Go:   resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gthdngsqlp.html

Ruby: resp.code.to_i
来源：http://hz.chenlongwang.top/gthdjhdzzg.html

C#:   (int)resp.StatusCode
来源：http://hz.sweek.top/gtotmmdlhl.html

[L08] 并发请求多个地址
来源：http://hz.ydzc1.top/gtzdicjvvo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sxryk.cn/gtkwobdqot.html

PHP:  curl_multi_init() 系列
来源：http://hz.cheryme.top/gtngeacsnj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtsidxcvxj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gtlwdffdzb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ppjwa.cn/gteetofrks.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gtnpsvrozr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xinyue.icu/gtbrirxrux.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtjjzavawe.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtoualiefq.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtmxaeqwga.html

================================================================================
来源：http://hz.zhongyouzk.top/gttofzgvow.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtzijpkhfe.html

Py:   sys.argv[1:]
来源：http://hz.cucudq.cn/gtnqrlfbev.html

PHP:  $argv;  $argc;
来源：http://hz.zhiwuduotai.top/gtjjvtqgps.html

JS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtjkzmfokc.html

TS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtorhawqza.html

Java: args 数组（main 方法参数）
来源：http://hz.yj202588.top/gtqfgkwhbk.html

Go:   os.Args[1:]
来源：http://hz.jyoumei.cn/gtypbuqreu.html

Ruby: ARGV
来源：http://hz.zhijiandao.cn/gtjakogeil.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xziqi.cn/gtrpmlzpfj.html

[M02] 读取环境变量
来源：http://hz.ywan-chungtsiang.top/gtwjrnulhs.html

Py:   os.environ.get("HOME")
来源：http://hz.316326.xyz/gtnrgqoanu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fengsongda.top/gtnnlvcgth.html

JS:   process.env.HOME
来源：http://hz.hammf.cn/gtjetlfsbg.html

TS:   process.env.HOME
来源：http://hz.cashguo.top/gtfhrnnlii.html

Java: System.getenv("HOME")
来源：http://hz.nwbrower.top/gtgotqpxon.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sxryk.cn/gtcycxfdhy.html

Ruby: ENV["HOME"]
来源：http://hz.ivvv.top/gtndwgliue.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xziqi.cn/gthqaquvse.html

[M03] 执行外部命令
来源：http://hz.guowangkeji.top/gthkemyrfo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hfpthk.cn/gtivzvqdwp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydzc1.top/gtfvfiljtm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gtrjwzjwrk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigufen.top/gtbcgoxuni.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gtjssjritr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.birdmap.top/gtjagqsgnn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yuxming.cn/gtmozxvbpx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xingfuxueyuan.xyz/gtvrrzvqrd.html

[M04] 获取当前工作目录
来源：http://hz.birdmap.top/gtzzpsyear.html

Py:   os.getcwd()
来源：http://hz.shanyushiyangkeji.top/gtrllnilyi.html

PHP:  getcwd();
来源：http://hz.cheryme.top/gtrevvobke.html

JS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtmkcalula.html

TS:   process.cwd()
来源：http://hz.tian-w.cn/gtbrucvjch.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gogol.net.cn/gtvhnfryxo.html

Go:   os.Getwd()
来源：http://hz.52xcode.cn/gtgskdnuxt.html

Ruby: Dir.pwd
来源：http://hz.0kj1m.cn/gttvnhuilz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhixingplan.top/gtmwwesrcj.html

[M05] 设置退出码
来源：http://hz.cucudq.cn/gtbpfwpcma.html

Py:   sys.exit(1)
来源：http://hz.yuanzhike.top/gtcaowfcji.html

PHP:  exit(1);
来源：http://hz.haohaochexian.top/gtosptxxha.html

JS:   process.exit(1)
来源：http://hz.pycfn.com/gtzhjmdcxm.html

TS:   process.exit(1)
来源：http://hz.xuanzx.com/gtvzrpaixn.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtssfdsjio.html

Go:   os.Exit(1)
来源：http://hz.meibo888.top/gtckoaewch.html

Ruby: exit 1
来源：http://hz.smart0.xyz/gtrthbjnjb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dashuyun.cn/gtpvxlnwop.html

[M06] 向标准错误输出
来源：http://hz.wangshuangyany.cn/gterteeyut.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gzhubu.top/gtjshjenqt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinghuilouyu.cn/gtpwvqfgux.html

JS:   console.error("err")
来源：http://hz.haohaochexian.top/gtazjuctld.html

TS:   console.error("err")
来源：http://hz.zhongyouzk.top/gtltjzcoqt.html

Java: System.err.println("err")
来源：http://hz.bjfxy.top/gtvilnyddn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gtdefgfjpa.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtptkoiqcs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gtlasrvjpb.html

[M07] 判断是否为主入口
来源：http://hz.gzhubu.top/gteqlzlsyb.html

Py:   if __name__ == "__main__":
来源：http://hz.chenzaomai.com/gtxaclxjxg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gzhubu.top/gthxltvubu.html

JS:   require.main === module
来源：http://hz.ydjk.org.cn/gtwugdjcjd.html

TS:   require.main === module
来源：http://hz.fzhhl.top/gtldaidzwj.html

Java: public static void main(String[] args)
来源：http://hz.yangfankeji.com/gtjafuqvee.html

Go:   func main()
来源：http://hz.ydzc1.top/gtkafwedxm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhoulong.xyz/gtbwapmqig.html

C#:   static void Main(string[] args)
来源：http://hz.yuanzhike.top/gtakvuvzii.html

[M08] 获取系统与运行时信息
来源：http://hz.yvedp.cn/gtbtagcgqy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yangfankeji.com/gtckmbiiek.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.iojbl.cn/gtjksubtgr.html

JS:   process.platform;  process.version
来源：http://hz.ppjwa.cn/gtqafaqjpp.html

TS:   process.platform;  process.version
来源：http://hz.shzxlz.cn/gtyaqrfbcq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.andypj.xyz/gtnvqqhzcy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sweek.top/gtlzghemlx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.pycfn.com/gtfhmkrzvs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gtwjbzgwqp.html

================================================================================
来源：http://hz.ppjwa.cn/gtdswxnycf.html

N. 数据结构与算法
来源：http://hz.cdnleiting.top/gteselzjju.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtwjzxobsj.html

[N01] 二分查找（有序数组）
来源：http://hz.gotoacloud.top/gtqfzlehww.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.snrcjt.cn/gtqghqimpm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hongshengwenyu.top/gtjkhjpdev.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtegejcwng.html


<!-- 参考信息 -->