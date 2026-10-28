代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gtvirxctap.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gtjdtlnyca.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gotoacloud.top/gtgkbzqksj.html

[H10] 资源自动释放
来源：http://hz.zhaomingkeji.xyz/gtoaxxuvni.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zdqjudy.top/gtakewmghd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangtech.top/gtfkpvpsmn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtnfwniryp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gthtjduhtu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yangfankeji.com/gtnedohaxz.html

Go:   defer f.Close()
来源：http://hz.yangfankeji.com/gtjwfaudxh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenzaomai.com/gtjnvryajx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangshuangyany.cn/gtdopjtywq.html

================================================================================
来源：http://hz.xziqi.cn/gtefszgjsx.html

I. 正则表达式
来源：http://hz.gogol.net.cn/gtlybhihyj.html

================================================================================
来源：http://hz.jqgfzy.top/gthozwhhjb.html

[I01] 判断是否匹配
来源：http://hz.jqgfzy.top/gtyqgoympn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xziqi.cn/gtqmtxrgez.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ywan-chungtsiang.top/gtjuhpcaiz.html

JS:   /\d+/.test(s)
来源：http://hz.vqdsnc.cn/gtibivcmkq.html

TS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtgqzkgeqc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.daxiang520.top/gtjptabctt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhongyouzk.top/gttsoteucr.html

Ruby: s.match?(/\d+/)
来源：http://hz.c1oappe.top/gtchilljco.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jlsjyb.cn/gtethtrlqu.html

[I02] 提取所有匹配
来源：http://hz.zhaomingkeji.xyz/gtflbprmdr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenlongwang.top/gtujshsahs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sweek.top/gtvicgtdzv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cheryme.top/gtyvqacesn.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgfzy.top/gtzpqqmxqf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gaohongyu789.top/gtoxywqbpf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cashguo.top/gtcarrqkbd.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gtyypvmuvb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cqqwz.cn/gtvmoggbyn.html

[I03] 提取捕获分组
来源：http://hz.0kj1m.cn/gtnuocwdfo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xylfe.cn/gtsqgncqrz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtauxkrlka.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenjidiqi.icu/gtrljiixcy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cashguo.top/gttgjoibac.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgfzy.top/gtnqpwjche.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinqigufen.top/gtrblnuvub.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ywan-chungtsiang.top/gtgfkjcwbv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.c1oappe.top/gtsocslqhc.html

[I04] 正则替换
来源：http://hz.redwolf501.top/gteuriugxj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ywan-chungtsiang.top/gtwshozmjw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gteqljocdo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtsnqygbfr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtcivzhuii.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daria6918.cn/gttqyhfxkz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinqigfzy.top/gtqwiiplgg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ivvv.top/gtcharvvek.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zdqjudy.top/gtgxqgcina.html

[I05] 按正则拆分
来源：http://hz.jlsjyb.cn/gtduwoyebn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dashuyun.cn/gtpibfplwa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ivvv.top/gthixlxkiz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtiiwebmsa.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtjblnhtjn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shangyingyoupin.top/gtemrcacwj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aibaodan.cn/gtrxrdouyy.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtbnxgaybf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gthvxuapcc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.birdmap.top/gtzcmksmjq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtsszefucf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yonumen.top/gtzepjihyn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigfzy.top/gtuibytjic.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtgteevcxn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhongyouzk.top/gtdkybumra.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.meibo888.top/gtsrjdxtip.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cqqwz.cn/gtguwjdfla.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tanke756.top/gtcwqduhau.html

[I07] 忽略大小写与多行模式
来源：http://hz.redwolf501.top/gtokikjqlk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shuidangran.top/gtpbfamtrb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.wangshuangyany.cn/gtyosjtbsp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jlsjyb.cn/gtystjlwnn.html

TS:   /error/gim
来源：http://hz.gogol.net.cn/gtwgtocpgp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yueranfly.top/gtzkagfvju.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fengsongda.top/gtdfutygql.html

Ruby: s.scan(/error/i)
来源：http://hz.zhixingplan.top/gtsirfzfcb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.9152youxi.cn/gtgraqaoye.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xingfuxueyuan.xyz/gtsdqpwfqr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxinkj.top/gteamghryl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gaohongyu789.top/gtglakjqjm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtuheznnwv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guowangkeji.top/gtxifkjymd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ivvv.top/gtnvnltpxx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cheryme.top/gtdxjkledg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.52xcode.cn/gtfmevpkwl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtyqrjqpke.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtfgtbmvyf.html

J. 日期与时间
来源：http://hz.ydjk.org.cn/gtdnjngswx.html

================================================================================
来源：http://hz.mhx1999.top/gtolezvxbf.html

[J01] 获取当前时间
来源：http://hz.chenjidiqi.icu/gtxisdhlpm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.vqdsnc.cn/gtvoghuxfe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gtepfddshi.html

JS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtudnfuziz.html

TS:   new Date();  Date.now()
来源：http://hz.zhoulong.xyz/gtpybywmch.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinyuanbaomall.cn/gtstnmrqam.html

Go:   time.Now()
来源：http://hz.sysykeji.top/gtssomimvb.html

Ruby: Time.now
来源：http://hz.hfpthk.cn/gthrzeepzw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gotoacloud.top/gtsyafjmur.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gtlmrzjbvy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtbzmlypjf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtktylixqw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sysykeji.top/gtmffmqfal.html

TS:   d.toISOString()
来源：http://hz.xuanzx.com/gtwzxiltrk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhaomingkeji.xyz/gtzrdtsxkp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sufxvd.cn/gtkonscmno.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtqoakezjl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtwofhoqxf.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangtech.top/gtkwcbwocv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yongpay.top/gtglwirzdo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yueranfly.top/gtwkagovdq.html

JS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtowsfleyi.html

TS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtstbcweuy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtjamvwrtr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.haohaochexian.top/gtmszxjjln.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hnqzz.top/gtipgxhcgv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuanzhike.top/gttybmiuqd.html

[J04] 时间戳与日期互转
来源：http://hz.hammf.cn/gtyfhwdqvl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.quarkkingdee.top/gtcgqzmamk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.smart0.xyz/gtfmlrivub.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhaomingkeji.xyz/gtczabmvws.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtwniskenx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hfpthk.cn/gtnqlcywri.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aibaodan.cn/gthnattpjn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hongshengwenyu.top/gtljoaunhb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sysykeji.top/gtgspxdasx.html

[J05] 时间加减（加 7 天）
来源：http://hz.ywan-chungtsiang.top/gtegugyptr.html

Py:   now + timedelta(days=7)
来源：http://hz.xuanzx.com/gtgqceymlw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jianghu66.top/gtjjxnsbtx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtsrkexrbb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenjidiqi.icu/gtwcivglxz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xinyue.icu/gtpwjgwlqa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gtunbnuexg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhoulong.xyz/gtmgmkxlza.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgfzy.top/gtgdxfetoj.html

[J06] 计算两时间之差
来源：http://hz.cqqwz.cn/gtmwwnfasw.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangkeji.top/gtrfxnofdd.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtajmxhtag.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.andypj.xyz/gtwxqjrvdl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ppjwa.cn/gtmaahmlra.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aizwys.cn/gtefitmhye.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtvinpcvrj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhongyouzk.top/gtfkpdnrgx.html

C#:   (end - start).TotalSeconds
来源：http://hz.ybcxt.top/gtiyblmttb.html

[J07] 比较两个日期
来源：http://hz.guowangkeji.top/gtwzttefxb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gthbzqvgnq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuanzx.com/gtrffxpwjx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tian-w.cn/gtkegiylzq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xziqi.cn/gtoujynbye.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj202588.top/gtivfbhrvw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daria6918.cn/gtidkzrmzz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtobobhxqb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtbsxtiamv.html

[J08] 提取年月日与星期
来源：http://hz.dianchejie.cn/gtlmzljgii.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yuxming.cn/gtarepvdco.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hywenlv.cn/gtefidwcyt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.meibo888.top/gtsaylsmtv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jianghu66.top/gtljzbrlrk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydzc1.top/gtkagwoiuv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gtomeunuvw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhiwuduotai.top/gtblozdtpe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pengpengdd.cyou/gtctwwtsrn.html

[J09] 时区处理
来源：http://hz.snrcjt.cn/gtpqbdtduh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aizwys.cn/gtopzgzgtx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guannengcc.top/gtjuviuvor.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtmpwfcexl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtlmphdbci.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gotoacloud.top/gtweaqgeft.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuanzx.com/gtzrigaveb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tianlin.xyz/gtvkebhxel.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.andypj.xyz/gtmtzicpel.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgufenzy.top/gtneelfvha.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.pengpengdd.cyou/gttwxxdskk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nwbrower.top/gtwwdgrvpl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yongpay.top/gtineetkrg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xingfuxueyuan.xyz/gtmfmjdgyc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.redwolf501.top/gtbngxgjzj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtccfikvtp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gttblsvvjs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ivvv.top/gtdzfvxnew.html

================================================================================
来源：http://hz.fzhhl.top/gtqlnjfiec.html

K. JSON 与序列化
来源：http://hz.hongshengwenyu.top/gttzzvbrjv.html

================================================================================
来源：http://hz.bjfxy.top/gtxbxsqwzo.html

[K01] 对象转 JSON 字符串
来源：http://hz.birdmap.top/gteumuoyow.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtdqpgawcv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtumqiglfn.html

JS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtryteifsl.html

TS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gtzvanwibk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtjxtfxdxt.html

Go:   json.Marshal(obj)
来源：http://hz.yangfankeji.com/gtbphqedev.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.andypj.xyz/gtmcewxyos.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hfpthk.cn/gtskwqszwu.html

[K02] JSON 字符串转对象
来源：http://hz.fengsongda.top/gttxgywcal.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gtlwjbajfi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.quarkkingdee.top/gtjuoadrlq.html

JS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtguvjaoci.html

TS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtixkihzih.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.vqdsnc.cn/gtydjqwoup.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtmiduyndj.html

Ruby: JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtkhukiqsh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtfcazfply.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jlsjyb.cn/gtpyyykkjy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtdczioobp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtoyhzidmy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtwimxvezc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtqeigsiwi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtwfxzwlhp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.redwolf501.top/gtsawhpdrs.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.iojbl.cn/gtjrhirfks.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhiwuduotai.top/gtyjklavyw.html

[K04] 读取 JSON 文件
来源：http://hz.gogol.net.cn/gtfmmylomn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cheryme.top/gtmrghtjex.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cdnleiting.top/gttnvxtnoz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daxiang520.top/gtnfvcimvj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtrduhtuta.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jiagoushi.top/gtmvbcunqk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gtoyfqgebe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gttteipdjd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ywan-chungtsiang.top/gtjgfkhzvr.html

[K05] 深拷贝对象
来源：http://hz.ydzc1.top/gttmbuszfg.html

Py:   copy.deepcopy(obj)
来源：http://hz.meibo888.top/gtxyohivgl.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xuetiantiany.cn/gtxpgjhazi.html

JS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtucxwvpwm.html

TS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtvwbgfoun.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jyoumei.cn/gtuoyvamoq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinyuanbaomall.cn/gtrzvyhvih.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxuanxn.top/gthahbkflp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtonvgzkzd.html

[K06] 解析 URL 查询串
来源：http://hz.jqgufenzy.top/gtxufzerrx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aibaodan.cn/gtobdvoqsu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.bjfxy.top/gtquktracm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtjnpqqctg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.quarkkingdee.top/gtudjryjvd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ywan-chungtsiang.top/gtsqmcczpn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guannengcc.top/gtubnkellv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258.top/gtapsamvyg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fzhhl.top/gtyylxtwjl.html

[K07] 进制转换
来源：http://hz.jinqigufen.top/gtdjwbsgun.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258.top/gttpdfftrj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinyuanbaomall.cn/gtaekeihdj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtjofhllkh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtmtzymezi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gttsdaowpz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xylfe.cn/gtgdtitwhd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zdqjudy.top/gtcpvlzuau.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.guowangkeji.top/gtoygmsyoc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cucudq.cn/gtcmexwtao.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gtisskwwsl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuetiantiany.cn/gtibshcqtf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gtdconcksb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtjngcvtoc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xylfe.cn/gtkvioeotb.html

Go:   encoding/gob
来源：http://hz.svipenyu.cn/gtrjunrkyl.html

Ruby: Marshal.dump(obj)
来源：http://hz.fengsongda.top/gtyjwulxac.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sufxvd.cn/gtwqdjtfjq.html

================================================================================
来源：http://hz.haohaochexian.top/gtsbubvpud.html

L. 网络请求
来源：http://hz.jqgufenzy.top/gtlibqbifp.html

================================================================================
来源：http://hz.xziqi.cn/gtmhepkrty.html

[L01] 发送 GET 请求
来源：http://hz.iojbl.cn/gtyjbakrxp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.vqdsnc.cn/gtsuaezclf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guowangkeji.top/gtllustvea.html

JS:   await fetch(url)
来源：http://hz.yongpay.top/gtkwxlqqlg.html

TS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtyrqmxgka.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pycfn.com/gtoxilnfzl.html

Go:   resp, err := http.Get(url)
来源：http://hz.feifeiyinyue.top/gtpaqmrsqw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhengqikj.top/gthyclnpuc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daria6918.cn/gttlseucgs.html

[L02] 发送 POST JSON
来源：http://hz.fengsongda.top/gtppvdbwlj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zdqjudy.top/gtmkpvryfh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shanyushiyangkeji.top/gttzeeceoa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtzkzepsbi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtfojyewry.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.wangshuangyany.cn/gtpxuntdyl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dashuyun.cn/gtkrilzact.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.kuanghao11.cn/gtekpstlix.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhiwuduotai.top/gtionsekkm.html

[L03] 设置自定义请求头
来源：http://hz.wangdashe.top/gtgvtllbfq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.wangshuangyany.cn/gtgmnipelm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuanzhike.top/gtaobedqjf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtrracxhzi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtklijhyqb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.dashuyun.cn/gtdgwmfvcc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gthjfdrfwm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hfpthk.cn/gtkmfnpovl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtkdhobsgu.html

[L04] 设置超时
来源：http://hz.0kj1m.cn/gttbjyirof.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sweek.top/gtdhyrjdmy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shanyushiyangtech.top/gtnsejmerf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtyonkvdmw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtyetmwrjl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ybcxt.top/gtfxvrerpa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pycfn.com/gtlfdjzqfl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gtedxhcwif.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ppjwa.cn/gtvjkhecku.html

[L05] 上传文件（multipart）
来源：http://hz.52xcode.cn/gtyfrrmxhv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aizwys.cn/gtbcmrmywo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hywenlv.cn/gtqygwwzbj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtxltdirpl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gthehgrqbd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pengpengdd.cyou/gtlrdabtqk.html


<!-- 参考信息 -->