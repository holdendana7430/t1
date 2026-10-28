代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hz.sysykeji.top/gtjyfieuke.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pengpengdd.cyou/gtukbuvlmg.html

[H09] 带错误码的异常
来源：http://hz.shuidangran.top/gtygxntznp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.quarkkingdee.top/gtjdchsmpl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.svipenyu.cn/gtfcispfqn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zdqjudy.top/gtgjbgbxvt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.bjfxy.top/gtdwmsbhfg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ywan-chungtsiang.top/gtdnefmbpd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cucudq.cn/gtwsycxtwm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shzxlz.cn/gtjssxdfvr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangshuangyany.cn/gtqgxmgapw.html

[H10] 资源自动释放
来源：http://hz.ehwqpu.com/gtcxfdtlah.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.pycfn.com/gtufvydcvr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gtzgyxmqeh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtzktrmbhh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gthxtpkgkz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pengpengdd.cyou/gtqcimhbqu.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gtfbfauirs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sxryk.cn/gtxjbziwsq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuanzhike.top/gtkzazixyb.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtndnezpph.html

I. 正则表达式
来源：http://hz.zhengqikj.top/gtuvrheens.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtmgwklqou.html

[I01] 判断是否匹配
来源：http://hz.jianghu66.top/gtdkmhggbc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgfzy.top/gtdjqgudgb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgfzy.top/gtipnlvoyb.html

JS:   /\d+/.test(s)
来源：http://hz.hywenlv.cn/gtjevhtbej.html

TS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtvaposfii.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.c1oappe.top/gtbnycwxim.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuetiantiany.cn/gtqihliewn.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhijiandao.cn/gtjqlbulqh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinyuanbaomall.cn/gtlqcperic.html

[I02] 提取所有匹配
来源：http://hz.xuanzx.com/gtodyzzbnx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.smart0.xyz/gtsyukchlo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.pycfn.com/gtexxqcxtt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtbpimvgab.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgfzy.top/gtmffhqqog.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guannengcc.top/gtimldlhji.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuetiantiany.cn/gtgldqxzgn.html

Ruby: s.scan(/\d+/)
来源：http://hz.ivvv.top/gtcnqukbho.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gotoacloud.top/gtkntmngqw.html

[I03] 提取捕获分组
来源：http://hz.meibo888.top/gtqxqdsxod.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.havefunace.top/gtgjpsyvaj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.fzhhl.top/gtrxblrkuw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sufxvd.cn/gtaiqdugbw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yvedp.cn/gtqtvxbuic.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.havefunace.top/gtfipdwgtn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258.top/gtapumlklf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhijiandao.cn/gtbpwevmxd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daria6918.cn/gtzuckqdev.html

[I04] 正则替换
来源：http://hz.ydzc1.top/gtgvtzokoe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jlsjyb.cn/gtitvhzatv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cucudq.cn/gtqoyaporo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.c1oappe.top/gtzuejadhd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtxswewnyh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.smart0.xyz/gtgyeisegi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.quarkkingdee.top/gtbwagxqgi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cucudq.cn/gttzkjcxhy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ybcxt.top/gtdnjtjmwt.html

[I05] 按正则拆分
来源：http://hz.haohaochexian.top/gtmvnruxwe.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fzhhl.top/gtsrzoqydy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhengqikj.top/gtjghhjyfd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtzhegtypv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtoququred.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shuidangran.top/gtdnwrbqqv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj20258.top/gtjnkrzyvh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtgiwavrsv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pycfn.com/gtmaoiudwg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hammf.cn/gtqkloehbl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gtxjlpstxm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xingfuxueyuan.xyz/gtbimwugim.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtfeiknwtm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtzpmgsggx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtaxisvdeh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.vqdsnc.cn/gtfozhrwix.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydzc1.top/gtlrgddsqt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.haohaochexian.top/gtasvbxsnv.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtxebzelst.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yueranfly.top/gtuwmsxwjd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258.top/gtriqrnaju.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tanke756.top/gtgicghxng.html

TS:   /error/gim
来源：http://hz.feifeiyinyue.top/gtcwpounde.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.quarkkingdee.top/gtbpzuowxl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fengsongda.top/gtgapvklzp.html

Ruby: s.scan(/error/i)
来源：http://hz.yonumen.top/gtvafqjnms.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gogol.net.cn/gtnufqhnyk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.iojbl.cn/gtlmfqcgnu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yangfankeji.com/gtmcdwpyos.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zycfv.cn/gtdhmwytnr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtsfphpuun.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtptdmnoni.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtidqzlixm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gzhubu.top/gttkkcmvfo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtuqmmbjpe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pycfn.com/gtcpipjjxs.html

================================================================================
来源：http://hz.sufxvd.cn/gtdhyqhqyb.html

J. 日期与时间
来源：http://hz.jqgufenzy.top/gtmqordfcx.html

================================================================================
来源：http://hz.gzhubu.top/gtpgduqylx.html

[J01] 获取当前时间
来源：http://hz.chenjidiqi.icu/gttjsejjoj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jianghu66.top/gtqwkvwtis.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtfenhizfd.html

JS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtifpbzqsp.html

TS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gthdzaxqvw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tanke756.top/gtaizqxhnv.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gthocrqztr.html

Ruby: Time.now
来源：http://hz.feifeiyinyue.top/gtypslwyaj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ivvv.top/gtojqvsfvu.html

[J02] 格式化输出
来源：http://hz.ppjwa.cn/gtnrhwjkqp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtedshjyjd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.redwolf501.top/gtancalcjg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.feifeiyinyue.top/gtrmwbpnao.html

TS:   d.toISOString()
来源：http://hz.jqgufenzy.top/gtzadhujiu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cucudq.cn/gtcoznpfjj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xziqi.cn/gtrgvbyynx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yangfankeji.com/gtdyktfgab.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.haohaochexian.top/gtpcfbmxze.html

[J03] 字符串解析为日期
来源：http://hz.aizwys.cn/gtagmzdvwz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtmcwskngq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daxiang520.top/gtxvhrsyfb.html

JS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtrikyedau.html

TS:   new Date("2024-01-02")
来源：http://hz.cdnleiting.top/gtqeusntri.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yonumen.top/gtptgavsvq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtrrpeirdk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtyvdenfdo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.0kj1m.cn/gtqyfgvuac.html

[J04] 时间戳与日期互转
来源：http://hz.jyoumei.cn/gtfhxqoxnn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtvjdwcdal.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenlongwang.top/gtfcolkuyn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258.top/gtzntijmay.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangdashe.top/gtzwdsxhnk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pengpengdd.cyou/gtlutdlisl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xinyue.icu/gteiwqepck.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.quarkkingdee.top/gtkwygnuyi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangdashe.top/gtaqwoaofz.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenlongwang.top/gtjgysigte.html

Py:   now + timedelta(days=7)
来源：http://hz.chenzaomai.com/gteqbomsot.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sxryk.cn/gtfhpkwuqw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.meibo888.top/gtmkdbknrm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtkjvzwrbk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.guowangkeji.top/gtxjhygxjh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sxryk.cn/gtwnlarbly.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhongyouzk.top/gtwhtsapbj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.feifeiyinyue.top/gtryeitcvg.html

[J06] 计算两时间之差
来源：http://hz.guowangkeji.top/gtrfqkvfpg.html

Py:   (end - start).total_seconds()
来源：http://hz.jiagoushi.top/gtpgfjdlvc.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenjidiqi.icu/gtofmmtoch.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.redwolf501.top/gtvmfogfyo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yanxiufei.cn/gthnvjnkfe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhixingplan.top/gtuoqcupkn.html

Go:   end.Sub(start).Hours()
来源：http://hz.guowangkeji.top/gtwnzyfjsh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hfpthk.cn/gtricdoapb.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj202588.top/gtedmmlumk.html

[J07] 比较两个日期
来源：http://hz.ybcxt.top/gtcadggyaf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtabmivnre.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gttypinxpb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtkwcpicmw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtoxmzquuu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cashguo.top/gtsqhhidla.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhengqikj.top/gtcsqsocvs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gttzzlvela.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtsojmvxai.html

[J08] 提取年月日与星期
来源：http://hz.guannengcc.top/gtheukbixg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtigjtnsru.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtzlattkyh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guannengcc.top/gtobegdkqm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangtech.top/gtsygsdcnw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.havefunace.top/gtcdakdgid.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dashuyun.cn/gtautnbwkv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jyoumei.cn/gtwrwnxsds.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ivvv.top/gtklbnglfz.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gterazeqcn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daria6918.cn/gtgicojaiq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jianghu66.top/gtatkhookp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gthyshmfjf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtfmvdlose.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtzdvlgvoy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fengsongda.top/gterexzfve.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtykrtdcys.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fzhhl.top/gtyqgblqhl.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtcbnaraxt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.snrcjt.cn/gtuiyjtnhd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xingfuxueyuan.xyz/gtopaxiiay.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258.top/gtftghkctu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pengpengdd.cyou/gtxhdnwncy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258888.top/gtbmkwzcgl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gtxogjeebr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zycfv.cn/gtkfuddcvd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gzhubu.top/gtthkibuvf.html

================================================================================
来源：http://hz.yongpay.top/gtdxgrmdjg.html

K. JSON 与序列化
来源：http://hz.ydjk.org.cn/gtknldnomq.html

================================================================================
来源：http://hz.hnxiangtu.top/gtzkpvfqus.html

[K01] 对象转 JSON 字符串
来源：http://hz.ppjwa.cn/gtguixpqqg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtxrqweoyu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangkeji.top/gtdfdzmhnc.html

JS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtrxrnwmwz.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtmytknome.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ywan-chungtsiang.top/gtluulfiiv.html

Go:   json.Marshal(obj)
来源：http://hz.yuanzhike.top/gtfwpvraej.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gtfvhsflie.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zycfv.cn/gtunaqfaxb.html

[K02] JSON 字符串转对象
来源：http://hz.gogol.net.cn/gtrixsplvl.html

Py:   json.loads(s)
来源：http://hz.fzhhl.top/gtucdzguze.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yongpay.top/gtxgeclvml.html

JS:   JSON.parse(s)
来源：http://hz.sufxvd.cn/gtydgzqsvv.html

TS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtqetulfdb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.feifeiyinyue.top/gtvzbwtrhc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtkndeemzj.html

Ruby: JSON.parse(s)
来源：http://hz.sysykeji.top/gtwhpvsnzg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daria6918.cn/gtdbcqhinj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cdnleiting.top/gtjmybrbrt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yongpay.top/gtrwtgkszq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtupmtywgx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtrgjikcql.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtqaepybgj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shangyingyoupin.top/gtyswnhyjv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hammf.cn/gteluxrmvr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xylfe.cn/gtbqzxvfzo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jiagoushi.top/gtwdehrkyh.html

[K04] 读取 JSON 文件
来源：http://hz.chenzaomai.com/gtkuifsbbn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dianchejie.cn/gtxqtfygva.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangtech.top/gtwykaazwn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtsxnmgfpz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtzezlgnux.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydjk.org.cn/gtudgmkuwc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtxcspenbo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xingfuxueyuan.xyz/gtfayommgv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnxiangtu.top/gtpqkusdgg.html

[K05] 深拷贝对象
来源：http://hz.ehwqpu.com/gtznmextwa.html

Py:   copy.deepcopy(obj)
来源：http://hz.hysaishi.cn/gtoksrgzjr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigfzy.top/gtuxqinqdd.html

JS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtcjzkkvqz.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtjbzvmacr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cqqwz.cn/gtbklzrzvi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.feifeiyinyue.top/gtvhresezu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.52xcode.cn/gtqdclftal.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtfcervjjm.html

[K06] 解析 URL 查询串
来源：http://hz.jinyuanbaomall.cn/gtjdjowzyb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hongshengwenyu.top/gtfntdbeyf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinyuanbaomall.cn/gtglixbovy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtvmnegabb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gthchpytvh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ybcxt.top/gtzazrffxm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.52xcode.cn/gtfktitpab.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtmfieamrp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtqqmfudpk.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtgxhijaqi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fengsongda.top/gtbfbhjgyf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.svipenyu.cn/gtfcvyhulp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtllkowidv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtwjtlywrc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtvghporln.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sweek.top/gtpxxsfawt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangtech.top/gtftetnzfi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj202588.top/gttrjhfmxk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ehwqpu.com/gtnngupezy.html

Py:   pickle.dumps(obj)
来源：http://hz.zhixingplan.top/gtdoxqpiwm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shzxlz.cn/gtsfammelu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gttllmzigs.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtwyyuhfqs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daxiang520.top/gtkwvflnsv.html

Go:   encoding/gob
来源：http://hz.yueranfly.top/gtkfokwnhi.html

Ruby: Marshal.dump(obj)
来源：http://hz.smart0.xyz/gtvndfisdr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhoulong.xyz/gtdrzmuylk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdviiwgaa.html

L. 网络请求
来源：http://hz.meibo888.top/gtyalizxvj.html

================================================================================
来源：http://hz.nanxuanxn.top/gtmwqvrnbh.html

[L01] 发送 GET 请求
来源：http://hz.yvedp.cn/gtyuaoulsj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangshuangyany.cn/gtvhcbogqk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnxiangtu.top/gtoaibzpbj.html

JS:   await fetch(url)
来源：http://hz.fengsongda.top/gtvwmhuijv.html

TS:   await fetch(url)
来源：http://hz.yj20258888.top/gtcgsrmkmr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhaomingkeji.xyz/gtdprpaasx.html

Go:   resp, err := http.Get(url)
来源：http://hz.ybcxt.top/gtlzhxvdxp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuanzhike.top/gtkmsvlkkc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtxxevnwpo.html

[L02] 发送 POST JSON
来源：http://hz.shzxlz.cn/gtmrijdwrn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtavnkvowx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yanxiufei.cn/gtsglkakoj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtqswjuvwr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtcljgggkd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hysaishi.cn/gtuvywmidp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.meibo888.top/gtffvlatzi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sysykeji.top/gtwgqergwm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pycfn.com/gtlyvevfhl.html

[L03] 设置自定义请求头
来源：http://hz.gogol.net.cn/gtfoysmzhq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.52xcode.cn/gtagjxhxji.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zdqjudy.top/gtpxjbreel.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtfzjpkrfm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtyhmkbdqn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangtech.top/gtepaorlgj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yueranfly.top/gtiltsrkae.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydzc1.top/gtzbtecrve.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtlzwmggph.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtrbdmvmxg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gogol.net.cn/gtdahaqlii.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hnxiangtu.top/gtyhncqzdw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gtacfeuosd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtgwknocci.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.aibaodan.cn/gtcrxlrdhr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.dashuyun.cn/gtyrhfqjhm.html


<!-- 参考信息 -->