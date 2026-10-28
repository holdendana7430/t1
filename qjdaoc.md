代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jyoumei.cn/gtcegcgvzf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnqzz.top/gtptnrpreu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtppsexqkr.html

================================================================================
来源：http://hz.smart0.xyz/gtaxystcjb.html

J. 日期与时间
来源：http://hz.jiagoushi.top/gtzcxqkycj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtubajrryp.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtjcxubzgd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aizwys.cn/gtwrbhdkxn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtbyvsfjnt.html

JS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtzlbpdxdp.html

TS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtgcdpfitn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shuidangran.top/gtegpfeown.html

Go:   time.Now()
来源：http://hz.jiagoushi.top/gtabzeaszx.html

Ruby: Time.now
来源：http://hz.dashuyun.cn/gtrvxxghxc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.daxiang520.top/gtuejyfzcc.html

[J02] 格式化输出
来源：http://hz.bjfxy.top/gtixjpunab.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtawfetsms.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gtfycwfdlg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.kuanghao11.cn/gtfpdxtxgw.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtkflxewix.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangkeji.top/gturtxsjsi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yonumen.top/gtugxenoan.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigufen.top/gttcuymmph.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jianghu66.top/gtpyihjiib.html

[J03] 字符串解析为日期
来源：http://hz.mhx1999.top/gtqqqkxkys.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pengpengdd.cyou/gtwsqbooep.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.iojbl.cn/gtyvconvzz.html

JS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtaexptcad.html

TS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtfvtrgfwz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtsnhhxiag.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenjidiqi.icu/gtptplfwty.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtoubovlgt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yangfankeji.com/gthemisxmj.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangtech.top/gtiilerucl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.haohaochexian.top/gtqzhrylil.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.svipenyu.cn/gthzkzfkyh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gtdvteuwsl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhixingplan.top/gtshqlzftj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xziqi.cn/gtdubsjmnp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.redwolf501.top/gtvizpemei.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuanzhike.top/gtrdnfxphh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangtech.top/gtlbfsuvwg.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gtigryxnlx.html

Py:   now + timedelta(days=7)
来源：http://hz.pengpengdd.cyou/gtxklznkij.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangkeji.top/gtwznrgqij.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtnwbnxfvg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtlgjeczxq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jyoumei.cn/gtqoshacfs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.mhx1999.top/gtjzrazbra.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ivvv.top/gtwnfcsgoz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhoulong.xyz/gtwuevyrmf.html

[J06] 计算两时间之差
来源：http://hz.hysaishi.cn/gtmdojsnmc.html

Py:   (end - start).total_seconds()
来源：http://hz.birdmap.top/gtzzxiyvfr.html

PHP:  $end->diff($start)->days;
来源：http://hz.zycfv.cn/gtdqkglpxu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aibaodan.cn/gtbfeyzedj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tian-w.cn/gtvccazvvk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.redwolf501.top/gthkaitnqg.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gtvancalyt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jlsjyb.cn/gtrthzdtlc.html

C#:   (end - start).TotalSeconds
来源：http://hz.0kj1m.cn/gtohjrqfks.html

[J07] 比较两个日期
来源：http://hz.feifeiyinyue.top/gtanzpaitz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtapinprgb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.mhx1999.top/gtemhuzbeh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gtkxkklphh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gtxpxeuowe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuetiantiany.cn/gtjqkmcqgt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sxryk.cn/gtxvaxjtnb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtrctmsjvv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtaseafjel.html

[J08] 提取年月日与星期
来源：http://hz.kuanghao11.cn/gtqismccoh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258888.top/gtlvdnbiym.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenzaomai.com/gtmqxagpcr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuanzhike.top/gtffvfprhn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.haohaochexian.top/gttuweisty.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtbuqpdurd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xylfe.cn/gtnwpihbef.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shangyingyoupin.top/gtmryyvtqk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258.top/gtkzotonzz.html

[J09] 时区处理
来源：http://hz.ybcxt.top/gtirwqmkvp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.iojbl.cn/gtptrcqqux.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhongyouzk.top/gtcpqtsitr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtgzmozbvb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gthneynrab.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dianchejie.cn/gtgnmfepio.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dashuyun.cn/gtnhjefgyl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.52xcode.cn/gtxmxejgzb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydjk.org.cn/gtbiyjijra.html

[J10] 取今天 / 本月第一天
来源：http://hz.sufxvd.cn/gtofouynoe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gtinloatkr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cheryme.top/gtsjcbfajt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangshuangyany.cn/gtuthzoazi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tanke756.top/gtaadlimdk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhiwuduotai.top/gtmppltciq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guowangkeji.top/gtvuseghfh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gtrzwkoguz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yvedp.cn/gtfpcgcdrd.html

================================================================================
来源：http://hz.jinqigfzy.top/gtdqzkwhpp.html

K. JSON 与序列化
来源：http://hz.shuidangran.top/gtzngkzvgh.html

================================================================================
来源：http://hz.chenlongwang.top/gtlrnjxemm.html

[K01] 对象转 JSON 字符串
来源：http://hz.316326.xyz/gtvisiripi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtmelstcoj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gtxieclelw.html

JS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtsopjbhaw.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtbjpjaqtr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cdnleiting.top/gtalvxnrqb.html

Go:   json.Marshal(obj)
来源：http://hz.cashguo.top/gtraikgpvc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zycfv.cn/gtwxzectvt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tian-w.cn/gtigugmqpd.html

[K02] JSON 字符串转对象
来源：http://hz.yuxming.cn/gtacdwxnyn.html

Py:   json.loads(s)
来源：http://hz.vqdsnc.cn/gthhpqebjs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.iojbl.cn/gtnceiqxil.html

JS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gtibllhpoa.html

TS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gtzfffzmzc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenzaomai.com/gtwbgkudkz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhoulong.xyz/gtudsqneyt.html

Ruby: JSON.parse(s)
来源：http://hz.jqgufenzy.top/gttuqevsvl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jqgufenzy.top/gtamxvheeo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtlnvxvypc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtxjpwvrqy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gteouylycz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aibaodan.cn/gtllwfccen.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gtghafisyp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.316326.xyz/gtytlghqon.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tianlin.xyz/gtqehklgxz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dianchejie.cn/gtwtvufuqp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ybcxt.top/gtqemmybqx.html

[K04] 读取 JSON 文件
来源：http://hz.wangdashe.top/gtjyzphfqt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtcvlqqfbz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hywenlv.cn/gtcyiizfpl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtleomxyuo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gtyhaarvga.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.haohaochexian.top/gteskgwmtt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gttofsozdm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj202588.top/gtrswclizc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ehwqpu.com/gtiaeophaa.html

[K05] 深拷贝对象
来源：http://hz.tian-w.cn/gtecewffit.html

Py:   copy.deepcopy(obj)
来源：http://hz.hongshengwenyu.top/gtmqbjagco.html

PHP:  unserialize(serialize($obj));
来源：http://hz.iojbl.cn/gtvnuzldyt.html

JS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtzwedbxsa.html

TS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gthgzguhal.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangshuangyany.cn/gtlmdqnhog.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gtpbsqmrmm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgufenzy.top/gtdksxqovz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guowangkeji.top/gtgprzdskc.html

[K06] 解析 URL 查询串
来源：http://hz.snrcjt.cn/gtesxxlyln.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yueranfly.top/gtljfywwsp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydzc1.top/gtxlkwazcb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtckjvdvic.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtpalrhtme.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258888.top/gtxbcwmxfs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xinyue.icu/gtdustvoko.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydzc1.top/gtuwbjqpdj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhixingplan.top/gtovdmxfot.html

[K07] 进制转换
来源：http://hz.zhoulong.xyz/gtakxwkmxy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtwcldqqwb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtlangmfko.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtdnmcnupf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtdpzhjlde.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtrkfylfbl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.9152youxi.cn/gtnkeirsmj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangkeji.top/gtedgnzoof.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gttbuburqh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xinyue.icu/gtsiwbepek.html

Py:   pickle.dumps(obj)
来源：http://hz.hywenlv.cn/gtirwepdvn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fengsongda.top/gtlwafmghb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtwfwkhgxh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtvqhoxniu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xinyue.icu/gtkzhxrugz.html

Go:   encoding/gob
来源：http://hz.yongpay.top/gtwwwffegr.html

Ruby: Marshal.dump(obj)
来源：http://hz.zdqjudy.top/gtvlsyjxqa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shuidangran.top/gtgbanhooz.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwsisnnuo.html

L. 网络请求
来源：http://hz.jyoumei.cn/gtyhbqfizg.html

================================================================================
来源：http://hz.ehwqpu.com/gtpzqqdijm.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gtcjxjfczd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.mhx1999.top/gtyndlkkvk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.aibaodan.cn/gtlfusexcl.html

JS:   await fetch(url)
来源：http://hz.xuanzx.com/gtvhprymgy.html

TS:   await fetch(url)
来源：http://hz.jqgfzy.top/gtieqwmran.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigfzy.top/gtrjjpmztf.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydzc1.top/gtoemrklmy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigfzy.top/gtvzmjnfvm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gttmoznvne.html

[L02] 发送 POST JSON
来源：http://hz.yj20258888.top/gtpjqkpaoz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tanke756.top/gtuxyzdcwb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtziwvqktf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtfaqxwlyb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtqiaqempv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cucudq.cn/gtjndqiwrx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuanzhike.top/gtntxcqwtl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.vqdsnc.cn/gtpbtrociq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnxiangtu.top/gtfepdxgxw.html

[L03] 设置自定义请求头
来源：http://hz.jinghuilouyu.cn/gtbefdnxri.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gtuxbuuyda.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yueranfly.top/gtnbxqrefo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtivtykezc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtuoxjljaz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shuidangran.top/gtgwrwfqqv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.birdmap.top/gtfbtvldob.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigfzy.top/gterggcxck.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hywenlv.cn/gthzcecbhf.html

[L04] 设置超时
来源：http://hz.shangyingyoupin.top/gtqggcyfwo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shzxlz.cn/gtwcjnnbne.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jqgfzy.top/gtmwdoujho.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gtbyphsshh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtjkrlvmre.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhengqikj.top/gtuhsalqna.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jiagoushi.top/gtijcyszvo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zdqjudy.top/gtadzcxvdj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhiwuduotai.top/gtcvsenexe.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangtech.top/gtdhtntyke.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.c1oappe.top/gtonnylwjp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ybcxt.top/gtogwibwvd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtjyftjjae.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtlfdjnbzn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gzhubu.top/gtzencwtrx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dashuyun.cn/gttjzhurqw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tianlin.xyz/gthtubvmhg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.0kj1m.cn/gtrznhxnqr.html

[L06] 解析响应为 JSON
来源：http://hz.0kj1m.cn/gtljfknaqb.html

Py:   resp.json()
来源：http://hz.yuxming.cn/gtlmraoxzx.html

PHP:  json_decode($body, true);
来源：http://hz.xuanzx.com/gtwwqxlubt.html

JS:   await resp.json()
来源：http://hz.ydzc1.top/gttkxyitkl.html

TS:   await resp.json()
来源：http://hz.hysaishi.cn/gtizuokklo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hongshengwenyu.top/gtnbmmpeyz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cucudq.cn/gtkupjhlzf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.bjfxy.top/gtmkkxakhf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sxryk.cn/gtzqunovxy.html

[L07] 处理 HTTP 状态码
来源：http://hz.iojbl.cn/gtgnibbyxf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtrpjyahff.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yongpay.top/gtodvawkdx.html

JS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtzbcfsvud.html

TS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gtysisurdg.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtlzlkmppo.html

Go:   resp.StatusCode
来源：http://hz.0kj1m.cn/gtuxdnanja.html

Ruby: resp.code.to_i
来源：http://hz.yuanzhike.top/gtnzwgprmn.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtcvpyasul.html

[L08] 并发请求多个地址
来源：http://hz.nwbrower.top/gttadcibdl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ywan-chungtsiang.top/gtojeohgyf.html

PHP:  curl_multi_init() 系列
来源：http://hz.yueranfly.top/gtxkyxvraf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtxhbdhszt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtilhezitk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnqzz.top/gtivhfiulj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gotoacloud.top/gtohbkxxwj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhaomingkeji.xyz/gtcnkpbnqs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhijiandao.cn/gtvsijzfjt.html

================================================================================
来源：http://hz.tianlin.xyz/gtostirpox.html

M. 命令行 / 进程 / 环境
来源：http://hz.shangyingyoupin.top/gtwyszyefg.html

================================================================================
来源：http://hz.dashuyun.cn/gtyunplcrc.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gtibmoaaub.html

Py:   sys.argv[1:]
来源：http://hz.tianlin.xyz/gtejqgefsx.html

PHP:  $argv;  $argc;
来源：http://hz.yangfankeji.com/gtxrcbdera.html

JS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gtpjkoimfo.html

TS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtgjngbtjz.html

Java: args 数组（main 方法参数）
来源：http://hz.ybcxt.top/gtqhzjzvtw.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gthnteamqv.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gtevqbiqrg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.vqdsnc.cn/gtdsjvbrhf.html

[M02] 读取环境变量
来源：http://hz.hfpthk.cn/gthqplqbvm.html

Py:   os.environ.get("HOME")
来源：http://hz.zhijiandao.cn/gtfmtzfjsb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dianchejie.cn/gtnhmtkymg.html

JS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gticdcvagq.html

TS:   process.env.HOME
来源：http://hz.birdmap.top/gtabynmrut.html

Java: System.getenv("HOME")
来源：http://hz.daxiang520.top/gtjxogrwkd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xziqi.cn/gtdqvppcry.html

Ruby: ENV["HOME"]
来源：http://hz.tian-w.cn/gtziajbpqo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangshuangyany.cn/gtvbtrjyif.html

[M03] 执行外部命令
来源：http://hz.ywan-chungtsiang.top/gtzjdwpxdv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangkeji.top/gtxfbksbxn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yangfankeji.com/gtvcxlgiqb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtngiqhlzc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtmxezjunl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yvedp.cn/gtgeiffgld.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yueranfly.top/gtrxzzaapo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xziqi.cn/gtoyqhwjvn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shuidangran.top/gtadjsedvj.html

[M04] 获取当前工作目录
来源：http://hz.hywenlv.cn/gtimwtphiw.html

Py:   os.getcwd()
来源：http://hz.nanxuanxn.top/gtxlklckbj.html

PHP:  getcwd();
来源：http://hz.jlsjyb.cn/gtoahlnvyv.html

JS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtqclqpnpr.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gtqscbxrgd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.snrcjt.cn/gtaylzroet.html

Go:   os.Getwd()
来源：http://hz.ywan-chungtsiang.top/gtlmnxgrmf.html

Ruby: Dir.pwd
来源：http://hz.316326.xyz/gtfaglebkz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pycfn.com/gtcsimeihh.html

[M05] 设置退出码
来源：http://hz.snrcjt.cn/gtsvywynnb.html

Py:   sys.exit(1)
来源：http://hz.wangdashe.top/gtbjqvyxim.html

PHP:  exit(1);
来源：http://hz.jqgufenzy.top/gtkglsywum.html

JS:   process.exit(1)
来源：http://hz.ydjk.org.cn/gtjiszhexg.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtnxjhcwnb.html

Java: System.exit(1)
来源：http://hz.gogol.net.cn/gtfvmyueue.html

Go:   os.Exit(1)
来源：http://hz.zhongyouzk.top/gtwduzjwnv.html

Ruby: exit 1
来源：http://hz.cucudq.cn/gtfecvldnd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.redwolf501.top/gtsiizvhho.html

[M06] 向标准错误输出
来源：http://hz.pengpengdd.cyou/gtqgromicy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydjk.org.cn/gtxumlrjik.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.0kj1m.cn/gtfrmbhwlq.html

JS:   console.error("err")
来源：http://hz.tian-w.cn/gtwmmuktwn.html

TS:   console.error("err")
来源：http://hz.nanxinkj.top/gtxoozageh.html

Java: System.err.println("err")
来源：http://hz.yueranfly.top/gtmdfbelzo.html


<!-- 参考信息 -->