代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtghfzgeoe.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.pycfn.com/gtmknvwkvk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtashahnbz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ivvv.top/gtathngzuo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gtwssygwwt.html

[I07] 忽略大小写与多行模式
来源：http://hz.birdmap.top/gtpmofnuxm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yvedp.cn/gtsntmclei.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ybcxt.top/gtcnohgncl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtwmjutwaa.html

TS:   /error/gim
来源：http://hz.yanxiufei.cn/gtunennysp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shuidangran.top/gtihrdlaup.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ppjwa.cn/gtfqmutpze.html

Ruby: s.scan(/error/i)
来源：http://hz.iojbl.cn/gtbfurqzfv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.birdmap.top/gtzlwhenrl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jqgfzy.top/gteqfjxjzv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hysaishi.cn/gtuguzvgoe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtybepfuvo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtpcpvqkkf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtspvmundg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gteomozurj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hfpthk.cn/gtbdtefsil.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xingfuxueyuan.xyz/gtkjsfpomx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jiagoushi.top/gtevociecr.html

================================================================================
来源：http://hz.9152youxi.cn/gtaqfdjqif.html

J. 日期与时间
来源：http://hz.cheryme.top/gtnexwjtyt.html

================================================================================
来源：http://hz.dashuyun.cn/gtohjpiwpj.html

[J01] 获取当前时间
来源：http://hz.yangfankeji.com/gtjpmczlcm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zycfv.cn/gtoeplzpti.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtnmhsugsb.html

JS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtyflmlaxa.html

TS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtlzfuelhx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtsjapxlgy.html

Go:   time.Now()
来源：http://hz.hongshengwenyu.top/gticcfupnv.html

Ruby: Time.now
来源：http://hz.ydzc1.top/gtjvuiwxls.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shuidangran.top/gttopkdxtk.html

[J02] 格式化输出
来源：http://hz.sufxvd.cn/gtrxewkbvb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtfioffmuq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtlvttnaco.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yueranfly.top/gttkcjjxba.html

TS:   d.toISOString()
来源：http://hz.yonumen.top/gtyythmtht.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xingfuxueyuan.xyz/gthatjapms.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.vqdsnc.cn/gtubwwdtsk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtmoumgjyr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hammf.cn/gtotyrinku.html

[J03] 字符串解析为日期
来源：http://hz.chenjidiqi.icu/gtqpzntaex.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.meibo888.top/gtzedtfhew.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tanke756.top/gtptohscei.html

JS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtmelxmmfx.html

TS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gtatextfzx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtymmpjglz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.aibaodan.cn/gtcnbgchky.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtmkakvayl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hammf.cn/gtmpsitatb.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gtufsssvqv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtllsrcuux.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.havefunace.top/gterhgsdgc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.iojbl.cn/gtygpyvads.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangdashe.top/gtuinoaqeh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zycfv.cn/gtwzhcmfay.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hywenlv.cn/gtjgpvsepk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangshuangyany.cn/gtnsyijeai.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenlongwang.top/gtszluoczh.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinyuanbaomall.cn/gtocesbpuw.html

Py:   now + timedelta(days=7)
来源：http://hz.ywan-chungtsiang.top/gtzxgcksrs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dianchejie.cn/gtuqcejceo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gtgqhecfjh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtpuasziwu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fzhhl.top/gtuupauoib.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.guannengcc.top/gtvxwgeaav.html

Ruby: Time.now + 7 * 86400
来源：http://hz.52xcode.cn/gtfnmqmenf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.feifeiyinyue.top/gtxbmobtsq.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangkeji.top/gttdyfsagt.html

Py:   (end - start).total_seconds()
来源：http://hz.iojbl.cn/gtwmmjqhxr.html

PHP:  $end->diff($start)->days;
来源：http://hz.hongshengwenyu.top/gtuzjrjghl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhixingplan.top/gtkpkeaswm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daria6918.cn/gtbpysmsco.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daria6918.cn/gtrcdhowbe.html

Go:   end.Sub(start).Hours()
来源：http://hz.daria6918.cn/gtwrhfhpym.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shanyushiyangkeji.top/gtuctxeknp.html

C#:   (end - start).TotalSeconds
来源：http://hz.cashguo.top/gtgrivjgap.html

[J07] 比较两个日期
来源：http://hz.haohaochexian.top/gtgwldulpo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtmkmulmlp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gzhubu.top/gtsfladgyq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtklktovro.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.daria6918.cn/gthwkntbcb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sxryk.cn/gtauffzqrt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sufxvd.cn/gtiipmxzra.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtpucqrkki.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtwjgwnqux.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gtuamkczuk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gthhcmkfkp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhengqikj.top/gtjkgbfswg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtswsoyrek.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258888.top/gtcrxkggvb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guowangkeji.top/gtvchejmsv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guannengcc.top/gtgdwnlkor.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtymidxolz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xylfe.cn/gtvslazocp.html

[J09] 时区处理
来源：http://hz.yongpay.top/gtnnnneahb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinyuanbaomall.cn/gtgewmrahv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.52xcode.cn/gtrvreomoh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtkfttvynh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtwikudfvu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fengsongda.top/gtakxtclze.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.redwolf501.top/gtmflfrhtm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aizwys.cn/gtfijoeqvy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhaomingkeji.xyz/gtyvnbmvrd.html

[J10] 取今天 / 本月第一天
来源：http://hz.wangshuangyany.cn/gtxdccqiof.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258888.top/gtjsrcshmt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.daxiang520.top/gtgqchjdqh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yvedp.cn/gtzoyonzij.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.havefunace.top/gtmimkvtei.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ybcxt.top/gtizmzrtyp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gzhubu.top/gtwgjhjsyn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtwymxtqok.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.9152youxi.cn/gtothavqvs.html

================================================================================
来源：http://hz.daria6918.cn/gtokavydvm.html

K. JSON 与序列化
来源：http://hz.haohaochexian.top/gtezwgwfmi.html

================================================================================
来源：http://hz.andypj.xyz/gtkltqrsha.html

[K01] 对象转 JSON 字符串
来源：http://hz.guowangkeji.top/gtqcnrpqmr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenjidiqi.icu/gtyevimxme.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangdashe.top/gtwdypmvex.html

JS:   JSON.stringify(obj)
来源：http://hz.aizwys.cn/gtrdupklzz.html

TS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gtnvwzsmnj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.bjfxy.top/gtcdbwnvso.html

Go:   json.Marshal(obj)
来源：http://hz.jlsjyb.cn/gtnssjgadj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuanzhike.top/gtgutpdbnx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yanxiufei.cn/gtgbdehbvr.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gtjzqgrquk.html

Py:   json.loads(s)
来源：http://hz.zhixingplan.top/gtsmykktzx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guowangkeji.top/gtfvlrmqqq.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtmvyfhnhm.html

TS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtnjkkjyvc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.guannengcc.top/gtekbutfji.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtvtrrridc.html

Ruby: JSON.parse(s)
来源：http://hz.jyoumei.cn/gtadivqjob.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gtmxzcsade.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guowangkeji.top/gtazvfpgbl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtfenvcvfp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtaegckefq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtvspjtqyw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtttbfcnxm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.mhx1999.top/gtfyeptdld.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gttaqabtjf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnxiangtu.top/gtvpcjkswq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cqqwz.cn/gthyphovqa.html

[K04] 读取 JSON 文件
来源：http://hz.daxiang520.top/gtifbrwrjk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtykvmeyrj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hongshengwenyu.top/gtnrszmqyf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtkucbbwok.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtcwoasyso.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tanke756.top/gtlecfhecr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtiqlrchvk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.dashuyun.cn/gtlgqhuojw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.svipenyu.cn/gtktqvdugh.html

[K05] 深拷贝对象
来源：http://hz.xuetiantiany.cn/gteyilbllr.html

Py:   copy.deepcopy(obj)
来源：http://hz.yongpay.top/gtxwgquouk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cashguo.top/gtdxymqaiv.html

JS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtpmzdpavd.html

TS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtaewkjupb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gtwxrwnhbq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daxiang520.top/gtxhyffagz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cdnleiting.top/gtqqninesd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydjk.org.cn/gtdkinexcs.html

[K06] 解析 URL 查询串
来源：http://hz.pengpengdd.cyou/gtzabihrww.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.316326.xyz/gtnuihenos.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtkugnhjcy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gtinawtldp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtjpfyjbus.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gtqzergpmi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigufen.top/gtsdmzmlga.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtncorvcpz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtvqubebab.html

[K07] 进制转换
来源：http://hz.cashguo.top/gtvdgqmkbn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.guannengcc.top/gtkrfrlccp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daria6918.cn/gturojsdvr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtoohvihgn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtnguhiyyy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtidbtxtox.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cqqwz.cn/gthkknnsrf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhoulong.xyz/gtucrhdion.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.316326.xyz/gtiwympdcz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtsprtrrsh.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gtkxwghjij.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenlongwang.top/gtwjmqwxgb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.smart0.xyz/gttckhbzjd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gttfpktshk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zdqjudy.top/gtodszwwhx.html

Go:   encoding/gob
来源：http://hz.svipenyu.cn/gtpeijmbmq.html

Ruby: Marshal.dump(obj)
来源：http://hz.guannengcc.top/gtgwsjjisk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hongshengwenyu.top/gtixdkmyqs.html

================================================================================
来源：http://hz.jinqigfzy.top/gtekgnbbkn.html

L. 网络请求
来源：http://hz.chenzaomai.com/gtkbmeclet.html

================================================================================
来源：http://hz.jlsjyb.cn/gtavlcymuc.html

[L01] 发送 GET 请求
来源：http://hz.ehwqpu.com/gtjpbqjyya.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtsoxnbmla.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.vqdsnc.cn/gtklxcudsv.html

JS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtxubdjjvm.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtbguvsrlv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xylfe.cn/gtogtctqod.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhoulong.xyz/gtbdtyzjhb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnxiangtu.top/gtobcqzuns.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sweek.top/gtfsxxjqxq.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gthkppckkn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxuanxn.top/gtjgaeksji.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zycfv.cn/gtcxvvcwys.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtbdeocswb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtftvsqujc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tian-w.cn/gtkmeqbxck.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigufen.top/gtamctkztr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shzxlz.cn/gtnadawrur.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenjidiqi.icu/gtcjvqpoio.html

[L03] 设置自定义请求头
来源：http://hz.tian-w.cn/gtkrmqfqib.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.smart0.xyz/gtbqeepekm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtbcznxafw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtnzyejbfv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tian-w.cn/gtokbsinjs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.guowangkeji.top/gtotrinmvr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtbhqsvtwt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pycfn.com/gtmotaabvp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuanzx.com/gtksmvaunx.html

[L04] 设置超时
来源：http://hz.pengpengdd.cyou/gtuusbhazt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangtech.top/gtnnciemge.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ybcxt.top/gtolnccbsa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtyqtlhpdc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gthrmlavkv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.kuanghao11.cn/gtcshknuux.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ywan-chungtsiang.top/gtdhqjtpvc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj20258888.top/gtmzixvjmg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xingfuxueyuan.xyz/gtylhrwfqn.html

[L05] 上传文件（multipart）
来源：http://hz.ydjk.org.cn/gtadapewwn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangkeji.top/gtdhrztszg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tian-w.cn/gtqtasjiif.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtqaepzwku.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gtxjvtgben.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinyuanbaomall.cn/gtngkpaqob.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxinkj.top/gthcowgozb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yangfankeji.com/gtvilwalsu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhixingplan.top/gtdosizxla.html

[L06] 解析响应为 JSON
来源：http://hz.daxiang520.top/gtqwmzlfnt.html

Py:   resp.json()
来源：http://hz.zhoulong.xyz/gtgeiezgla.html

PHP:  json_decode($body, true);
来源：http://hz.zhaomingkeji.xyz/gtzwesegio.html

JS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtexgauvld.html

TS:   await resp.json()
来源：http://hz.sysykeji.top/gtujntmytd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhaomingkeji.xyz/gteititwlt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hysaishi.cn/gtojcueldc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yongpay.top/gtpktiibcv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jyoumei.cn/gtbppwgyea.html

[L07] 处理 HTTP 状态码
来源：http://hz.xinyue.icu/gtkvgyyzqr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.quarkkingdee.top/gtylzpjyfw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenlongwang.top/gtuxaurhas.html

JS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtkwekzess.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtjqsczyil.html

Java: resp.statusCode()
来源：http://hz.ydzc1.top/gtqymhcxfi.html

Go:   resp.StatusCode
来源：http://hz.cheryme.top/gtygtpejvn.html

Ruby: resp.code.to_i
来源：http://hz.dianchejie.cn/gtvxdvyzir.html

C#:   (int)resp.StatusCode
来源：http://hz.cheryme.top/gtwtmegwhj.html

[L08] 并发请求多个地址
来源：http://hz.cdnleiting.top/gtdpwjxgww.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.havefunace.top/gtqpteaprh.html

PHP:  curl_multi_init() 系列
来源：http://hz.cdnleiting.top/gtyowrbmxe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtcidvwikb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtwpsfmvfh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigfzy.top/gtwjshotnq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hysaishi.cn/gtpovhkcpe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shangyingyoupin.top/gtpvogtbgm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xylfe.cn/gtzpkqvhln.html

================================================================================
来源：http://hz.xylfe.cn/gtxxpfffwc.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgufenzy.top/gtsccbfhoi.html

================================================================================
来源：http://hz.andypj.xyz/gtkbeutueo.html

[M01] 读取命令行参数
来源：http://hz.jqgfzy.top/gtlclhfugi.html

Py:   sys.argv[1:]
来源：http://hz.kuanghao11.cn/gtwmuazrqq.html

PHP:  $argv;  $argc;
来源：http://hz.gotoacloud.top/gtfadfaqna.html

JS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gtchavwhad.html

TS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtoirwwpte.html

Java: args 数组（main 方法参数）
来源：http://hz.hnqzz.top/gtyohhhrzm.html

Go:   os.Args[1:]
来源：http://hz.yongpay.top/gtyijtyvhb.html

Ruby: ARGV
来源：http://hz.jyoumei.cn/gtzuhciumk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pycfn.com/gthixxnkpn.html

[M02] 读取环境变量
来源：http://hz.jlsjyb.cn/gtpmbfebyo.html

Py:   os.environ.get("HOME")
来源：http://hz.pengpengdd.cyou/gtsgccjmju.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daxiang520.top/gtdotkaagf.html

JS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtlwcfaqke.html

TS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gttdozeasz.html

Java: System.getenv("HOME")
来源：http://hz.ydzc1.top/gtyzgvhbgk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daria6918.cn/gtdbfrlfpi.html

Ruby: ENV["HOME"]
来源：http://hz.jqgufenzy.top/gtfkmhudkr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.c1oappe.top/gtlyfwdjuh.html

[M03] 执行外部命令
来源：http://hz.jyoumei.cn/gteacgwfjn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgfzy.top/gtetvlbmey.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xinyue.icu/gtwnngypah.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gtilklouma.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fengsongda.top/gtwalvdwiw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hfpthk.cn/gteblqfglc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tanke756.top/gtmmvdylzk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.c1oappe.top/gtezvxzqah.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hywenlv.cn/gtftphnnfs.html

[M04] 获取当前工作目录
来源：http://hz.jqgufenzy.top/gtywxphlaf.html

Py:   os.getcwd()
来源：http://hz.nwbrower.top/gtrfeiyoqs.html

PHP:  getcwd();
来源：http://hz.iojbl.cn/gtgrfobszq.html

JS:   process.cwd()
来源：http://hz.sysykeji.top/gtsmeqywue.html


<!-- 参考信息 -->