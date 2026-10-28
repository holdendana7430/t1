代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.0kj1m.cn/gtnukjwmvm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xinyue.icu/gtxwwjmcez.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.andypj.xyz/gtpxrddcms.html

[H10] 资源自动释放
来源：http://hz.cdnleiting.top/gtpbnsosiu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinqigufen.top/gtvdxsdzjq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fengsongda.top/gtzdmiomak.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtvbokncdg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtdnampdxt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinghuilouyu.cn/gtsmmmfpii.html

Go:   defer f.Close()
来源：http://hz.bjfxy.top/gtjumnitkw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.guowangkeji.top/gtpkcmzzdl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hammf.cn/gtnawxzsjr.html

================================================================================
来源：http://hz.iojbl.cn/gttfphzzep.html

I. 正则表达式
来源：http://hz.ehwqpu.com/gtqdpybjqe.html

================================================================================
来源：http://hz.gogol.net.cn/gtybdbzkad.html

[I01] 判断是否匹配
来源：http://hz.jianghu66.top/gtyddcgihc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fengsongda.top/gtphllmzsb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shanyushiyangtech.top/gtqpqhiwwq.html

JS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtwawlbnow.html

TS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtoozhbvua.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.snrcjt.cn/gtjyhswctt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gtnsecahph.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtkzhflsss.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sysykeji.top/gtbifvafeq.html

[I02] 提取所有匹配
来源：http://hz.yongpay.top/gtgzucbdos.html

Py:   re.findall(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtuqjjfszj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.snrcjt.cn/gtgxvlpzsk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sweek.top/gtfpvmilbq.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtqpithnbq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cqqwz.cn/gtsetycrec.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtgwyhmobl.html

Ruby: s.scan(/\d+/)
来源：http://hz.nwbrower.top/gtmyljobfc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sufxvd.cn/gtjqgblpvn.html

[I03] 提取捕获分组
来源：http://hz.cheryme.top/gtbmkkqlos.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhiwuduotai.top/gtwusuxrgj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sysykeji.top/gteymducle.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenlongwang.top/gtzyzttdbc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gaohongyu789.top/gthkznjswh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dashuyun.cn/gtjgdvstzh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ehwqpu.com/gttxlyjgay.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.snrcjt.cn/gtrzypsybp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shanyushiyangtech.top/gtageckmkj.html

[I04] 正则替换
来源：http://hz.haohaochexian.top/gtsbnkwmea.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cqqwz.cn/gtmrhxaism.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pengpengdd.cyou/gtmlrmmkce.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtwriozfzp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shuidangran.top/gtqdjxpuop.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tian-w.cn/gtkunqyhro.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gzhubu.top/gtklscqvjx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhiwuduotai.top/gtcpypmmyj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenlongwang.top/gtryfilivg.html

[I05] 按正则拆分
来源：http://hz.feifeiyinyue.top/gtgzcjueti.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sxryk.cn/gtwxqabtsz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhaomingkeji.xyz/gtkpscqtzm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtpkecvuym.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtaaoiwgsp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.0kj1m.cn/gteozrdjfw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.mhx1999.top/gtogbdodre.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtgxwhnkfv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gthiaqpgtv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangdashe.top/gtonopdfji.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtqnxgfhhv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ybcxt.top/gtarzxelxp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtrckuvrlf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtyqfforxc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jiagoushi.top/gtocirwlrn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tanke756.top/gtzqxgltyp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinyuanbaomall.cn/gtcoobbqcd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtnhgfhnoq.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenlongwang.top/gttdthrwxt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxuanxn.top/gtkxrzpzfg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zycfv.cn/gtnzxhabsh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gaohongyu789.top/gthgkdsozq.html

TS:   /error/gim
来源：http://hz.zhijiandao.cn/gtxsoupmbk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sweek.top/gtgxpxieep.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cdnleiting.top/gtulqagdgy.html

Ruby: s.scan(/error/i)
来源：http://hz.cucudq.cn/gtbcglcoed.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cqqwz.cn/gtrkyinevj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangdashe.top/gtprjghlwk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.dashuyun.cn/gtxmmiittg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gtyegnkebi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtnmabvzwk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtejcwzsoe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydjk.org.cn/gtiwjiqmaw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhoulong.xyz/gtvejgpfqh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guowangkeji.top/gtmplckhxk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yuxming.cn/gtpwgwubst.html

================================================================================
来源：http://hz.ppjwa.cn/gtmxgszgmr.html

J. 日期与时间
来源：http://hz.iojbl.cn/gtfzccgqbn.html

================================================================================
来源：http://hz.tianlin.xyz/gtcgbmkxis.html

[J01] 获取当前时间
来源：http://hz.dianchejie.cn/gtwuzecaea.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258.top/gtvqfdbnnl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.mhx1999.top/gtlxpgnuku.html

JS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtsygpkfbb.html

TS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gthfpcjjmq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shuidangran.top/gtxxbxwcho.html

Go:   time.Now()
来源：http://hz.jianghu66.top/gttlenlphz.html

Ruby: Time.now
来源：http://hz.nanxinkj.top/gtmwjsuype.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258.top/gtdcbatvdv.html

[J02] 格式化输出
来源：http://hz.mhx1999.top/gtmhaiifzk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtqithxmah.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gtrrqbnavr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jyoumei.cn/gtbfohfhey.html

TS:   d.toISOString()
来源：http://hz.yongpay.top/gtohgdxacc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gogol.net.cn/gtofqmhtll.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenzaomai.com/gtowdkmleo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtsiwpieot.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenlongwang.top/gtnxrfmyxs.html

[J03] 字符串解析为日期
来源：http://hz.shzxlz.cn/gtzrznlgil.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aizwys.cn/gtoqupwewp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aizwys.cn/gtmgfdjkhg.html

JS:   new Date("2024-01-02")
来源：http://hz.jianghu66.top/gtexsoxbik.html

TS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gtfzsnkpxy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtsubvyody.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtqgdigfgw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gtfmoombrh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sweek.top/gtntkcmcmy.html

[J04] 时间戳与日期互转
来源：http://hz.52xcode.cn/gtvszjrbvi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.redwolf501.top/gtmdkcjyhq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangtech.top/gtcadimiie.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yongpay.top/gttvookrjq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtxwnpxcyy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pycfn.com/gtqldkgwpk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hongshengwenyu.top/gtvbzpsseg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuetiantiany.cn/gttydafwct.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gtgcbzwvnl.html

[J05] 时间加减（加 7 天）
来源：http://hz.yongpay.top/gtlfpqxuuw.html

Py:   now + timedelta(days=7)
来源：http://hz.zhiwuduotai.top/gtoxdeetbe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hywenlv.cn/gtezslkmik.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guannengcc.top/gthbzpdydx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtpaeuipsk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtnnhbyptq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zycfv.cn/gtrunuvgni.html

Ruby: Time.now + 7 * 86400
来源：http://hz.andypj.xyz/gturehnufr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pengpengdd.cyou/gtxyqlgaqe.html

[J06] 计算两时间之差
来源：http://hz.birdmap.top/gtyhmgugit.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gtladwnsnn.html

PHP:  $end->diff($start)->days;
来源：http://hz.yongpay.top/gtsjebrihu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gtrledbywt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhiwuduotai.top/gtasgssbua.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cucudq.cn/gtcqeeelzz.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangtech.top/gtluozhqwe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.andypj.xyz/gtqijhxyzi.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gtqfwcghrl.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtqpvpwlsl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtorocfkfc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ywan-chungtsiang.top/gtvsrfxxif.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.redwolf501.top/gtrwmavery.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtfluviwkc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnqzz.top/gtbvudssyj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhaomingkeji.xyz/gtvjjwzvan.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtmjrnnzpg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtbgtuebgl.html

[J08] 提取年月日与星期
来源：http://hz.meibo888.top/gtdncxqvez.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gtyacqbpis.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.quarkkingdee.top/gtaubrzluz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tianlin.xyz/gtdackmrhq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnqzz.top/gtzjcbuhus.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gogol.net.cn/gtfhozneio.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gtbmcqeirj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gtfqisxmrp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guannengcc.top/gtdgfldrnd.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtjsdsdfet.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.svipenyu.cn/gtzmuatpiy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yvedp.cn/gtiejnxqlx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtihyrwytz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtabbojqhz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigufen.top/gtmqrzuxpv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daria6918.cn/gtuxwaxidr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ivvv.top/gtegklgfne.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hfpthk.cn/gttfopzibv.html

[J10] 取今天 / 本月第一天
来源：http://hz.xziqi.cn/gtvowkrkqa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jyoumei.cn/gtsyjvdsrs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guannengcc.top/gtbnndxmal.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gotoacloud.top/gtbuqiyspx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jqgfzy.top/gtbceahyvr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhijiandao.cn/gtyurhxqji.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dashuyun.cn/gtymwkxjud.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuanzx.com/gthjlduleg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daxiang520.top/gtsmhyuzuf.html

================================================================================
来源：http://hz.xylfe.cn/gtztyoaxzl.html

K. JSON 与序列化
来源：http://hz.9152youxi.cn/gtaqhlpgnb.html

================================================================================
来源：http://hz.hysaishi.cn/gtfroyzsuh.html

[K01] 对象转 JSON 字符串
来源：http://hz.cdnleiting.top/gtwgfruqdg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtljhoxjye.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hongshengwenyu.top/gtwyszwkja.html

JS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtqazygsev.html

TS:   JSON.stringify(obj)
来源：http://hz.shangyingyoupin.top/gtbqtlitas.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hnqzz.top/gthtmtjumg.html

Go:   json.Marshal(obj)
来源：http://hz.daxiang520.top/gtdzkwylbv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hysaishi.cn/gtjqowvfak.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenjidiqi.icu/gtigdjtfyv.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gtjgbnziqm.html

Py:   json.loads(s)
来源：http://hz.zdqjudy.top/gtzqutzmra.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydjk.org.cn/gtprjhubsw.html

JS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtoiqyumpj.html

TS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtwcjembnp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.mhx1999.top/gtpxznzwtm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtdaaorokg.html

Ruby: JSON.parse(s)
来源：http://hz.meibo888.top/gtujzqubzp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ppjwa.cn/gttiljrrwt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtilicycsv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtmqjfxdua.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtfummotlf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ivvv.top/gtgzqbbzhu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtzdcydrcw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cashguo.top/gtoveswgou.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.meibo888.top/gtfdpcvmaw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.pycfn.com/gtehnatqkw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.kuanghao11.cn/gtoijytzdp.html

[K04] 读取 JSON 文件
来源：http://hz.hywenlv.cn/gtsutnxyxn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gtyivntjpr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gaohongyu789.top/gtzujvmfhk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtmmtqkcso.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtzurfcjtf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangshuangyany.cn/gtxzjehahm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtumjmcvrp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.0kj1m.cn/gtknzojtmu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gtoxireyhj.html

[K05] 深拷贝对象
来源：http://hz.chenlongwang.top/gtrfavqhdi.html

Py:   copy.deepcopy(obj)
来源：http://hz.yonumen.top/gtqmorktzv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.haohaochexian.top/gtkzqfetoj.html

JS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtpnxnhckh.html

TS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtcargexkb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cqqwz.cn/gtziuzyrvt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.meibo888.top/gtaiscqsqa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aibaodan.cn/gtylzegirx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydjk.org.cn/gtsbgclgep.html

[K06] 解析 URL 查询串
来源：http://hz.nanxinkj.top/gtvzfxpkqs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dianchejie.cn/gtbslodrkp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtflealnar.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gttujlxvld.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtvpsfslow.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hysaishi.cn/gtnigqerfd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gtrendyevi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zycfv.cn/gtgjovicgr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shzxlz.cn/gtkzhbtjnu.html

[K07] 进制转换
来源：http://hz.wangdashe.top/gtsqkxusfl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tanke756.top/gtawmwbpkq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fengsongda.top/gtjlysudfn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gtjlrroqpg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtnvuzmrzs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtvfirzvrt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yonumen.top/gtesckyhsw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daria6918.cn/gthodtmezt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pycfn.com/gtvyillxes.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhengqikj.top/gtaucftqov.html

Py:   pickle.dumps(obj)
来源：http://hz.guowangkeji.top/gtjksnthir.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhongyouzk.top/gtjjjoayyy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.vqdsnc.cn/gtjhdjtwsq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtllojtmzs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtpewzocrl.html

Go:   encoding/gob
来源：http://hz.snrcjt.cn/gtvjayisfa.html

Ruby: Marshal.dump(obj)
来源：http://hz.smart0.xyz/gtqevukzij.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgufenzy.top/gtanfryinc.html

================================================================================
来源：http://hz.xziqi.cn/gtjqrqzyhp.html

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gthfbqwgsg.html

================================================================================
来源：http://hz.jlsjyb.cn/gthskdvwue.html

[L01] 发送 GET 请求
来源：http://hz.hfpthk.cn/gtuipcqgvq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhixingplan.top/gtaxsatewr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daria6918.cn/gtdyzttlci.html

JS:   await fetch(url)
来源：http://hz.cheryme.top/gtptdasmto.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtafrdizcn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.bjfxy.top/gtruulpepo.html

Go:   resp, err := http.Get(url)
来源：http://hz.gaohongyu789.top/gtebdtncsr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hfpthk.cn/gthxfjxolv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtprkxmond.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtdvujhzkp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhengqikj.top/gtfxhvctht.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tianlin.xyz/gtopqiixdd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.bjfxy.top/gtwtcbxlae.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtabrjouzr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.feifeiyinyue.top/gttwtbhuan.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pengpengdd.cyou/gtcuspcfaq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxinkj.top/gtxwcxzahc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgufenzy.top/gtkoemjhro.html

[L03] 设置自定义请求头
来源：http://hz.nanxinkj.top/gtjptyroiv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuetiantiany.cn/gtqhzljokh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.dashuyun.cn/gtlxkxmssc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtsoeaulbd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gtfrenxbef.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxinkj.top/gtxkqtzzwn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtkoljvvym.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xingfuxueyuan.xyz/gtswfrvkkn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.aibaodan.cn/gtfwubzxmp.html

[L04] 设置超时
来源：http://hz.hnxiangtu.top/gthmuzumkn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhoulong.xyz/gtfokjphny.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.meibo888.top/gtvujxtmiq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtskqgbuap.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtaaqfoeik.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xziqi.cn/gtnnhtcfyp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tian-w.cn/gtdgspxdyy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuetiantiany.cn/gtlvnpboey.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.andypj.xyz/gtpwjdjiuh.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtxflitrqt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigufen.top/gtvbzjcuki.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangtech.top/gtslokbjoj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtmqeszpxo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtcyuqvhgq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zycfv.cn/gttbcpoqdt.html


<!-- 参考信息 -->