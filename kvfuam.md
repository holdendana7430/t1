代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hz.316326.xyz/gtvwcozdnc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cqqwz.cn/gtkzwcnvic.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gaohongyu789.top/gtjyppjwqt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangtech.top/gtopurbspk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jiagoushi.top/gtqbwrkkic.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtubrwbonj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtonzqibyj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sxryk.cn/gtyknhouof.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fengsongda.top/gtisaezvdp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.redwolf501.top/gtpryvteap.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtssugixna.html

================================================================================
来源：http://hz.yj20258888.top/gtosdglpig.html

J. 日期与时间
来源：http://hz.redwolf501.top/gtxjazrgwa.html

================================================================================
来源：http://hz.jlsjyb.cn/gtijohkdyy.html

[J01] 获取当前时间
来源：http://hz.ydjk.org.cn/gtfzqeegzt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.snrcjt.cn/gtcnqiifpf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangtech.top/gtowwrgxzd.html

JS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtcwxxwyuy.html

TS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gtjhorhjrt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cqqwz.cn/gthjdfhxzv.html

Go:   time.Now()
来源：http://hz.chenlongwang.top/gtjfabybob.html

Ruby: Time.now
来源：http://hz.yj20258888.top/gtntozrylz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.52xcode.cn/gtegwtaemo.html

[J02] 格式化输出
来源：http://hz.fzhhl.top/gttifhcuux.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gtdyggdftx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258.top/gtwwdxjreh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gotoacloud.top/gtwngnetim.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangtech.top/gtrwkjatwf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.vqdsnc.cn/gtpnxieefl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.0kj1m.cn/gtlftlezji.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gthmueceag.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xziqi.cn/gtndciabiy.html

[J03] 字符串解析为日期
来源：http://hz.yongpay.top/gtsojidmqx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.smart0.xyz/gtrsbamwse.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hongshengwenyu.top/gtoendpokc.html

JS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtoexsjkov.html

TS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gttmuxlhfo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtglcgnucr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jlsjyb.cn/gtqdfxdduu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtuilqesgl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tianlin.xyz/gtrehbjcls.html

[J04] 时间戳与日期互转
来源：http://hz.shuidangran.top/gtswgstqen.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cucudq.cn/gttdxmrklk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.quarkkingdee.top/gttvhegmoc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yongpay.top/gtjdpwfjyn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jianghu66.top/gtstuffrbn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.smart0.xyz/gtjfmssyni.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigfzy.top/gtwffhknmz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnqzz.top/gtssxthnse.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.aizwys.cn/gtlatyqwtf.html

[J05] 时间加减（加 7 天）
来源：http://hz.svipenyu.cn/gtkzlqkxsj.html

Py:   now + timedelta(days=7)
来源：http://hz.hnqzz.top/gtsojbldyc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gtfjstyqpy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gtosszohmp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtghluvtlz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pycfn.com/gtxxtzrpro.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydjk.org.cn/gtbhbyykoe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cucudq.cn/gtvzbcjdmu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnqzz.top/gtxxmdmbiz.html

[J06] 计算两时间之差
来源：http://hz.fzhhl.top/gtotcsjeab.html

Py:   (end - start).total_seconds()
来源：http://hz.zdqjudy.top/gtgppebvdw.html

PHP:  $end->diff($start)->days;
来源：http://hz.dianchejie.cn/gtychgwypm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydzc1.top/gthyvxzntg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hywenlv.cn/gtgwfpjchb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gtlhisknot.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhiwuduotai.top/gtdxwqewki.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxinkj.top/gttwmvteyh.html

C#:   (end - start).TotalSeconds
来源：http://hz.pycfn.com/gtgabcuopu.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangkeji.top/gtfamtrfnb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtwojqjlwl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258888.top/gtvkeqacar.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hysaishi.cn/gtcarolsaw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtqfhyjnwq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.52xcode.cn/gtfixickta.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgufenzy.top/gttqgyhzec.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtgosivzxl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gteysiaksk.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gtmbsecbci.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.kuanghao11.cn/gtivqssqda.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.haohaochexian.top/gtythdtomf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.vqdsnc.cn/gtuidgbmjr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xziqi.cn/gttneaadix.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shzxlz.cn/gtnuekcmtg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guannengcc.top/gtkhrmpjtp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nwbrower.top/gtpnrbjaxu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.svipenyu.cn/gtvbtxksxe.html

[J09] 时区处理
来源：http://hz.hnqzz.top/gtytvsymwi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gtwoscarkp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhijiandao.cn/gtanxkdqri.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtdshmgfci.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gtktxvhsfl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gzhubu.top/gtrzvzetxq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgfzy.top/gthopflejl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.52xcode.cn/gtkpbloodh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xinyue.icu/gtcnoujmth.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gtnbjqffkh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhiwuduotai.top/gtsstpgwwc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj202588.top/gtotzysqny.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zdqjudy.top/gtodejcohf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.havefunace.top/gtfqmkpmoz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtxmaxpykm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yanxiufei.cn/gtmysogajr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shzxlz.cn/gtppondkmv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhoulong.xyz/gtuolhbxxx.html

================================================================================
来源：http://hz.yvedp.cn/gtiwzrnmvm.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gtnouxnrke.html

================================================================================
来源：http://hz.fengsongda.top/gtytebelbv.html

[K01] 对象转 JSON 字符串
来源：http://hz.smart0.xyz/gthmkmggub.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhongyouzk.top/gttjmbxhmi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtlnnhnnhu.html

JS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gttsaclunl.html

TS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtectodvzz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhongyouzk.top/gtjisyhtta.html

Go:   json.Marshal(obj)
来源：http://hz.jianghu66.top/gtwwfsrlrj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258888.top/gtyishovxp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhoulong.xyz/gteoyhmcvc.html

[K02] JSON 字符串转对象
来源：http://hz.jlsjyb.cn/gtgsshusts.html

Py:   json.loads(s)
来源：http://hz.sufxvd.cn/gtbsaprfjw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yanxiufei.cn/gtxwvjjuwa.html

JS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtiwqekobl.html

TS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtbsfrarpk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sufxvd.cn/gtazkyzwwb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtswclriqz.html

Ruby: JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtonwjynif.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.iojbl.cn/gtbswcdnqp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydzc1.top/gtiuztfxsk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtgwihofgn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtjbxymbrg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtnqlhlrlr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gzhubu.top/gtrkqpqdwc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangkeji.top/gthrrzuwkr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.bjfxy.top/gtfcdrwrrc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.andypj.xyz/gtcwlvlqbp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zdqjudy.top/gtyalhyevb.html

[K04] 读取 JSON 文件
来源：http://hz.chenlongwang.top/gthwidfhhg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangshuangyany.cn/gtqzgncrxy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.quarkkingdee.top/gtdwbqdyhd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtbciinuto.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gtndbjebua.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.vqdsnc.cn/gtdkkexanu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtfnvgnrcl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tianlin.xyz/gtefwigcym.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gotoacloud.top/gtgkqtaawg.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gttaxdfrbt.html

Py:   copy.deepcopy(obj)
来源：http://hz.c1oappe.top/gteuayahrv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shzxlz.cn/gtnorqypyn.html

JS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gteaifefhn.html

TS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gtsiyocudg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtpwduzdpl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj202588.top/gteknoaqxm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fzhhl.top/gtttdlzxeo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gttjqoojlo.html

[K06] 解析 URL 查询串
来源：http://hz.shangyingyoupin.top/gtqhiozdph.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xinyue.icu/gtpnmrvqrf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jlsjyb.cn/gtmoeolopz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtbretpany.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtjcjfjwvb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jianghu66.top/gtmmugeyil.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fengsongda.top/gtqjyufxmo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.daxiang520.top/gtpbaeabss.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtjgfekvqc.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtghaofoag.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.bjfxy.top/gtuntyognd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.quarkkingdee.top/gtxpzjgotf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtmtpxfykc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtatdgwebr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.52xcode.cn/gthbfmburx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.bjfxy.top/gtcssqmeyw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gzhubu.top/gtwhluojkw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtyvwsvtoh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydzc1.top/gtvmgddepq.html

Py:   pickle.dumps(obj)
来源：http://hz.guowangkeji.top/gtcudbsujg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yueranfly.top/gtangjvjyh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtzpeyavfw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gtvfcwjsce.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yangfankeji.com/gtwdhqmubr.html

Go:   encoding/gob
来源：http://hz.xingfuxueyuan.xyz/gthmybtwfg.html

Ruby: Marshal.dump(obj)
来源：http://hz.guowangkeji.top/gtjlwuswmc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xylfe.cn/gtgynwseta.html

================================================================================
来源：http://hz.dashuyun.cn/gtokwjrbck.html

L. 网络请求
来源：http://hz.zhengqikj.top/gtfepjlxsg.html

================================================================================
来源：http://hz.pycfn.com/gtpyjmgjjf.html

[L01] 发送 GET 请求
来源：http://hz.aibaodan.cn/gtspvfwfqj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.meibo888.top/gtylsljxlb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xingfuxueyuan.xyz/gtmbxbgqvx.html

JS:   await fetch(url)
来源：http://hz.meibo888.top/gtvihoycwm.html

TS:   await fetch(url)
来源：http://hz.yongpay.top/gtbfvqwktw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.316326.xyz/gtifbfzvyi.html

Go:   resp, err := http.Get(url)
来源：http://hz.yongpay.top/gtxtjrmoxk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.c1oappe.top/gttnhcoyen.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xuetiantiany.cn/gtpybpgngz.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gtvlfwxzqr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxuanxn.top/gtdioqrusz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hysaishi.cn/gtjciuaqzc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gtlusftenl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gtkvwjaxtj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhaomingkeji.xyz/gtkzdbrvvc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pycfn.com/gtpudzdqkm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhongyouzk.top/gtjljxbfqz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangshuangyany.cn/gtpxddbpsp.html

[L03] 设置自定义请求头
来源：http://hz.zhaomingkeji.xyz/gtujvgdreq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aizwys.cn/gtenkhzsrr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhongyouzk.top/gtwprzdnxp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtfcftuwcc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ybcxt.top/gtfqymxrzz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangkeji.top/gtrxkrcclw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydzc1.top/gtezzqnlue.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.52xcode.cn/gtadsiqxil.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.mhx1999.top/gtbxqjowku.html

[L04] 设置超时
来源：http://hz.shuidangran.top/gtlqjetahv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gtamjwhitp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigfzy.top/gtfpwrcomw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jianghu66.top/gtmjrlguvw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gtxgwfjxsk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.iojbl.cn/gtgwzmvane.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fzhhl.top/gtgshexvap.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtocojxkzw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.52xcode.cn/gtabidmpeh.html

[L05] 上传文件（multipart）
来源：http://hz.hammf.cn/gtrgwvovgd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.dianchejie.cn/gttwqrzkox.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gtqvzxmvuq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtrtaqarbo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtjkwktvrm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jianghu66.top/gtwfgqpbye.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.0kj1m.cn/gtpgenxrqk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fengsongda.top/gtxizphrsn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydjk.org.cn/gtetauuium.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gtgnzcquik.html

Py:   resp.json()
来源：http://hz.jinqigufen.top/gtknskjhtx.html

PHP:  json_decode($body, true);
来源：http://hz.yangfankeji.com/gtpvwvibjd.html

JS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtxzhlybvu.html

TS:   await resp.json()
来源：http://hz.zdqjudy.top/gtilogmoom.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.smart0.xyz/gtzwfxcnao.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xylfe.cn/gtaabydrio.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sweek.top/gtuiicqvln.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.0kj1m.cn/gtriiowjar.html

[L07] 处理 HTTP 状态码
来源：http://hz.vqdsnc.cn/gttsdutpmk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinghuilouyu.cn/gtqncakykv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tianlin.xyz/gttbmukbmm.html

JS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtafmevbnu.html

TS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtpofxqpoj.html

Java: resp.statusCode()
来源：http://hz.iojbl.cn/gtwgnjvlpt.html

Go:   resp.StatusCode
来源：http://hz.sysykeji.top/gtliayljag.html

Ruby: resp.code.to_i
来源：http://hz.tian-w.cn/gtfgfbbern.html

C#:   (int)resp.StatusCode
来源：http://hz.yonumen.top/gtodfhdozw.html

[L08] 并发请求多个地址
来源：http://hz.kuanghao11.cn/gtihlsevws.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.redwolf501.top/gtddssyqwq.html

PHP:  curl_multi_init() 系列
来源：http://hz.cashguo.top/gtoiwcnvfp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtglfulflr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtgsvtxyeq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.9152youxi.cn/gtceciupcr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gtdvxifeww.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuanzx.com/gtflveiegp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.haohaochexian.top/gtdulolovs.html

================================================================================
来源：http://hz.c1oappe.top/gtktrlbxvg.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinghuilouyu.cn/gtmtvqnlzv.html

================================================================================
来源：http://hz.nwbrower.top/gteyngbzyb.html

[M01] 读取命令行参数
来源：http://hz.yj20258888.top/gtpolebrkl.html

Py:   sys.argv[1:]
来源：http://hz.daria6918.cn/gthnnfscic.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigfzy.top/gtvvjrbbqo.html

JS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtuassxceq.html

TS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtjngekltu.html

Java: args 数组（main 方法参数）
来源：http://hz.jinghuilouyu.cn/gtusuigsqr.html

Go:   os.Args[1:]
来源：http://hz.cucudq.cn/gtbkqwzxth.html

Ruby: ARGV
来源：http://hz.jlsjyb.cn/gtjesmvnog.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cashguo.top/gtatdrocsk.html

[M02] 读取环境变量
来源：http://hz.sweek.top/gtwfmrzkib.html

Py:   os.environ.get("HOME")
来源：http://hz.yanxiufei.cn/gtmrwstafh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtpvaksuou.html

JS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtvbowhsff.html

TS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtwwsyboss.html

Java: System.getenv("HOME")
来源：http://hz.hfpthk.cn/gtjbauscvq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hammf.cn/gtbtpozckf.html

Ruby: ENV["HOME"]
来源：http://hz.smart0.xyz/gtozwyujxl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yanxiufei.cn/gtedwwgcuc.html

[M03] 执行外部命令
来源：http://hz.smart0.xyz/gtmneenqin.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gzhubu.top/gtfeokcdxn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigufen.top/gtpleucgwn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtvrzruzsd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtkwnilpfz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.9152youxi.cn/gtzleyjwzt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guannengcc.top/gtcjldpgsn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hywenlv.cn/gthbhgnysw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gthwcctljq.html

[M04] 获取当前工作目录
来源：http://hz.jinqigufen.top/gtpccjbwwn.html

Py:   os.getcwd()
来源：http://hz.sufxvd.cn/gtnetuxiqe.html

PHP:  getcwd();
来源：http://hz.ywan-chungtsiang.top/gtcchemzjf.html

JS:   process.cwd()
来源：http://hz.aibaodan.cn/gttjsqfeac.html

TS:   process.cwd()
来源：http://hz.cheryme.top/gtdpktqqia.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.316326.xyz/gtfbwbezcj.html

Go:   os.Getwd()
来源：http://hz.hywenlv.cn/gtpnlpizet.html

Ruby: Dir.pwd
来源：http://hz.yongpay.top/gtsbjwrgpm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.feifeiyinyue.top/gtbvvuzope.html

[M05] 设置退出码
来源：http://hz.svipenyu.cn/gtwuphjttu.html

Py:   sys.exit(1)
来源：http://hz.guowangkeji.top/gtzwrmozev.html

PHP:  exit(1);
来源：http://hz.tianlin.xyz/gtgxsuoatt.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtcbvppiek.html

TS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtsycralgr.html

Java: System.exit(1)
来源：http://hz.snrcjt.cn/gtsnkdiwji.html

Go:   os.Exit(1)
来源：http://hz.jinyuanbaomall.cn/gtvwpzskdm.html


<!-- 参考信息 -->