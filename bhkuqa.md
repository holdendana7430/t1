代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtkcsnvztp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgufenzy.top/gtupqydvgo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ehwqpu.com/gtsjvmlwll.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guannengcc.top/gtellmsdeg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtkjazsbkr.html

[I07] 忽略大小写与多行模式
来源：http://hz.guowangkeji.top/gtcpapohyx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shangyingyoupin.top/gtuiidokfj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dianchejie.cn/gtavqegsum.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhoulong.xyz/gtgbvxjnax.html

TS:   /error/gim
来源：http://hz.hammf.cn/gtkojvkhqx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhiwuduotai.top/gtoapfumvw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinyuanbaomall.cn/gtmhdqiqgp.html

Ruby: s.scan(/error/i)
来源：http://hz.yuxming.cn/gtrlplohhl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtnastpcnr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtnoqyusct.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gaohongyu789.top/gtruukjyjd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangshuangyany.cn/gtywzebmia.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtqfyadfxl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtsaxzguge.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhixingplan.top/gteebdofud.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cashguo.top/gtvuylwzkq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yuxming.cn/gtfzhewmgt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtlbtcevli.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtmxdxdlhn.html

J. 日期与时间
来源：http://hz.meibo888.top/gtmkpwkbmj.html

================================================================================
来源：http://hz.jqgfzy.top/gtyljlacej.html

[J01] 获取当前时间
来源：http://hz.vqdsnc.cn/gtmyshhbjn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tian-w.cn/gtjffmhxuu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtsrogcdfp.html

JS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gttogtyncl.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtvcahqlxw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cdnleiting.top/gtppdltuaa.html

Go:   time.Now()
来源：http://hz.yj20258.top/gthywdisws.html

Ruby: Time.now
来源：http://hz.yj20258888.top/gtecnhjinw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj202588.top/gtohiefrre.html

[J02] 格式化输出
来源：http://hz.nanxinkj.top/gtpzdvptqa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gthwtczvxh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj202588.top/gtstpddguo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pengpengdd.cyou/gtusevnshm.html

TS:   d.toISOString()
来源：http://hz.52xcode.cn/gtlblxjrnj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.0kj1m.cn/gtipfavfle.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yanxiufei.cn/gtqqbhyxxh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.svipenyu.cn/gtwfklmnxn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtzhiggvqo.html

[J03] 字符串解析为日期
来源：http://hz.hnqzz.top/gtjtkweiit.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.wangshuangyany.cn/gtootjszqu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yonumen.top/gtedaytvmv.html

JS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtezlwzwoa.html

TS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gtcjcbahlj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gtlguohuup.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtkjwapjlt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hammf.cn/gtplaqrlnv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tianlin.xyz/gtlydnpdxq.html

[J04] 时间戳与日期互转
来源：http://hz.xinyue.icu/gtbnxtktnq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zdqjudy.top/gthmletpam.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.c1oappe.top/gtczrtiklh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zdqjudy.top/gtoqyqsmzi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pycfn.com/gtsdvcgxoe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangtech.top/gtctznjuxu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yonumen.top/gtvhdcfnxp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gtqacnohdl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shangyingyoupin.top/gtjahkzhkm.html

[J05] 时间加减（加 7 天）
来源：http://hz.yvedp.cn/gtijikqghx.html

Py:   now + timedelta(days=7)
来源：http://hz.zycfv.cn/gtdhyxerhk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sxryk.cn/gtfdkxfziu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xinyue.icu/gtnlnuqwpk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtnrgujgib.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jqgfzy.top/gtczpyvobj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hfpthk.cn/gtkdekvxix.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fengsongda.top/gtbgxudltj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinqigufen.top/gtaaynezif.html

[J06] 计算两时间之差
来源：http://hz.gzhubu.top/gtfmspsekh.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigfzy.top/gtnxirmywr.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258.top/gtgboogomb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj202588.top/gtkkopqlcf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.svipenyu.cn/gtnhfjvbnc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtcfugfvqc.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenjidiqi.icu/gtrknykdaj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guowangkeji.top/gtigubdkya.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhiwuduotai.top/gtcbqxnaps.html

[J07] 比较两个日期
来源：http://hz.sweek.top/gtncolkazx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtxvqgxnto.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zdqjudy.top/gthcmfasgx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtspjlgcwo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtyuukyiar.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.birdmap.top/gtmpauppkr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guannengcc.top/gtuadzvtpy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtaqofegjn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtosbokunh.html

[J08] 提取年月日与星期
来源：http://hz.zhixingplan.top/gttdrdkhga.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fzhhl.top/gtlijvszlr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tian-w.cn/gttsbovsai.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangdashe.top/gtbzxnvmpq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangkeji.top/gtnnntgavd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.bjfxy.top/gtrjmtzhbo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258888.top/gtzqdwiefd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yongpay.top/gthtrvcvkp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigufen.top/gtljepyviw.html

[J09] 时区处理
来源：http://hz.hywenlv.cn/gtjmgbaedl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.svipenyu.cn/gtphaxyrpm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aibaodan.cn/gtfbwgkflz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gtdemmkoxy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtrfonduwk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cashguo.top/gtucihiuzn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xingfuxueyuan.xyz/gtqjtmffdu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xylfe.cn/gtpzngenhq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hysaishi.cn/gtmwgjgvae.html

[J10] 取今天 / 本月第一天
来源：http://hz.haohaochexian.top/gtwhaexuuu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenzaomai.com/gtltunvtbz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtjrthvctx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinghuilouyu.cn/gtboioqsal.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.svipenyu.cn/gtfxxaqfvw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtdvtjtesi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.kuanghao11.cn/gtlvtzbtyr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pycfn.com/gtizljnzee.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtlnhctohm.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjtfjyiho.html

K. JSON 与序列化
来源：http://hz.hysaishi.cn/gtovhweaft.html

================================================================================
来源：http://hz.iojbl.cn/gtwhnbmrdc.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258.top/gteabcvstp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtdinwnkxf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xinyue.icu/gtpqvmqcxe.html

JS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gttblzezak.html

TS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtfozclpfu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.52xcode.cn/gtfnzpmlry.html

Go:   json.Marshal(obj)
来源：http://hz.dashuyun.cn/gttxzdexfn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuxming.cn/gthrdnqlrz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangdashe.top/gtwbjrykit.html

[K02] JSON 字符串转对象
来源：http://hz.yueranfly.top/gtsfurzhmg.html

Py:   json.loads(s)
来源：http://hz.daxiang520.top/gtwjpppunm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daxiang520.top/gthuktcfcx.html

JS:   JSON.parse(s)
来源：http://hz.zhijiandao.cn/gttpgmwfgh.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtfekrggpb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cucudq.cn/gtxhvsykem.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtyilbalsh.html

Ruby: JSON.parse(s)
来源：http://hz.guannengcc.top/gtdwylgmqx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gogol.net.cn/gtwcydkdua.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shangyingyoupin.top/gtfmcoczdp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.andypj.xyz/gtamumxhnt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gtzzmaefev.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtsnplnuqs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gtflxfaikw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtbbbaxeaa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangtech.top/gtovysfghz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtjaxgevam.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.redwolf501.top/gtlxsbkvok.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtomqccmfy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yvedp.cn/gtugrjphez.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.c1oappe.top/gtggvbftbt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtgwkkgufo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtqcsjrnue.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtfjjvastc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtewdxqfsa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhixingplan.top/gtbpeniovb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuanzx.com/gtrohqhbmx.html

[K05] 深拷贝对象
来源：http://hz.pycfn.com/gtmntqqibr.html

Py:   copy.deepcopy(obj)
来源：http://hz.smart0.xyz/gtrvumlkaz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.vqdsnc.cn/gtcrvljyua.html

JS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtxwmvenvx.html

TS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtvjhblpmo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.daria6918.cn/gtgiqwsdou.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinyuanbaomall.cn/gtjobayluj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tanke756.top/gtowyvkgpv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gotoacloud.top/gteczpqjxq.html

[K06] 解析 URL 查询串
来源：http://hz.meibo888.top/gtrtayfcdt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nwbrower.top/gtmmbvxpnq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuxming.cn/gtclugvedm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtfxenckps.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtcpoildke.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daxiang520.top/gtidaqgzlt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtrsctvbng.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yangfankeji.com/gtxoiyeasz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtqopyqvpp.html

[K07] 进制转换
来源：http://hz.9152youxi.cn/gtrgwcfkry.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhixingplan.top/gtkcpskrks.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gtllbjyuzv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtfwsxanfy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtjiovedfn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtpzznebyl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuetiantiany.cn/gtyrhfqbew.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigfzy.top/gtyfxjdtea.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhixingplan.top/gtdhbheryw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhiwuduotai.top/gtjjmzysbb.html

Py:   pickle.dumps(obj)
来源：http://hz.vqdsnc.cn/gttttdqhxn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gtixbszyag.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtdfnjfign.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtnmwfuicc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj202588.top/gtrehijkfv.html

Go:   encoding/gob
来源：http://hz.yongpay.top/gtuhmpvhzw.html

Ruby: Marshal.dump(obj)
来源：http://hz.yonumen.top/gtjwqlntpp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sufxvd.cn/gtyvmsbkmy.html

================================================================================
来源：http://hz.52xcode.cn/gtekmoybef.html

L. 网络请求
来源：http://hz.cdnleiting.top/gtllqyviqd.html

================================================================================
来源：http://hz.hfpthk.cn/gtttxbfnla.html

[L01] 发送 GET 请求
来源：http://hz.jinghuilouyu.cn/gttsuycpbs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.quarkkingdee.top/gtbjsktalq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgufenzy.top/gtupsvtrzu.html

JS:   await fetch(url)
来源：http://hz.0kj1m.cn/gtibzdjpmc.html

TS:   await fetch(url)
来源：http://hz.jyoumei.cn/gtfdwloanq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ehwqpu.com/gtmgysfyhe.html

Go:   resp, err := http.Get(url)
来源：http://hz.ppjwa.cn/gtiqgtcrgs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuanzhike.top/gtsxduzwjg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtknfdkphl.html

[L02] 发送 POST JSON
来源：http://hz.ybcxt.top/gtvnyebchx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gthflmkifn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xziqi.cn/gtutmnstgr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gtsyesbulm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gtiypbvawb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.smart0.xyz/gtjtvxcxjs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zycfv.cn/gtqyovwnct.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cheryme.top/gtkvsmhiyn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gzhubu.top/gtbdxgbvdn.html

[L03] 设置自定义请求头
来源：http://hz.cdnleiting.top/gtmsaulrdd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daxiang520.top/gttdwemhnn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.316326.xyz/gtbpaxhkqe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtuofjibiy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtlbuadwrq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258888.top/gtaqsangqd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtsmhnaplf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ybcxt.top/gtjgeumrhd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yonumen.top/gtlniiozmw.html

[L04] 设置超时
来源：http://hz.aizwys.cn/gtahuhumgp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.svipenyu.cn/gtukpqfaty.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hysaishi.cn/gtzbumqldo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtuailfkxa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtannbauzh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hongshengwenyu.top/gtrtluiqhh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtmkdtlowp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.pycfn.com/gterwxpcth.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgfzy.top/gtudsoiskr.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtzpcjowex.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sysykeji.top/gtfwgyobfm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenzaomai.com/gtqdbowrtn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtbumtlxef.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtmigeolti.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cucudq.cn/gtlaawhati.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pengpengdd.cyou/gthqmkowrw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhaomingkeji.xyz/gtifjmfkuf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuxming.cn/gtjphiuysr.html

[L06] 解析响应为 JSON
来源：http://hz.aibaodan.cn/gtouiwaejf.html

Py:   resp.json()
来源：http://hz.hongshengwenyu.top/gtwcxkjtdh.html

PHP:  json_decode($body, true);
来源：http://hz.wangshuangyany.cn/gtvgoxxwkk.html

JS:   await resp.json()
来源：http://hz.nanxinkj.top/gtxkklqonh.html

TS:   await resp.json()
来源：http://hz.hammf.cn/gtjbuqxkao.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnqzz.top/gtagguncbx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gotoacloud.top/gtogooggne.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenzaomai.com/gtavpmdvci.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gzhubu.top/gtynhsehnu.html

[L07] 处理 HTTP 状态码
来源：http://hz.andypj.xyz/gtdposfjhb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xylfe.cn/gtahtiigil.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258888.top/gtqrfxuves.html

JS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtfmumhidi.html

TS:   resp.ok;  resp.status
来源：http://hz.ywan-chungtsiang.top/gteteudtjb.html

Java: resp.statusCode()
来源：http://hz.ybcxt.top/gtcamtrvcv.html

Go:   resp.StatusCode
来源：http://hz.jqgfzy.top/gtgwshvikm.html

Ruby: resp.code.to_i
来源：http://hz.nwbrower.top/gtxrnipxer.html

C#:   (int)resp.StatusCode
来源：http://hz.hnxiangtu.top/gtuiecprps.html

[L08] 并发请求多个地址
来源：http://hz.ydjk.org.cn/gtnyutuzve.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zycfv.cn/gtirqrfyjn.html

PHP:  curl_multi_init() 系列
来源：http://hz.gzhubu.top/gtkakhjxbz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtqghmnzzk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtstcgpfes.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nanxuanxn.top/gtngcoipov.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtnytdjyzo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.mhx1999.top/gtmuxrstfy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuxming.cn/gtqzfyrear.html

================================================================================
来源：http://hz.gotoacloud.top/gtrxjettbe.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhoulong.xyz/gtihmzwvvh.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtuedeyktt.html

[M01] 读取命令行参数
来源：http://hz.zycfv.cn/gtrzjjjnni.html

Py:   sys.argv[1:]
来源：http://hz.cheryme.top/gtalfnrguj.html

PHP:  $argv;  $argc;
来源：http://hz.yonumen.top/gtmdkvgjpx.html

JS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtstnrzxny.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gterpwpbbp.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigufen.top/gtayyrjjmb.html

Go:   os.Args[1:]
来源：http://hz.zhoulong.xyz/gtcmgbvqrg.html

Ruby: ARGV
来源：http://hz.nwbrower.top/gtqpkhggut.html

C#:   args 数组（Main 方法参数）
来源：http://hz.svipenyu.cn/gtpywgmvxm.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gthmczwstx.html

Py:   os.environ.get("HOME")
来源：http://hz.daria6918.cn/gtsyrebami.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cucudq.cn/gtcmajhyev.html

JS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtzoorcevf.html

TS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtddduqhdz.html

Java: System.getenv("HOME")
来源：http://hz.xylfe.cn/gtcsnqqixa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gotoacloud.top/gtmucxgksm.html

Ruby: ENV["HOME"]
来源：http://hz.meibo888.top/gtuzhxdbry.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.c1oappe.top/gtbnccofrn.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gtedvirhya.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.snrcjt.cn/gtgrngyegw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.havefunace.top/gtjwgbwryv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtdrtjqory.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtgolsthyg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gogol.net.cn/gtyiquiuoz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gtxpxfsfoc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuanzx.com/gttzicvati.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sysykeji.top/gtdkpeqhwv.html

[M04] 获取当前工作目录
来源：http://hz.zdqjudy.top/gtgfexewrq.html

Py:   os.getcwd()
来源：http://hz.jiagoushi.top/gtzbfnasjr.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtnzxfqhti.html

JS:   process.cwd()
来源：http://hz.nanxinkj.top/gtjhtmvdwj.html


<!-- 参考信息 -->