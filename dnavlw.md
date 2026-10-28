代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hz.chenjidiqi.icu/gtzoryokez.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.feifeiyinyue.top/gttdhluhqv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guannengcc.top/gttexsyzjj.html

Ruby: s.scan(/\d+/)
来源：http://hz.yuxming.cn/gtqsbmxpqi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cucudq.cn/gtrcsgcnrm.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangkeji.top/gtqexxdmwn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shangyingyoupin.top/gtzjbhgwnz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gotoacloud.top/gtmfcbzzuu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yongpay.top/gtcdalpodf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tanke756.top/gtrhpdqwqf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gaohongyu789.top/gtlnceyhdb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cucudq.cn/gtsowgdwrz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydzc1.top/gtanslyzby.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.feifeiyinyue.top/gtmwxlhhfi.html

[I04] 正则替换
来源：http://hz.guannengcc.top/gtmxvzuigg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yvedp.cn/gtenzvokji.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtkopypqev.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zdqjudy.top/gtcvabewae.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ivvv.top/gtshlttgvn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zycfv.cn/gteafpqwpp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxuanxn.top/gthpbrhnzh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pycfn.com/gtiodubzyz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.quarkkingdee.top/gtqgeaxtyy.html

[I05] 按正则拆分
来源：http://hz.kuanghao11.cn/gtrnoarglu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jyoumei.cn/gtpcontuuu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.aibaodan.cn/gtbtgoffkc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtadxvsxdl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtomifjufw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hywenlv.cn/gtowditafo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhiwuduotai.top/gtbbyaerfd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtyckuvqsp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yonumen.top/gtpshamchq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gtycvdpxep.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gttsyuyqqj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhongyouzk.top/gtphusmizf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtkgeudbma.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtuppityzu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtpzhkvdkh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinyuanbaomall.cn/gtcwmywvcz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnqzz.top/gthtybjpau.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ehwqpu.com/gtzvfvhzzw.html

[I07] 忽略大小写与多行模式
来源：http://hz.hongshengwenyu.top/gtewvcjtsg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhengqikj.top/gtlzcxcgsi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xylfe.cn/gtkssrykpb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xylfe.cn/gtvpuivysg.html

TS:   /error/gim
来源：http://hz.sweek.top/gtvqmzpnzg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj20258.top/gtichlzpcq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.havefunace.top/gtwbteroba.html

Ruby: s.scan(/error/i)
来源：http://hz.gogol.net.cn/gtvbcxnwer.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.andypj.xyz/gtnluxpufz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pycfn.com/gtxpilfnym.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.redwolf501.top/gtddlsvgno.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cdnleiting.top/gtfydwnjvi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtzbkpaolv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhixingplan.top/gtqnifautv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cqqwz.cn/gtycvpssoq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.pycfn.com/gtzhzzrobx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hywenlv.cn/gtugrgdosq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cashguo.top/gtpxocjvaf.html

================================================================================
来源：http://hz.9152youxi.cn/gtpxlymxuy.html

J. 日期与时间
来源：http://hz.yj20258888.top/gtcvuacboa.html

================================================================================
来源：http://hz.smart0.xyz/gtnddehjyn.html

[J01] 获取当前时间
来源：http://hz.xylfe.cn/gtyuyazhlp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtiulqalgi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.meibo888.top/gtogqlphgh.html

JS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtmlwlyeyt.html

TS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gttfvoruwb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jlsjyb.cn/gtarddbbce.html

Go:   time.Now()
来源：http://hz.zycfv.cn/gtvsufwchl.html

Ruby: Time.now
来源：http://hz.hnqzz.top/gtfctpvfuy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.smart0.xyz/gtlyfqjucr.html

[J02] 格式化输出
来源：http://hz.0kj1m.cn/gtkmjicuib.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtcougbdou.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtykgvgmow.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yongpay.top/gtqsrsursi.html

TS:   d.toISOString()
来源：http://hz.gogol.net.cn/gtgajrfhdu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zycfv.cn/gtktgyaqhl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenjidiqi.icu/gtclgxdinn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtsqeildde.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sxryk.cn/gtlffzyajb.html

[J03] 字符串解析为日期
来源：http://hz.dashuyun.cn/gtfubeixck.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xingfuxueyuan.xyz/gtzbdnvjat.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydzc1.top/gtjlpowonq.html

JS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtjxhspvje.html

TS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtfgkclmfj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtswxfrgxy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gthezfmlrh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtxdrfwank.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gzhubu.top/gtmppxnxca.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtalogrrrr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.316326.xyz/gtuxfakvsd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zycfv.cn/gtlvhndmoe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhaomingkeji.xyz/gtndsluarv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydzc1.top/gtbkqmuzxv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangkeji.top/gthpprisel.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigfzy.top/gtjqwwprey.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xingfuxueyuan.xyz/gtommpxkrg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.smart0.xyz/gtdmityvss.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhongyouzk.top/gtjkysfaen.html

Py:   now + timedelta(days=7)
来源：http://hz.xziqi.cn/gtrzhuyasf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhoulong.xyz/gtlgmrkjrj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtuygwaiso.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aizwys.cn/gtzyrlvxwa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258888.top/gtdavhdgaa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jiagoushi.top/gtffcvavpe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xingfuxueyuan.xyz/gtzmjmncgg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cdnleiting.top/gttnfihpoq.html

[J06] 计算两时间之差
来源：http://hz.gotoacloud.top/gtascbfmfp.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgfzy.top/gtfwxwrptc.html

PHP:  $end->diff($start)->days;
来源：http://hz.shuidangran.top/gtypmfoihx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yonumen.top/gtsuwyhrgj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yanxiufei.cn/gteccgdwzl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.bjfxy.top/gtttqdgljy.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtftglizqb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.andypj.xyz/gtiamlexyb.html

C#:   (end - start).TotalSeconds
来源：http://hz.sufxvd.cn/gtndednuqz.html

[J07] 比较两个日期
来源：http://hz.jianghu66.top/gtufgmfgle.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtrelufelj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sysykeji.top/gtyzsjidas.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtehnsquda.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtgcwocmhm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hammf.cn/gtzyvefbel.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hysaishi.cn/gtuexxxqqb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtleapkwgc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtgsfolmfc.html

[J08] 提取年月日与星期
来源：http://hz.yj20258.top/gtaclukozk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.9152youxi.cn/gtilvuxwon.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dianchejie.cn/gtiootdobv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.9152youxi.cn/gtsneoqygu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxinkj.top/gtyzojjipg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fzhhl.top/gtuzmunkfs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shzxlz.cn/gtxvnbssqu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yonumen.top/gtsorxyjnk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gtbqjryprh.html

[J09] 时区处理
来源：http://hz.daxiang520.top/gttfgmprwp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gogol.net.cn/gtjjmhyqba.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ywan-chungtsiang.top/gtinfwesid.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtstuoqwlm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtvqlaywav.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jyoumei.cn/gtvtkyuqty.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtqsiaughy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gaohongyu789.top/gthchkhjml.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xziqi.cn/gtkmykkuue.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhiwuduotai.top/gtlkxbjznl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hongshengwenyu.top/gttjjyiyim.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangdashe.top/gtjnfrfakb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yvedp.cn/gteevpoksl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ehwqpu.com/gtkitlnogq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pycfn.com/gtazsccjwp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuxming.cn/gticlpkpgo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tian-w.cn/gtlzthbzzx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yongpay.top/gtmiwxxgft.html

================================================================================
来源：http://hz.vqdsnc.cn/gtshholodq.html

K. JSON 与序列化
来源：http://hz.yangfankeji.com/gthoxjbsxg.html

================================================================================
来源：http://hz.andypj.xyz/gtvmmcsllp.html

[K01] 对象转 JSON 字符串
来源：http://hz.sxryk.cn/gtlvyhulvq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gthgnrzwwf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtzozgrycb.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtqrvqtwfb.html

TS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtpaouesec.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.0kj1m.cn/gtmgvbjequ.html

Go:   json.Marshal(obj)
来源：http://hz.hongshengwenyu.top/gtjklzswxm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hammf.cn/gtrtlexphx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangtech.top/gtbwxmbsdq.html

[K02] JSON 字符串转对象
来源：http://hz.hysaishi.cn/gtlkpzgcxg.html

Py:   json.loads(s)
来源：http://hz.zhiwuduotai.top/gtupgedkgi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtwdzbdyqo.html

JS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtcmbiyxkn.html

TS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtqzuunhbw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pengpengdd.cyou/gtztotmern.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtiwagsxqh.html

Ruby: JSON.parse(s)
来源：http://hz.mhx1999.top/gtooizuebu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gaohongyu789.top/gtexfdtcvp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gtntbllouk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pycfn.com/gtifvxndhc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gthumyvvfb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gthvkiumiw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhaomingkeji.xyz/gtjndcvnlh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.meibo888.top/gtouygwwzo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yangfankeji.com/gtwwlvssrd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hfpthk.cn/gtrheumhuf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gzhubu.top/gtxfomxbpz.html

[K04] 读取 JSON 文件
来源：http://hz.nwbrower.top/gtuntlcgag.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangkeji.top/gtjxagztxo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yangfankeji.com/gtzlxadtpp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangdashe.top/gtzcegvjwt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gttcteiprc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xylfe.cn/gtdgnpcozr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtibredlkc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hysaishi.cn/gttlqxmtsy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.snrcjt.cn/gtajqhdcld.html

[K05] 深拷贝对象
来源：http://hz.gaohongyu789.top/gtmsojydql.html

Py:   copy.deepcopy(obj)
来源：http://hz.cdnleiting.top/gtmcozvnle.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhaomingkeji.xyz/gtsimxcjmr.html

JS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtkqhpsyvn.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtauiyablk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jyoumei.cn/gtxcaqldrm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ybcxt.top/gttwyrupmu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fzhhl.top/gthosykqjo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenlongwang.top/gtgondgucg.html

[K06] 解析 URL 查询串
来源：http://hz.ywan-chungtsiang.top/gtkyzuiyhy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.redwolf501.top/gthmqapdns.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinyuanbaomall.cn/gtvlhuvcpx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtuwjozovh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtvpnwjwxn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.redwolf501.top/gtgdvezvwp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yongpay.top/gtbartksud.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fengsongda.top/gthqrnoigy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hnqzz.top/gtmpkbcfdh.html

[K07] 进制转换
来源：http://hz.52xcode.cn/gtgvcblcdm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.havefunace.top/gtbbufolfq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zycfv.cn/gtkpzzzwha.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtrjhsswxk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtlnaralpn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gtjvxmtbkv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gttnfnseyv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fzhhl.top/gttlawztgi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hongshengwenyu.top/gtyeqijyok.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aizwys.cn/gtebpyiirz.html

Py:   pickle.dumps(obj)
来源：http://hz.hfpthk.cn/gtbvncnibw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.0kj1m.cn/gtquormnem.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sufxvd.cn/gtyphdteas.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtxilmpudc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sysykeji.top/gtrfhrdocf.html

Go:   encoding/gob
来源：http://hz.guowangkeji.top/gtcmsdufld.html

Ruby: Marshal.dump(obj)
来源：http://hz.svipenyu.cn/gtskpoxcqe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aizwys.cn/gttuwylypu.html

================================================================================
来源：http://hz.mhx1999.top/gtnsujectg.html

L. 网络请求
来源：http://hz.zhengqikj.top/gtuheuatux.html

================================================================================
来源：http://hz.sufxvd.cn/gtkayrxohs.html

[L01] 发送 GET 请求
来源：http://hz.yonumen.top/gtazvhvtxz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.mhx1999.top/gtfacusnvv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtgzbhbklx.html

JS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtoosmehqg.html

TS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtshbbvjgu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gotoacloud.top/gtjxpppnne.html

Go:   resp, err := http.Get(url)
来源：http://hz.xuanzx.com/gtyhobtrfd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dashuyun.cn/gtekhzhfjh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cheryme.top/gtfgdkamkg.html

[L02] 发送 POST JSON
来源：http://hz.chenlongwang.top/gtvotxhujn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ywan-chungtsiang.top/gtkfaocfka.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cheryme.top/gtvazvfquc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.52xcode.cn/gtiforskkz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtoxheldxp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhongyouzk.top/gtgbmwzfdk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guannengcc.top/gtcsptswpo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.aibaodan.cn/gtnzknidbe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.316326.xyz/gtjscgmkjr.html

[L03] 设置自定义请求头
来源：http://hz.ivvv.top/gtbohbbzzh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cheryme.top/gtdhslksss.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shangyingyoupin.top/gtipwwdbcl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gtczqwdttm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtgkbmrvjk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.bjfxy.top/gtinipipqy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.smart0.xyz/gtshpjfqhq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhengqikj.top/gtekhtbkbl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yongpay.top/gtayvmnnnm.html

[L04] 设置超时
来源：http://hz.cheryme.top/gtomacshud.html

Py:   requests.get(url, timeout=5)
来源：http://hz.feifeiyinyue.top/gtkxtfadst.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.dashuyun.cn/gtgheosdws.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtdtonaetp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gtlhqxyybo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tanke756.top/gturmrlcgg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.havefunace.top/gthyshttax.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.vqdsnc.cn/gtpxdkcytx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.haohaochexian.top/gtdogchjeg.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtdtewhhae.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtkgipihku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guannengcc.top/gtjbuiksfl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gteynocuwa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gtlpuafais.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhixingplan.top/gtnbobmpfi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yonumen.top/gtcrvolulk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shangyingyoupin.top/gtclqzwfaq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.birdmap.top/gtmvfbolid.html

[L06] 解析响应为 JSON
来源：http://hz.52xcode.cn/gtuglxrlll.html

Py:   resp.json()
来源：http://hz.yj202588.top/gtacdhhtmc.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtpgzbadlt.html

JS:   await resp.json()
来源：http://hz.hnqzz.top/gtttunqwud.html

TS:   await resp.json()
来源：http://hz.yj202588.top/gtutwjqamv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cheryme.top/gtqojhylbs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xylfe.cn/gtmixqtpsw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgufenzy.top/gtiwdfusrw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.52xcode.cn/gtmgzhnbyl.html

[L07] 处理 HTTP 状态码
来源：http://hz.tianlin.xyz/gtkbvvoulp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ehwqpu.com/gtauqfdbdy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.quarkkingdee.top/gtqevlefui.html

JS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtoxyscvgk.html

TS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtnjfvcsty.html

Java: resp.statusCode()
来源：http://hz.shuidangran.top/gttizzblat.html

Go:   resp.StatusCode
来源：http://hz.iojbl.cn/gttmclrtqf.html

Ruby: resp.code.to_i
来源：http://hz.snrcjt.cn/gtrzlhxdoq.html

C#:   (int)resp.StatusCode
来源：http://hz.xziqi.cn/gteruwtoqg.html

[L08] 并发请求多个地址
来源：http://hz.yonumen.top/gtfcsdersk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgfzy.top/gtomuvzffi.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenlongwang.top/gtuzkzwzxn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gthdsbtimv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtkqkqoevs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigufen.top/gtmktzesrz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jianghu66.top/gtmflrsnph.html


<!-- 参考信息 -->