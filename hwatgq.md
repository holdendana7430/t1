代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sysykeji.top/gtkmvbluid.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhengqikj.top/gtzedtethe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gtzfbtlnpx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtiefiltcb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ehwqpu.com/gtebxhtfnu.html

Go:   defer f.Close()
来源：http://hz.wangshuangyany.cn/gtrxomtqmb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yueranfly.top/gtmyfmjabb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.quarkkingdee.top/gtteuxvpdc.html

================================================================================
来源：http://hz.mhx1999.top/gtcvqavzgg.html

I. 正则表达式
来源：http://hz.jianghu66.top/gtsmjwwbkl.html

================================================================================
来源：http://hz.0kj1m.cn/gtvqwvfety.html

[I01] 判断是否匹配
来源：http://hz.wangshuangyany.cn/gtmfczugcm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.havefunace.top/gtwjgluxby.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yangfankeji.com/gtmfrwpcrb.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtzakghqjk.html

TS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gthgspporq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.mhx1999.top/gtftzglphy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xylfe.cn/gturgstkvo.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnxiangtu.top/gtlqknfaav.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ybcxt.top/gtbklzmpoi.html

[I02] 提取所有匹配
来源：http://hz.yj20258888.top/gtkxbnmdnq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtacjyxvfc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258.top/gtqjzkapfg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gzhubu.top/gtglvvymii.html

TS:   s.match(/\d+/g)
来源：http://hz.ivvv.top/gtujerkbnk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenzaomai.com/gtffjcvbuv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sweek.top/gtpbanmekb.html

Ruby: s.scan(/\d+/)
来源：http://hz.0kj1m.cn/gtcvtrzwgy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dashuyun.cn/gtcpfsgdit.html

[I03] 提取捕获分组
来源：http://hz.fengsongda.top/gtctwzoprx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sysykeji.top/gtgqlnoifs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangdashe.top/gtoggagaik.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guowangkeji.top/gtwbpwgszs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.svipenyu.cn/gtivplvzay.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sweek.top/gtutizvitb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yvedp.cn/gtyssmjtjr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtefewmxdn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sysykeji.top/gthryvusib.html

[I04] 正则替换
来源：http://hz.andypj.xyz/gthvlagtvu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gtagemggxe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtyvbikksw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtbqzqcfpc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtenbadgxy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dianchejie.cn/gtbbhdclcu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenlongwang.top/gtrptycldo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sweek.top/gthipauemo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shangyingyoupin.top/gtdliawrki.html

[I05] 按正则拆分
来源：http://hz.dianchejie.cn/gtxrakhqez.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zycfv.cn/gtqsppdyfu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258888.top/gtjcomjrhv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gturfnemij.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtoevncpbf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zdqjudy.top/gtaxikjxca.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuetiantiany.cn/gtucsqmfnq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gthmkmuyeg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jiagoushi.top/gtgmgsrpej.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj202588.top/gtjjgplpjp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtqvjqgfqb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gtrkvrrfss.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtpnoywzua.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtkpzquder.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhongyouzk.top/gtxzkabvwp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shuidangran.top/gtjhwfkygl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgfzy.top/gtjvfsfcux.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtemnnmems.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhengqikj.top/gtbrajbjmo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sxryk.cn/gtltwreteq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.andypj.xyz/gtyancaruy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.feifeiyinyue.top/gtfopvrggu.html

TS:   /error/gim
来源：http://hz.bjfxy.top/gtbtyilyvn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.quarkkingdee.top/gtmyhsjjnh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hywenlv.cn/gtshdsjlje.html

Ruby: s.scan(/error/i)
来源：http://hz.hywenlv.cn/gtogxsttgo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhongyouzk.top/gtgjjafeci.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dianchejie.cn/gtyrqtdroj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pycfn.com/gtjswwlvyp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuetiantiany.cn/gttwucmtuh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.quarkkingdee.top/gtjbfcztlc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtmifyfybi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tian-w.cn/gtjpbwqmft.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hywenlv.cn/gtkukqvzmw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hammf.cn/gtrnpaplij.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gtgwieduts.html

================================================================================
来源：http://hz.meibo888.top/gtanhmjqwr.html

J. 日期与时间
来源：http://hz.xinyue.icu/gtotcfbrxk.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtnarbgvpg.html

[J01] 获取当前时间
来源：http://hz.jianghu66.top/gtniezchmz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hnqzz.top/gtzvyuxsfg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sweek.top/gtlgdydhpg.html

JS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtqfuozjpz.html

TS:   new Date();  Date.now()
来源：http://hz.meibo888.top/gtkymlepui.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.316326.xyz/gtqmbjlbzj.html

Go:   time.Now()
来源：http://hz.jyoumei.cn/gtnulodrnf.html

Ruby: Time.now
来源：http://hz.shangyingyoupin.top/gtieldxola.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhengqikj.top/gtrwhujabb.html

[J02] 格式化输出
来源：http://hz.zhongyouzk.top/gtxcauvxzm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.havefunace.top/gthlnkfxve.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtvczhiyob.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtddvhtyvy.html

TS:   d.toISOString()
来源：http://hz.hnxiangtu.top/gtchgztvsq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ppjwa.cn/gtotqnrwdg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.mhx1999.top/gtdlxwgsyi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtmimmobuu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hongshengwenyu.top/gtohrsbtzp.html

[J03] 字符串解析为日期
来源：http://hz.xziqi.cn/gtqqlfbehq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xingfuxueyuan.xyz/gtftlckfnr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hysaishi.cn/gtzzzayfhw.html

JS:   new Date("2024-01-02")
来源：http://hz.fzhhl.top/gtzxvfcfex.html

TS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gttpjekeyw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gthqozxxsi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtjkirqpcv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtatjxxdpt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtdfntesra.html

[J04] 时间戳与日期互转
来源：http://hz.hongshengwenyu.top/gtsjifbxui.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.kuanghao11.cn/gtyuaebgvt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zycfv.cn/gtojchoymo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.9152youxi.cn/gtfgjmgiuc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gtkgvaflbj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guannengcc.top/gtwndohqip.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.quarkkingdee.top/gtuepkxlcs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.0kj1m.cn/gtrsesejem.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.c1oappe.top/gtqmzssjkl.html

[J05] 时间加减（加 7 天）
来源：http://hz.sweek.top/gtfcfvixvh.html

Py:   now + timedelta(days=7)
来源：http://hz.bjfxy.top/gtaohanduh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xziqi.cn/gtqwpjmzkx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gtidcaahyk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtvgbkmvtf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj202588.top/gthqubease.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sxryk.cn/gtacrztbai.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenlongwang.top/gtlftdslqx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangshuangyany.cn/gtxidvnvnj.html

[J06] 计算两时间之差
来源：http://hz.daxiang520.top/gtdnfytvtp.html

Py:   (end - start).total_seconds()
来源：http://hz.ydjk.org.cn/gtuhadoqkk.html

PHP:  $end->diff($start)->days;
来源：http://hz.zycfv.cn/gtfraguqen.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.iojbl.cn/gtxrpynwhq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhongyouzk.top/gtsxlkzbhn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.52xcode.cn/gtzxliephe.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gtpyeiohhv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yonumen.top/gtgnpapxnw.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtimmcsppb.html

[J07] 比较两个日期
来源：http://hz.cqqwz.cn/gtkblpycgg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gthwmsjrzd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jyoumei.cn/gtvydxaguf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gteicrqmik.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtwnkrgkzg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cdnleiting.top/gtuthlaovd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cashguo.top/gtpnsokkfy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtvedannxs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtnnepvtfa.html

[J08] 提取年月日与星期
来源：http://hz.tianlin.xyz/gtvylimwzs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hongshengwenyu.top/gtaomambjr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinghuilouyu.cn/gtdyyxryfc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aibaodan.cn/gtrhmfybrb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xylfe.cn/gtdqlpvtiw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pycfn.com/gtuwqmvnyz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtvalwdivl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258888.top/gtumgqnjbv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuetiantiany.cn/gtjwinqajg.html

[J09] 时区处理
来源：http://hz.sufxvd.cn/gtmmbjdtpz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xingfuxueyuan.xyz/gtnajxdclh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pycfn.com/gtxkltgidh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtjtfhuawd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtljkzsjle.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuanzx.com/gtocedpuqd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cdnleiting.top/gtkjhrepen.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.andypj.xyz/gtsupmxqjt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgufenzy.top/gtgzgdlneh.html

[J10] 取今天 / 本月第一天
来源：http://hz.ehwqpu.com/gtfzetgcjj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aibaodan.cn/gtzpavtehg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinyuanbaomall.cn/gtuqvlhwxs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gthvkkufkk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yongpay.top/gtdbhecrla.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.kuanghao11.cn/gtltukfjas.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuetiantiany.cn/gtakrwpllv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydzc1.top/gtneioabat.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gtyzvzsfjc.html

================================================================================
来源：http://hz.jqgfzy.top/gtoymmeuhn.html

K. JSON 与序列化
来源：http://hz.xuetiantiany.cn/gtzucsmumc.html

================================================================================
来源：http://hz.zhijiandao.cn/gtlaqmmpiy.html

[K01] 对象转 JSON 字符串
来源：http://hz.jianghu66.top/gtnackunza.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtixecrcar.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtugedpdcg.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtnqwxikwd.html

TS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtbieonnny.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.quarkkingdee.top/gtjcsgklfq.html

Go:   json.Marshal(obj)
来源：http://hz.zhaomingkeji.xyz/gtycmdktcq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ivvv.top/gtwwsmzooz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinyuanbaomall.cn/gtffdofnxw.html

[K02] JSON 字符串转对象
来源：http://hz.xylfe.cn/gtrltpqoyr.html

Py:   json.loads(s)
来源：http://hz.chenlongwang.top/gttjptjhqb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daxiang520.top/gtsrhlibtn.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtldksdqyv.html

TS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtrymmxhvv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gaohongyu789.top/gtjbjicazt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shzxlz.cn/gtytweucdx.html

Ruby: JSON.parse(s)
来源：http://hz.fengsongda.top/gtlzwrcnpp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinghuilouyu.cn/gtcgweufyr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tianlin.xyz/gtwgykcggw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtqqcuykau.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtpyvefwgd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jianghu66.top/gtocatgoih.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtbeaxxfvj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtqjiitnej.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gaohongyu789.top/gtqieuqmcm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yvedp.cn/gtdwczaoya.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgufenzy.top/gtwegjnseh.html

[K04] 读取 JSON 文件
来源：http://hz.sufxvd.cn/gtswqhufak.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gaohongyu789.top/gtokdnscxl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hywenlv.cn/gtirekxrox.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gtecqijynp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtzaexjgfn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigfzy.top/gtfagcfltm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtpkhdvdqt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yvedp.cn/gtpdztjrah.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jyoumei.cn/gtklqfcsql.html

[K05] 深拷贝对象
来源：http://hz.cashguo.top/gtcznriylv.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnxiangtu.top/gtugwahxsu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtcvtyvirr.html

JS:   structuredClone(obj)
来源：http://hz.hnqzz.top/gtopoknhjk.html

TS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtkyptdshp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xinyue.icu/gtaiwbuend.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydjk.org.cn/gtprjyvunx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xinyue.icu/gtnzzpnkvi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhongyouzk.top/gtgftvanij.html

[K06] 解析 URL 查询串
来源：http://hz.zhiwuduotai.top/gtyenlrqbt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258.top/gtwgzglllr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daxiang520.top/gtkrgugqoc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtkwnsrblt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtteuutied.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zdqjudy.top/gtmwvnsjaq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtbrzpnwpr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gogol.net.cn/gthcydjtiz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tian-w.cn/gtikyuhxga.html

[K07] 进制转换
来源：http://hz.ydzc1.top/gtsdqbqdzf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhengqikj.top/gtayewahks.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cdnleiting.top/gtrthfqrau.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtgdnskqiw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtafabviiv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtfbusbfew.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cheryme.top/gtldyndqfv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.haohaochexian.top/gtkhbsxzgt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hywenlv.cn/gtwfsnmoyn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sysykeji.top/gtftrzdwhz.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigufen.top/gtpvvzrfsh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ydzc1.top/gtyyeepqll.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gtkjzatgxp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gttxkzedsf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.kuanghao11.cn/gteirbrofx.html

Go:   encoding/gob
来源：http://hz.ehwqpu.com/gtwuxqbfbu.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhijiandao.cn/gtukzivmib.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj202588.top/gtlhdxnbqg.html

================================================================================
来源：http://hz.meibo888.top/gtothkxecb.html

L. 网络请求
来源：http://hz.zhongyouzk.top/gtveeymxtp.html

================================================================================
来源：http://hz.fzhhl.top/gtkkfioizq.html

[L01] 发送 GET 请求
来源：http://hz.zhengqikj.top/gtfkrndngp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yvedp.cn/gtwmtnesbh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jlsjyb.cn/gtwwcydhzo.html

JS:   await fetch(url)
来源：http://hz.cucudq.cn/gtqugudrir.html

TS:   await fetch(url)
来源：http://hz.iojbl.cn/gtpkivldyo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shzxlz.cn/gtpfjcgobo.html

Go:   resp, err := http.Get(url)
来源：http://hz.pengpengdd.cyou/gtdflqgotg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangkeji.top/gtymvcimru.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ybcxt.top/gtptzbecvt.html

[L02] 发送 POST JSON
来源：http://hz.yj20258.top/gtkohdhfhu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.fzhhl.top/gtvznuptie.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.svipenyu.cn/gtjdqygyep.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gtibemtzmh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gthrzbnzvh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sysykeji.top/gthomwjcza.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yongpay.top/gtwkdjmswy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.kuanghao11.cn/gtkmfsdrdg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tianlin.xyz/gtizksnsvm.html

[L03] 设置自定义请求头
来源：http://hz.cqqwz.cn/gtfhjzqieg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuxming.cn/gtctfejlal.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.snrcjt.cn/gtkemcmbjd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtszhbuogi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gtqnvfgncs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sufxvd.cn/gtlmcpmepf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gttbinbdnj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yonumen.top/gtwufocmqi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtrnbbelcu.html

[L04] 设置超时
来源：http://hz.guowangkeji.top/gtubxxjdap.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydzc1.top/gthyqlugsw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aizwys.cn/gtzuwhvhlk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtmmlsosep.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gtwjfwqwjb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fzhhl.top/gtsbeghqjy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fzhhl.top/gtregkwrnh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhijiandao.cn/gtpsvduaft.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtvkplkysd.html

[L05] 上传文件（multipart）
来源：http://hz.jiagoushi.top/gtqhopfigp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtgnjyjvcm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangkeji.top/gtpoyzhzcp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtoidnducu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtdnfwwhvl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.dashuyun.cn/gtgrexlfnk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.quarkkingdee.top/gteljwcpvg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yonumen.top/gtlberabac.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtexwpnimm.html

[L06] 解析响应为 JSON
来源：http://hz.hfpthk.cn/gtkiogwbii.html


<!-- 参考信息 -->