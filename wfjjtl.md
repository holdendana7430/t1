代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtxpltruzx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtbeawonky.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangdashe.top/gtrdbzntdk.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangtech.top/gtwjyokplh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258.top/gtkdyhoosz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gzhubu.top/gtaskmxgdf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gtcluqgdmb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xylfe.cn/gtvmrksdgg.html

[J03] 字符串解析为日期
来源：http://hz.tanke756.top/gtsxxketqo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhiwuduotai.top/gteiezfuja.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dianchejie.cn/gtgxwusfnf.html

JS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtttcbvxxb.html

TS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtyuzmkaap.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtnbabanlw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.quarkkingdee.top/gtiivkwwcp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gtdayyayrx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fengsongda.top/gtemjxbkxd.html

[J04] 时间戳与日期互转
来源：http://hz.shangyingyoupin.top/gtghfyffqt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtfzznzbmz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxuanxn.top/gtotbptlbv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.quarkkingdee.top/gtnevfcgny.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tanke756.top/gtoqcheetv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tanke756.top/gtdrnneudl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shzxlz.cn/gtwmdeugru.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigfzy.top/gtjnglxiqf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.316326.xyz/gtzctuahhr.html

[J05] 时间加减（加 7 天）
来源：http://hz.dianchejie.cn/gtzqumzhzn.html

Py:   now + timedelta(days=7)
来源：http://hz.zhiwuduotai.top/gttzcivybs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.andypj.xyz/gtorzedhbp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtvxwvhgsf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtyidslinx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aizwys.cn/gtxfudxroq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangkeji.top/gtcvvjmlvw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jlsjyb.cn/gtuzvmyjei.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtwewonprz.html

[J06] 计算两时间之差
来源：http://hz.smart0.xyz/gtndohclfb.html

Py:   (end - start).total_seconds()
来源：http://hz.fengsongda.top/gtweykwcbg.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinqigfzy.top/gtipmqdwpb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.haohaochexian.top/gthhbiljkf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.0kj1m.cn/gtdifnlyfo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.havefunace.top/gtrtnkwduw.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtylyaokfz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hammf.cn/gtweadunyq.html

C#:   (end - start).TotalSeconds
来源：http://hz.316326.xyz/gtahbtmoif.html

[J07] 比较两个日期
来源：http://hz.zhaomingkeji.xyz/gtwyswlveb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtotajwjxa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shzxlz.cn/gtnnwankcp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtkrozxppn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.vqdsnc.cn/gtdkncvazy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuanzx.com/gtvcwxhjux.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gtmrvesnfc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtkpyaobwo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtqcqaqxpj.html

[J08] 提取年月日与星期
来源：http://hz.fengsongda.top/gtxyiqtade.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangdashe.top/gtsokyorun.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinghuilouyu.cn/gtcgoxxeke.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fzhhl.top/gteagdaqxs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.quarkkingdee.top/gtwrthedll.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gzhubu.top/gtuxylknxg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gtkqnjvjpy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gthwujnqba.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nanxinkj.top/gttrwejdqf.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtblbdgxqn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gtthgoihqi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zdqjudy.top/gtsbzfrwwi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtgrnbgyof.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtakcirdaf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.smart0.xyz/gtnmeznuum.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ybcxt.top/gtpbatrajf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuetiantiany.cn/gthcemzohn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.feifeiyinyue.top/gtsacrntit.html

[J10] 取今天 / 本月第一天
来源：http://hz.yanxiufei.cn/gtblxookct.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigufen.top/gtbxpazmdo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhoulong.xyz/gtguiyhoae.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yvedp.cn/gtvqreiage.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtpplcnvvo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.vqdsnc.cn/gtzmnakfbo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.meibo888.top/gtsrzxbfml.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gaohongyu789.top/gtnvqjdbbx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.birdmap.top/gtikxwnstf.html

================================================================================
来源：http://hz.0kj1m.cn/gtwfaqrvhn.html

K. JSON 与序列化
来源：http://hz.zhixingplan.top/gtimahzbxf.html

================================================================================
来源：http://hz.cucudq.cn/gtjbfjllvj.html

[K01] 对象转 JSON 字符串
来源：http://hz.hywenlv.cn/gtexllxzng.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gtmbeyvlsv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtcsutyjwy.html

JS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtsygjkxhs.html

TS:   JSON.stringify(obj)
来源：http://hz.jlsjyb.cn/gturbgmtug.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jyoumei.cn/gtdeqxfpqh.html

Go:   json.Marshal(obj)
来源：http://hz.snrcjt.cn/gttzqprpyl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.316326.xyz/gtgwvatghw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuxming.cn/gtruwtrdez.html

[K02] JSON 字符串转对象
来源：http://hz.hysaishi.cn/gticlediqd.html

Py:   json.loads(s)
来源：http://hz.tianlin.xyz/gtrmfciepg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhiwuduotai.top/gtbcfrcueq.html

JS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtlornirua.html

TS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtqsveteek.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.guowangkeji.top/gtkyeinpeb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtwxbaxmdr.html

Ruby: JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtmkcponqo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sufxvd.cn/gtybxgkpce.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.0kj1m.cn/gtvfefrsfc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtkotrvhoi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtymwmoken.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gtrkihistm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gtskigvjpc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtnkpbcdpc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuanzx.com/gtghgkneam.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenzaomai.com/gtffrquajs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnqzz.top/gtdjurdxlq.html

[K04] 读取 JSON 文件
来源：http://hz.havefunace.top/gtabmamxqo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.316326.xyz/gtpokkmzkr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yongpay.top/gtzwxjigqr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtipeaflot.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtlejasrgz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.haohaochexian.top/gtvlplsujm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shzxlz.cn/gtcajrqyvm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xinyue.icu/gttbezqbgp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhaomingkeji.xyz/gturnjmauk.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtegfbdrow.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxinkj.top/gtqcanodmr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.dashuyun.cn/gtymoewmpk.html

JS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtorrbnrmm.html

TS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gthlvgimgx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenlongwang.top/gtcskcuwyx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pengpengdd.cyou/gtdncrlltm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xuetiantiany.cn/gtdykamaha.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258.top/gtsaqcsaei.html

[K06] 解析 URL 查询串
来源：http://hz.316326.xyz/gtmrgwhtiy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aizwys.cn/gtkvbimauj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xingfuxueyuan.xyz/gtgplxonzm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtoqkyxudn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtphdmhaez.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.birdmap.top/gtahzemeqe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yongpay.top/gtwdplxzxi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtvfoybadn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuxming.cn/gtukhbyyil.html

[K07] 进制转换
来源：http://hz.nanxuanxn.top/gtryxbixxv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgufenzy.top/gtrrsdrnpr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jianghu66.top/gtloeitzax.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtjdnnangb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtsynrkwlu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ybcxt.top/gttylwxijg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtnnqxzkyu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.iojbl.cn/gtkgxjwoxj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yangfankeji.com/gtwtxnbpgu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.0kj1m.cn/gttugjmroy.html

Py:   pickle.dumps(obj)
来源：http://hz.dashuyun.cn/gtgibxktfk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.haohaochexian.top/gtzswxmbvv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gttevlitwk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gtetzhrctw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yvedp.cn/gtsduzcwby.html

Go:   encoding/gob
来源：http://hz.xziqi.cn/gtccimhrqv.html

Ruby: Marshal.dump(obj)
来源：http://hz.xylfe.cn/gtutppmwel.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenlongwang.top/gtzvegckyx.html

================================================================================
来源：http://hz.guannengcc.top/gtusqyjkik.html

L. 网络请求
来源：http://hz.zhaomingkeji.xyz/gttdmpfhmp.html

================================================================================
来源：http://hz.zycfv.cn/gthelworca.html

[L01] 发送 GET 请求
来源：http://hz.cheryme.top/gtmqdczeyh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.dashuyun.cn/gtnlomyvik.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258888.top/gttwgcqzlc.html

JS:   await fetch(url)
来源：http://hz.tianlin.xyz/gttixplchj.html

TS:   await fetch(url)
来源：http://hz.yj20258888.top/gttihwrjru.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenlongwang.top/gteejatdvr.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhengqikj.top/gtozxastom.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnqzz.top/gtbxsytqof.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.c1oappe.top/gtpnvxmwvo.html

[L02] 发送 POST JSON
来源：http://hz.xylfe.cn/gtjbwfdrqc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yanxiufei.cn/gtibfgrpoq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhiwuduotai.top/gtcavibbeu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gttimiqmqs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gthkgkrzmv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hywenlv.cn/gtvhrpmeox.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dashuyun.cn/gtwgugyxbb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinqigfzy.top/gtdwxzbzvp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj202588.top/gtjpclfukc.html

[L03] 设置自定义请求头
来源：http://hz.hammf.cn/gtmoahnrdm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ivvv.top/gtafoqidjc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangkeji.top/gtlkwgyvfc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtqghtjbom.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gthvootrzk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aibaodan.cn/gtdndmeiwd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtcdpazqre.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yvedp.cn/gtemgzvzyd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtmytjxzcq.html

[L04] 设置超时
来源：http://hz.iojbl.cn/gtoultlvwt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sweek.top/gtqbvmzaji.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yonumen.top/gtzsqowrpa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtslfxyeai.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtrsbzidje.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.aibaodan.cn/gtpnjvcjml.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sufxvd.cn/gtglniiwet.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yvedp.cn/gthcpkcejn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj202588.top/gtchpovknk.html

[L05] 上传文件（multipart）
来源：http://hz.gzhubu.top/gtgvrwacjo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daria6918.cn/gtobkejyio.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhixingplan.top/gtsjxejrck.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtpnkqazzh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtezhrvrky.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhijiandao.cn/gtftwlxfvk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhongyouzk.top/gtuydswige.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gotoacloud.top/gtqpdvirni.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gaohongyu789.top/gtiaczjzxy.html

[L06] 解析响应为 JSON
来源：http://hz.yuxming.cn/gtbjtviuge.html

Py:   resp.json()
来源：http://hz.aibaodan.cn/gtcgqvugvx.html

PHP:  json_decode($body, true);
来源：http://hz.svipenyu.cn/gtsffoculz.html

JS:   await resp.json()
来源：http://hz.cdnleiting.top/gtumocrilo.html

TS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtlujekcvk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hysaishi.cn/gtixkikidy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.9152youxi.cn/gtxrlcfxzh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.52xcode.cn/gttnmcnkjg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhoulong.xyz/gtncsfdbur.html

[L07] 处理 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtuddlyhze.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fzhhl.top/gtrrjtgwvn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuxming.cn/gttghpjngu.html

JS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangkeji.top/gtzuuqtpaq.html

TS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtqkakzeqr.html

Java: resp.statusCode()
来源：http://hz.shangyingyoupin.top/gtrybjxwkx.html

Go:   resp.StatusCode
来源：http://hz.52xcode.cn/gtusgkbtxi.html

Ruby: resp.code.to_i
来源：http://hz.yvedp.cn/gtoaczzgcb.html

C#:   (int)resp.StatusCode
来源：http://hz.zhixingplan.top/gtmotekauo.html

[L08] 并发请求多个地址
来源：http://hz.0kj1m.cn/gtomltpejc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tian-w.cn/gtqbclnmcp.html

PHP:  curl_multi_init() 系列
来源：http://hz.xinyue.icu/gtpedzwmcn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtxrfzvwxd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtzivmtqhn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.birdmap.top/gtkaqspwjg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnqzz.top/gtoheflowv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuetiantiany.cn/gtlfoogbmm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.iojbl.cn/gtbxtdxfgl.html

================================================================================
来源：http://hz.smart0.xyz/gtjgkhvsqe.html

M. 命令行 / 进程 / 环境
来源：http://hz.ivvv.top/gtjhbetjki.html

================================================================================
来源：http://hz.cucudq.cn/gternhhyid.html

[M01] 读取命令行参数
来源：http://hz.fengsongda.top/gtntjcfvlq.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtqcdmdcid.html

PHP:  $argv;  $argc;
来源：http://hz.snrcjt.cn/gtluxezynp.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtimfgzrqb.html

TS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gtvifpzgkr.html

Java: args 数组（main 方法参数）
来源：http://hz.smart0.xyz/gtsoiijnmg.html

Go:   os.Args[1:]
来源：http://hz.yuxming.cn/gtxdllowpt.html

Ruby: ARGV
来源：http://hz.guannengcc.top/gtjckrmvnm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sufxvd.cn/gtzmnstdnn.html

[M02] 读取环境变量
来源：http://hz.meibo888.top/gtzzkiqblp.html

Py:   os.environ.get("HOME")
来源：http://hz.fengsongda.top/gtcmqghhzo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhijiandao.cn/gtyzgkjclk.html

JS:   process.env.HOME
来源：http://hz.zhengqikj.top/gthzfwzgxz.html

TS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtinhaknqk.html

Java: System.getenv("HOME")
来源：http://hz.dashuyun.cn/gtbmdxsses.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtfdowvaqn.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gtolzdzabw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gzhubu.top/gtsqssmebs.html

[M03] 执行外部命令
来源：http://hz.mhx1999.top/gtmcakcizh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xziqi.cn/gtgdpcukhr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.c1oappe.top/gtvmftorto.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ywan-chungtsiang.top/gtwyjkryah.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gtgfadrkua.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhengqikj.top/gtjynxznak.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xylfe.cn/gtozzpdfvk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.havefunace.top/gtlcjvpdua.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtuokypjgj.html

[M04] 获取当前工作目录
来源：http://hz.cucudq.cn/gtekefkrfl.html

Py:   os.getcwd()
来源：http://hz.hfpthk.cn/gtgimxbzoh.html

PHP:  getcwd();
来源：http://hz.sweek.top/gtqtjcstot.html

JS:   process.cwd()
来源：http://hz.aizwys.cn/gtoemlfshj.html

TS:   process.cwd()
来源：http://hz.shuidangran.top/gthuiyodsd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.redwolf501.top/gtloradfox.html

Go:   os.Getwd()
来源：http://hz.shzxlz.cn/gtcpijehwa.html

Ruby: Dir.pwd
来源：http://hz.xuanzx.com/gtexiifdwv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cucudq.cn/gtimmlexzq.html

[M05] 设置退出码
来源：http://hz.yonumen.top/gtnlsdufsh.html

Py:   sys.exit(1)
来源：http://hz.nanxuanxn.top/gtatcjzmug.html

PHP:  exit(1);
来源：http://hz.yongpay.top/gtdbkoiwzn.html

JS:   process.exit(1)
来源：http://hz.hysaishi.cn/gtwaahgylg.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtcsuolbpz.html

Java: System.exit(1)
来源：http://hz.chenzaomai.com/gtzmnchoku.html

Go:   os.Exit(1)
来源：http://hz.wangdashe.top/gtdfluxznx.html

Ruby: exit 1
来源：http://hz.jyoumei.cn/gttpamxuhm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhixingplan.top/gtlqxxdqvp.html

[M06] 向标准错误输出
来源：http://hz.guannengcc.top/gtsfjiaoax.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yangfankeji.com/gtkwafwntu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xziqi.cn/gtefxqrmvm.html

JS:   console.error("err")
来源：http://hz.hammf.cn/gtnnwvuogf.html

TS:   console.error("err")
来源：http://hz.52xcode.cn/gtcocdldgd.html

Java: System.err.println("err")
来源：http://hz.cdnleiting.top/gtcrlihczg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yonumen.top/gtrweohrla.html

Ruby: warn "err"
来源：http://hz.ywan-chungtsiang.top/gtoounrhgv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.meibo888.top/gtfcznrlmf.html

[M07] 判断是否为主入口
来源：http://hz.meibo888.top/gtgmkyjqor.html

Py:   if __name__ == "__main__":
来源：http://hz.jinyuanbaomall.cn/gtfyrdrqqa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gaohongyu789.top/gttayhfclj.html

JS:   require.main === module
来源：http://hz.hammf.cn/gtxhxvvcbv.html

TS:   require.main === module
来源：http://hz.snrcjt.cn/gtubflxmtc.html

Java: public static void main(String[] args)
来源：http://hz.dashuyun.cn/gtnjbgqhxp.html

Go:   func main()
来源：http://hz.kuanghao11.cn/gtmujgppdu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ivvv.top/gtiaqxzfab.html

C#:   static void Main(string[] args)
来源：http://hz.nwbrower.top/gtpcnbwoor.html

[M08] 获取系统与运行时信息
来源：http://hz.ivvv.top/gtvzyvtcgd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.fengsongda.top/gtllmzuejh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuetiantiany.cn/gtqabtqpod.html

JS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtwzuuvhqh.html


<!-- 参考信息 -->