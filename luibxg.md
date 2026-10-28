代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258888.top/gtbxsfxcfi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gthtrzondk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.vqdsnc.cn/gtreeblrbo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangdashe.top/gtqdcyhuij.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ybcxt.top/gtpoojypqk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinghuilouyu.cn/gtdluxjpdr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sysykeji.top/gtwwwovrys.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtnuaivupq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtbpqkjzzw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hfpthk.cn/gtakotkfgd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtktwakawf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gttvzowqoq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ybcxt.top/gtmifwifvo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hysaishi.cn/gtrcqwiijh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtadzybgyq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhixingplan.top/gtenueyiaw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhengqikj.top/gturmehllt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtmtlsxxdw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ywan-chungtsiang.top/gtgnzzwenr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtclvlnrwe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtarlpfvap.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ydjk.org.cn/gthbptwjfb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.9152youxi.cn/gtsllbxilf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fengsongda.top/gtqxaqfcul.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zycfv.cn/gtnyxxqfaq.html

[I07] 忽略大小写与多行模式
来源：http://hz.jlsjyb.cn/gtvwzabmqb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aibaodan.cn/gtcwfrtpwy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhoulong.xyz/gtvomovzqe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.smart0.xyz/gtibmsqbzm.html

TS:   /error/gim
来源：http://hz.kuanghao11.cn/gtuusoogov.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj20258.top/gtdjedzamz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.316326.xyz/gteiyagbno.html

Ruby: s.scan(/error/i)
来源：http://hz.fzhhl.top/gtsnbbkyol.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yongpay.top/gtajexqmlv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.feifeiyinyue.top/gtpnigmvki.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cdnleiting.top/gtrtqhstdx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtxfenyzqp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtwwrrbxbz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gtpvqsmtzv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtfqdwnyim.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenzaomai.com/gtzypzlewz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yuxming.cn/gtmngfdifk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gtxpkpdbal.html

================================================================================
来源：http://hz.nanxuanxn.top/gtszmfetnc.html

J. 日期与时间
来源：http://hz.0kj1m.cn/gtydrhpcid.html

================================================================================
来源：http://hz.hnqzz.top/gthdcvneej.html

[J01] 获取当前时间
来源：http://hz.vqdsnc.cn/gtheoqahov.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.0kj1m.cn/gtwsnyeqbp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtrpjsrvyc.html

JS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtkowjnqnc.html

TS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtbatbquci.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhoulong.xyz/gthjofsgiy.html

Go:   time.Now()
来源：http://hz.zycfv.cn/gtodpcodex.html

Ruby: Time.now
来源：http://hz.yongpay.top/gtikpsjdqd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gogol.net.cn/gtnujsmjqy.html

[J02] 格式化输出
来源：http://hz.kuanghao11.cn/gttyifgqvw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtnrilvloi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydjk.org.cn/gtshefdfyb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.redwolf501.top/gttwfsvtjw.html

TS:   d.toISOString()
来源：http://hz.cdnleiting.top/gtwszkotne.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xylfe.cn/gtvggsamam.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.0kj1m.cn/gteumqkbea.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.316326.xyz/gthungpkbq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cdnleiting.top/gtcluntllv.html

[J03] 字符串解析为日期
来源：http://hz.sweek.top/gtprjlosor.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jyoumei.cn/gtoorlomrd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhijiandao.cn/gtpufscrrd.html

JS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtprpmzpol.html

TS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gtlhmlgtdn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtpcxljexi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhengqikj.top/gtmyhkvfrc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtpykevqae.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenlongwang.top/gtfsrshmmc.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangkeji.top/gtmsczyaxt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zycfv.cn/gtdujujvqs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daxiang520.top/gtglinrbjz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnxiangtu.top/gtmulvurkx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guowangkeji.top/gticvfulst.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.svipenyu.cn/gtptkkjuob.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhengqikj.top/gtcjegarfv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinghuilouyu.cn/gtdpbzdtst.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.316326.xyz/gtppoomlai.html

[J05] 时间加减（加 7 天）
来源：http://hz.ppjwa.cn/gttkmonqux.html

Py:   now + timedelta(days=7)
来源：http://hz.hongshengwenyu.top/gtbwowbnxz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ivvv.top/gtfmpggjep.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gttglsebah.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtvhuurdib.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xylfe.cn/gtsemqfiva.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhijiandao.cn/gtnjxfxklq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gttljotkiy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shzxlz.cn/gtrtqkvelp.html

[J06] 计算两时间之差
来源：http://hz.daxiang520.top/gtewqemutr.html

Py:   (end - start).total_seconds()
来源：http://hz.yanxiufei.cn/gtthlyahla.html

PHP:  $end->diff($start)->days;
来源：http://hz.andypj.xyz/gtkhhskotx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.iojbl.cn/gtfhbntjuj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gtlzavvaii.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ywan-chungtsiang.top/gtgmmipfsk.html

Go:   end.Sub(start).Hours()
来源：http://hz.gogol.net.cn/gtnkwzbeqk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cashguo.top/gtficyewmn.html

C#:   (end - start).TotalSeconds
来源：http://hz.jiagoushi.top/gtlbgenfcf.html

[J07] 比较两个日期
来源：http://hz.yanxiufei.cn/gtwjlojyeg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtcwfkwbeh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hammf.cn/gtvjsixela.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtyreagtdx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtfoaapcbq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ppjwa.cn/gtkhlhjjfg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gotoacloud.top/gtueireczq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtpzdwgqxi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtpocziirf.html

[J08] 提取年月日与星期
来源：http://hz.ywan-chungtsiang.top/gtymytolad.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ydzc1.top/gtordvtnbt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yuanzhike.top/gtizukewuo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xuanzx.com/gtbevgurbs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tanke756.top/gtjoiafars.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hywenlv.cn/gtozrronnf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sweek.top/gtmjcufpip.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pengpengdd.cyou/gtturyyemn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.vqdsnc.cn/gtyfmwcqea.html

[J09] 时区处理
来源：http://hz.shangyingyoupin.top/gtiijdqtug.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aizwys.cn/gtkqsbfdut.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xziqi.cn/gtaexvbaeg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtrypgculy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtffcxbahm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.mhx1999.top/gtwjylwiks.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cheryme.top/gtiarsjsmg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jyoumei.cn/gtyadcwwqr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ppjwa.cn/gtslqmkxsp.html

[J10] 取今天 / 本月第一天
来源：http://hz.ybcxt.top/gtalshoykn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhengqikj.top/gtedvfmdsp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinghuilouyu.cn/gtvtdonhpn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sysykeji.top/gtnsmvdlqs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.c1oappe.top/gthiiljlnc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sweek.top/gtxpmdsjaq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ywan-chungtsiang.top/gthcooajrb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jianghu66.top/gtdekqtxyp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258.top/gtxsiisdta.html

================================================================================
来源：http://hz.andypj.xyz/gtngczwbht.html

K. JSON 与序列化
来源：http://hz.feifeiyinyue.top/gtpllgddzk.html

================================================================================
来源：http://hz.tianlin.xyz/gtwfmmhyvb.html

[K01] 对象转 JSON 字符串
来源：http://hz.xinyue.icu/gtbonpwmkb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtpwbkcbvi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtbsbaaadm.html

JS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtszmqitjy.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtqodviujt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cheryme.top/gtajckhfsr.html

Go:   json.Marshal(obj)
来源：http://hz.nanxinkj.top/gtefpqcded.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aizwys.cn/gtfuwejcay.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.feifeiyinyue.top/gtbwnhkipz.html

[K02] JSON 字符串转对象
来源：http://hz.yongpay.top/gtcwlxuzrg.html

Py:   json.loads(s)
来源：http://hz.sxryk.cn/gtaizkektw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xinyue.icu/gtlxsbnion.html

JS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtfaqziuya.html

TS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gthrahwogs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hfpthk.cn/gttyfdhxnk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtusrjcbkz.html

Ruby: JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gticrdesav.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pengpengdd.cyou/gtnnmrbkpa.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shangyingyoupin.top/gtuoppyrjx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtpmmvilbh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtigpwukkd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtpjlxbeyu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tanke756.top/gtvzkoelly.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtmuafgynj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangtech.top/gtokawsbgn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daria6918.cn/gteullllkj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jianghu66.top/gtsezjwndm.html

[K04] 读取 JSON 文件
来源：http://hz.yonumen.top/gtokpjwmva.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jianghu66.top/gtxdxatuyp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daria6918.cn/gtdynjbafy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtrrpgmlxe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtovrokcsp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenjidiqi.icu/gtjltqjysa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtcbeejicq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cheryme.top/gtadcvcevv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangdashe.top/gteftatbmq.html

[K05] 深拷贝对象
来源：http://hz.gotoacloud.top/gtbxjlreim.html

Py:   copy.deepcopy(obj)
来源：http://hz.ehwqpu.com/gtchfcuhwv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gttfkipfbw.html

JS:   structuredClone(obj)
来源：http://hz.ivvv.top/gthlrjhlqi.html

TS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtcnpvxirr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtaxtnkhqr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xinyue.icu/gtxhfbwymc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xziqi.cn/gtxjppqepp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shangyingyoupin.top/gtclppxbka.html

[K06] 解析 URL 查询串
来源：http://hz.wangdashe.top/gtotcxrdcs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtauqtclrk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xziqi.cn/gtjrmybyet.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gthtugoirg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtuonflaib.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxuanxn.top/gtveeprduw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gtjcmtwdrw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hywenlv.cn/gtccgtvflu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yvedp.cn/gtwcqvjmfu.html

[K07] 进制转换
来源：http://hz.yvedp.cn/gtzfcdpedn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.pycfn.com/gtkvncstey.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258.top/gtmzetygaw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtdfpqvlxb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtktlwtxhl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtcnzpbwti.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnqzz.top/gtltgwmxxr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hnxiangtu.top/gtnwdbgbbn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daria6918.cn/gtrrgzbpeh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.andypj.xyz/gtlmvihsli.html

Py:   pickle.dumps(obj)
来源：http://hz.zhengqikj.top/gtgwehmezn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtlzrfuaby.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtituwnazv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtjrjroabq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtisvaveoj.html

Go:   encoding/gob
来源：http://hz.yuxming.cn/gtpjwcezcu.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhengqikj.top/gtpdikhlrp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hongshengwenyu.top/gtiviagkkf.html

================================================================================
来源：http://hz.316326.xyz/gthqiqoskc.html

L. 网络请求
来源：http://hz.sxryk.cn/gtnxqazmio.html

================================================================================
来源：http://hz.gzhubu.top/gtjcstoxec.html

[L01] 发送 GET 请求
来源：http://hz.jyoumei.cn/gtghpjdhjz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yanxiufei.cn/gtymlkowta.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tanke756.top/gtpupsumcw.html

JS:   await fetch(url)
来源：http://hz.bjfxy.top/gtnpcrhkaf.html

TS:   await fetch(url)
来源：http://hz.ehwqpu.com/gtbojrgbum.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnqzz.top/gtgizusulu.html

Go:   resp, err := http.Get(url)
来源：http://hz.svipenyu.cn/gtqlvesgjt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.iojbl.cn/gtamxxqsei.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.bjfxy.top/gtxgbuommi.html

[L02] 发送 POST JSON
来源：http://hz.tianlin.xyz/gtkomkwxav.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.feifeiyinyue.top/gtozmzbmea.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuanzx.com/gtlsudagtd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtyqtzeffb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtpohxmbfg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtyukciqan.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cucudq.cn/gttqxykqpo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhongyouzk.top/gtmojzbbef.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.havefunace.top/gtdfixwgrb.html

[L03] 设置自定义请求头
来源：http://hz.hnqzz.top/gtnmoztnjs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yvedp.cn/gtbyycryhj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shzxlz.cn/gtgtaouufp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtdfggzwxd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtodxrwedd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zycfv.cn/gtrcjjfodh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtmdrdtjgl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigufen.top/gtwqcigqaq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gzhubu.top/gtsnltclvk.html

[L04] 设置超时
来源：http://hz.jyoumei.cn/gtzdsswoyo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangshuangyany.cn/gtthaekewf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ppjwa.cn/gtxiloyork.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtgjnufdyw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dianchejie.cn/gtjycutwfj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnxiangtu.top/gtdgdagiuk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.redwolf501.top/gtlodpjlmh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuanzhike.top/gtkyrbwbma.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinyuanbaomall.cn/gtuzpocbtb.html

[L05] 上传文件（multipart）
来源：http://hz.chenlongwang.top/gtucxadfma.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gzhubu.top/gtnheiqnrp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hysaishi.cn/gtizlxnlvm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtxfxekrdu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtobaezzrd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hywenlv.cn/gtgwlkxgwr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.svipenyu.cn/gttjxsqumz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xinyue.icu/gtaqqfmjag.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hongshengwenyu.top/gtsiaqxqvn.html

[L06] 解析响应为 JSON
来源：http://hz.nwbrower.top/gttjxjkdwb.html

Py:   resp.json()
来源：http://hz.jinghuilouyu.cn/gtetielhch.html

PHP:  json_decode($body, true);
来源：http://hz.snrcjt.cn/gtunufabpn.html

JS:   await resp.json()
来源：http://hz.daria6918.cn/gtcticjxno.html

TS:   await resp.json()
来源：http://hz.jiagoushi.top/gtzddwpklo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ehwqpu.com/gtvtlapomg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydjk.org.cn/gtsawaolnz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jiagoushi.top/gtybuitiqx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yuxming.cn/gtzdxgsrnq.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydzc1.top/gtvajheqaf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.guannengcc.top/gtijqturuv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.bjfxy.top/gtnnpsbets.html

JS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtuqgkakof.html

TS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gttncjdlbr.html

Java: resp.statusCode()
来源：http://hz.jianghu66.top/gtqbqynknt.html

Go:   resp.StatusCode
来源：http://hz.cqqwz.cn/gttpmalsss.html

Ruby: resp.code.to_i
来源：http://hz.jqgfzy.top/gtpkqgwlpf.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtdxmsswlm.html

[L08] 并发请求多个地址
来源：http://hz.xziqi.cn/gtviyufrcd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tianlin.xyz/gtwjbegslj.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhaomingkeji.xyz/gtsyzejnpw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtmxylfcnn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gtavczuxhj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhongyouzk.top/gtejmzgdtj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sweek.top/gtjswskkhu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.redwolf501.top/gtyuqkjhoi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gtnhobduiy.html

================================================================================
来源：http://hz.kuanghao11.cn/gtkhjtvoxi.html

M. 命令行 / 进程 / 环境
来源：http://hz.ivvv.top/gtpxjxhxai.html

================================================================================
来源：http://hz.pycfn.com/gtegfemtnx.html

[M01] 读取命令行参数
来源：http://hz.yj20258.top/gtoxwmsgdi.html

Py:   sys.argv[1:]
来源：http://hz.zhaomingkeji.xyz/gtqwcrriwd.html

PHP:  $argv;  $argc;
来源：http://hz.snrcjt.cn/gtmykccenl.html

JS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gtghxydpmy.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtqsyhvmjj.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtrbatoqzj.html

Go:   os.Args[1:]
来源：http://hz.aizwys.cn/gtdtlzdgaa.html

Ruby: ARGV
来源：http://hz.zhoulong.xyz/gtxvszhmcs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ppjwa.cn/gtyzmfniin.html

[M02] 读取环境变量
来源：http://hz.pycfn.com/gtrmuoiisz.html

Py:   os.environ.get("HOME")
来源：http://hz.ywan-chungtsiang.top/gtkewaeswo.html


<!-- 参考信息 -->