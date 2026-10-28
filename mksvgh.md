代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhiwuduotai.top/gthebxrztu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ybcxt.top/gtwyslsjpj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj20258888.top/gtmigwihfb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangtech.top/gthkdhtakr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gogol.net.cn/gtxquvabuj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xingfuxueyuan.xyz/gtaexfcomv.html

[I04] 正则替换
来源：http://hz.tian-w.cn/gttccwbiyg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.feifeiyinyue.top/gtcyuxkadw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.mhx1999.top/gtrrjnkqks.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ivvv.top/gtphzgivgl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sysykeji.top/gtpnrgsxvi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jianghu66.top/gtqopogzje.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenjidiqi.icu/gtyzgzojkq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daria6918.cn/gtdchbsdjy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dashuyun.cn/gtxgaglmmv.html

[I05] 按正则拆分
来源：http://hz.dianchejie.cn/gtoolcexil.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yueranfly.top/gtrxtongsz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cqqwz.cn/gtnynrwkmj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtkrigjazp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtkiryteln.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yueranfly.top/gtucryfodf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.birdmap.top/gtzngyqvrf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtagecddkj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gaohongyu789.top/gtufuornen.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ehwqpu.com/gthyufzkee.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtoxscxlaj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtgynqhuxu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtqnjazfmc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtixlthgmt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xylfe.cn/gtqdryejsm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.dashuyun.cn/gtnxgevnbu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.quarkkingdee.top/gtoagvsqwn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtazheyuav.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnqzz.top/gtqpkbxxna.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.kuanghao11.cn/gtlxhoqikp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zycfv.cn/gtovndckct.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuxming.cn/gtdfuiwdst.html

TS:   /error/gim
来源：http://hz.cqqwz.cn/gtwxktsatb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.svipenyu.cn/gtprjfptvx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gtphjygnxa.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxinkj.top/gtknwcrauf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydjk.org.cn/gtxekhfzgb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.mhx1999.top/gtjikgyivv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.dianchejie.cn/gtiachitgm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tanke756.top/gtjrchjpus.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtzvdiaqkl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9152youxi.cn/gtrupoivvy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtyuecuwzz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xziqi.cn/gtatkbkufs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.feifeiyinyue.top/gthkcjloro.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.havefunace.top/gthuxmtwvv.html

================================================================================
来源：http://hz.fzhhl.top/gtgsckccap.html

J. 日期与时间
来源：http://hz.zhaomingkeji.xyz/gtaqqwzaxi.html

================================================================================
来源：http://hz.sufxvd.cn/gtukgnfanq.html

[J01] 获取当前时间
来源：http://hz.pycfn.com/gtwerxbocm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jqgfzy.top/gtyjizkgje.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gtstdnwimx.html

JS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtptlogsly.html

TS:   new Date();  Date.now()
来源：http://hz.zhaomingkeji.xyz/gtgfeafraa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yuanzhike.top/gtyoxquvfu.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtzwlmjxmn.html

Ruby: Time.now
来源：http://hz.gotoacloud.top/gtibelggji.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ivvv.top/gthkjdsamz.html

[J02] 格式化输出
来源：http://hz.wangshuangyany.cn/gthvthwuli.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtuuzpmlzs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gthaohnueu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.vqdsnc.cn/gtorysjcrb.html

TS:   d.toISOString()
来源：http://hz.yj20258.top/gtsrwredhf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ehwqpu.com/gtefufnaqx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj202588.top/gtsmukilbl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtjnwpmirw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ehwqpu.com/gttohmsksh.html

[J03] 字符串解析为日期
来源：http://hz.0kj1m.cn/gtmpxruxci.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cheryme.top/gtsxeooqiu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.iojbl.cn/gtyugforyw.html

JS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtkmrsquer.html

TS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtitogchua.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtatrqaqfr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.svipenyu.cn/gtpiovoqmp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.quarkkingdee.top/gtkojfurpv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zdqjudy.top/gtevfxijlf.html

[J04] 时间戳与日期互转
来源：http://hz.daria6918.cn/gtfdjlvxkn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.9152youxi.cn/gtokzcysfu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ybcxt.top/gtqvahytcx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhongyouzk.top/gttxerbtaa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tanke756.top/gtbtvfhwhx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pengpengdd.cyou/gttvbahakd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xylfe.cn/gtlkrtgjay.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pycfn.com/gthtcooald.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hfpthk.cn/gtbfpsbrrq.html

[J05] 时间加减（加 7 天）
来源：http://hz.yangfankeji.com/gtcwougwqm.html

Py:   now + timedelta(days=7)
来源：http://hz.c1oappe.top/gtmhvepxvx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtscpoziyk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtkobcbiki.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yongpay.top/gtjtuhtvpn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtgxmcyuon.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hongshengwenyu.top/gtwhrmcspk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuxming.cn/gtunmohkfl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pycfn.com/gtrvzjeksr.html

[J06] 计算两时间之差
来源：http://hz.jianghu66.top/gtxpieikmy.html

Py:   (end - start).total_seconds()
来源：http://hz.zdqjudy.top/gtjwdbfhkj.html

PHP:  $end->diff($start)->days;
来源：http://hz.cqqwz.cn/gthxujgnwg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guowangkeji.top/gtscetfjft.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xinyue.icu/gtvnzuhiyz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinqigfzy.top/gtrimuswdc.html

Go:   end.Sub(start).Hours()
来源：http://hz.andypj.xyz/gtbojkmcgv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jlsjyb.cn/gtublxiydb.html

C#:   (end - start).TotalSeconds
来源：http://hz.ivvv.top/gtwdgzrjib.html

[J07] 比较两个日期
来源：http://hz.nwbrower.top/gtzaltbpwe.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtfslgjnzk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.svipenyu.cn/gtsxjejepg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgfzy.top/gthcatmfno.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gticcowpkr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jianghu66.top/gtczpjhjdc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.iojbl.cn/gtopidikfg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtlhgxsxlb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtrjwryefx.html

[J08] 提取年月日与星期
来源：http://hz.yuxming.cn/gtzdvhkojl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yongpay.top/gtpxhljpyu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fengsongda.top/gtlynerirm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jlsjyb.cn/gtjofndaiw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.fengsongda.top/gticpweifi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pycfn.com/gtzagskhqq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.0kj1m.cn/gtxaakmvhr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fzhhl.top/gtkzyzwyid.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj202588.top/gtrwugrxcq.html

[J09] 时区处理
来源：http://hz.hywenlv.cn/gtzonnwuqb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cashguo.top/gtvdpnmqlc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hnxiangtu.top/gtpevmuugo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gtuetgpjfh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtokejkvvj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtriilpazj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinyuanbaomall.cn/gttngzfuye.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.smart0.xyz/gtwclzirls.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigufen.top/gtckssqslc.html

[J10] 取今天 / 本月第一天
来源：http://hz.vqdsnc.cn/gtuuojqncj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtyzfvdjrh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinghuilouyu.cn/gtzmpcmgoy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ydjk.org.cn/gtvhvhwzgm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtgkgrpwxw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.vqdsnc.cn/gtvfuaaaez.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ivvv.top/gtjwazlkwj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jiagoushi.top/gtsjdmyfjd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.quarkkingdee.top/gtidnbwhrt.html

================================================================================
来源：http://hz.yueranfly.top/gtixaukcfv.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtuascxdsc.html

================================================================================
来源：http://hz.cheryme.top/gtgncvurvm.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtztqjjiyc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtajraimns.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtvoyxcltl.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangtech.top/gtrtzdoupv.html

TS:   JSON.stringify(obj)
来源：http://hz.xylfe.cn/gtanefhnnl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jqgfzy.top/gtjemgadwj.html

Go:   json.Marshal(obj)
来源：http://hz.gzhubu.top/gteixgvzlh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cdnleiting.top/gtiqcmynro.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xingfuxueyuan.xyz/gtqmtcetft.html

[K02] JSON 字符串转对象
来源：http://hz.ydjk.org.cn/gtiryzktxv.html

Py:   json.loads(s)
来源：http://hz.wangshuangyany.cn/gtgvgnudsl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ivvv.top/gtbmjjvsyx.html

JS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtvialefaf.html

TS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtlmujyqeh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydjk.org.cn/gtrewvilkv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtasnepeum.html

Ruby: JSON.parse(s)
来源：http://hz.havefunace.top/gtikseuwhl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aizwys.cn/gtvxwdkmat.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fengsongda.top/gtikqckpvm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtbisxjxzj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gthdmgcdhd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gthkfcgqun.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtqxpptsxq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenjidiqi.icu/gtzcztfqin.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gzhubu.top/gtuuvmtyrj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.pycfn.com/gtiihxbixt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.0kj1m.cn/gtmuzjupey.html

[K04] 读取 JSON 文件
来源：http://hz.cucudq.cn/gtdrzueihf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxinkj.top/gtxqyixrsv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxinkj.top/gtznyjeija.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtsciqdyxd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtsuwjvoff.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pycfn.com/gtwaqqwjrn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtvgotrxzg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtdynpdmnr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tian-w.cn/gtwvxajppe.html

[K05] 深拷贝对象
来源：http://hz.ehwqpu.com/gtlfmigppw.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhaomingkeji.xyz/gtawzfaneo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gtdydjxryl.html

JS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtlsmfbmqr.html

TS:   structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtdrxvouwq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.haohaochexian.top/gttqchvyjc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daria6918.cn/gtqatekcdq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258888.top/gtnljijnxx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dianchejie.cn/gtgcquntzj.html

[K06] 解析 URL 查询串
来源：http://hz.guannengcc.top/gtpoietvks.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtstzcyxuj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuanzx.com/gtegogqnnv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtvlonhlwu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtuozwbshj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gzhubu.top/gtqqqrytqm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yonumen.top/gtrgugvnaw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cucudq.cn/gtrzgynrhl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtdbtfqxuz.html

[K07] 进制转换
来源：http://hz.hongshengwenyu.top/gtebvzgfgf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jiagoushi.top/gtdrsubswm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gzhubu.top/gtiqpzgtbq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtothjdcgu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtfysjavbv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtvjqjexwu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.haohaochexian.top/gtrcsrqlhq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxinkj.top/gtedxpwfwb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gogol.net.cn/gtkwmhiupr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cashguo.top/gtesxsjcmv.html

Py:   pickle.dumps(obj)
来源：http://hz.xinyue.icu/gtxflgzlgr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.birdmap.top/gtaxbuwaaw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xziqi.cn/gtqtnqqgfq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtkisozyod.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daria6918.cn/gtdpddmnjy.html

Go:   encoding/gob
来源：http://hz.316326.xyz/gtbtutnhde.html

Ruby: Marshal.dump(obj)
来源：http://hz.c1oappe.top/gtqkkunooq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuanzhike.top/gtnlrmnfwk.html

================================================================================
来源：http://hz.52xcode.cn/gtvbosyinl.html

L. 网络请求
来源：http://hz.ivvv.top/gtbkcgblnk.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfmkbliee.html

[L01] 发送 GET 请求
来源：http://hz.316326.xyz/gtqoxokbax.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yvedp.cn/gtzkwyflsq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daria6918.cn/gtoanpqmqv.html

JS:   await fetch(url)
来源：http://hz.kuanghao11.cn/gtkjvvncni.html

TS:   await fetch(url)
来源：http://hz.guannengcc.top/gtvtteymtm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhixingplan.top/gtagbsulzl.html

Go:   resp, err := http.Get(url)
来源：http://hz.kuanghao11.cn/gtpvhhaoqe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.quarkkingdee.top/gtvobnjdve.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xylfe.cn/gtcwxtvlyf.html

[L02] 发送 POST JSON
来源：http://hz.316326.xyz/gtpizzomal.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gogol.net.cn/gtkcyqegri.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.haohaochexian.top/gthzftqsek.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtmniycyki.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtgxkrlwdg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gtfcdzwbsz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.bjfxy.top/gtitgxttji.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yueranfly.top/gtwumfvgtk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cqqwz.cn/gtnkdqwsci.html

[L03] 设置自定义请求头
来源：http://hz.zhongyouzk.top/gtswdmjinf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zdqjudy.top/gtobgqoflf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fengsongda.top/gtsixcluhr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xingfuxueyuan.xyz/gtolircopn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtoibwowdk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daria6918.cn/gtgxcpdllf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtqeexwuij.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yonumen.top/gtsfqrybyt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xylfe.cn/gtpdwydbpy.html

[L04] 设置超时
来源：http://hz.0kj1m.cn/gtwtaueztc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gtyqpkxxtf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jiagoushi.top/gtgazmattk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtukkhoegb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtwmzswxcw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhengqikj.top/gthpndbunf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yangfankeji.com/gtnlykumag.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtwyqfcmht.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtjofxiwmq.html

[L05] 上传文件（multipart）
来源：http://hz.tanke756.top/gtznlyfynq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.bjfxy.top/gtxnhmcvxr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shangyingyoupin.top/gtgyuaonih.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gtruciqzuk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtrcjumdkd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydjk.org.cn/gtuaveigbm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guowangkeji.top/gtvzrhamxg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fzhhl.top/gtbofmjzns.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangtech.top/gtkknwisdt.html

[L06] 解析响应为 JSON
来源：http://hz.kuanghao11.cn/gtmgoqvybj.html

Py:   resp.json()
来源：http://hz.meibo888.top/gtqfssfcgn.html

PHP:  json_decode($body, true);
来源：http://hz.xylfe.cn/gtnohlohbp.html

JS:   await resp.json()
来源：http://hz.yongpay.top/gtuynopvbu.html

TS:   await resp.json()
来源：http://hz.tanke756.top/gtcpggmihj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtedppdlvz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigufen.top/gtvmhycqqp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sufxvd.cn/gtchchnuih.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenjidiqi.icu/gthxoqthue.html

[L07] 处理 HTTP 状态码
来源：http://hz.aizwys.cn/gtklgzltxx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.9152youxi.cn/gtpwnlnjwl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj202588.top/gtfeequauf.html

JS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtcgjwyakk.html

TS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtznpincmq.html

Java: resp.statusCode()
来源：http://hz.cheryme.top/gtsxmszqwj.html

Go:   resp.StatusCode
来源：http://hz.316326.xyz/gtobcgvqmn.html

Ruby: resp.code.to_i
来源：http://hz.ydjk.org.cn/gtfyonmiag.html

C#:   (int)resp.StatusCode
来源：http://hz.aibaodan.cn/gtdjrhdflg.html

[L08] 并发请求多个地址
来源：http://hz.redwolf501.top/gtjeejrpjs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ehwqpu.com/gtmkvmbonn.html

PHP:  curl_multi_init() 系列
来源：http://hz.meibo888.top/gtlnpzywaz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtrmbtxend.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gteadrrvbr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.feifeiyinyue.top/gtcarvcriv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shzxlz.cn/gtfvmdxakm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cqqwz.cn/gtahbqptap.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cheryme.top/gthbtuvyhl.html

================================================================================
来源：http://hz.jlsjyb.cn/gtujfocltd.html

M. 命令行 / 进程 / 环境
来源：http://hz.birdmap.top/gtmlgloher.html

================================================================================
来源：http://hz.cdnleiting.top/gtrrukxiia.html

[M01] 读取命令行参数
来源：http://hz.ydzc1.top/gtdikkbhtz.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gtwazhgnon.html

PHP:  $argv;  $argc;
来源：http://hz.hnxiangtu.top/gtpbpjicxv.html


<!-- 参考信息 -->