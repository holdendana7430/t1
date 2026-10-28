代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hz.gaohongyu789.top/gtcmvbwomq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhiwuduotai.top/gtfjiilkil.html

[H09] 带错误码的异常
来源：http://hz.ywan-chungtsiang.top/gttylzrbbo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhengqikj.top/gtsbxcvohe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tanke756.top/gtizxtcwpa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258.top/gttdycgwow.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.andypj.xyz/gtdmovwzfp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.daria6918.cn/gtzaeklaau.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ehwqpu.com/gtxymetqsv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangdashe.top/gtczbmqaam.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jlsjyb.cn/gtyyxenywf.html

[H10] 资源自动释放
来源：http://hz.pengpengdd.cyou/gtvlmdmuxk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yanxiufei.cn/gtlzqekamm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.aizwys.cn/gtczcsybpv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yangfankeji.com/gtqyvjczwd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtotqjmwvl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.andypj.xyz/gtskttkfcr.html

Go:   defer f.Close()
来源：http://hz.ppjwa.cn/gtwocwkhae.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gogol.net.cn/gtyfjxmbkr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.svipenyu.cn/gtmvfpqasc.html

================================================================================
来源：http://hz.xylfe.cn/gtvzvnuamw.html

I. 正则表达式
来源：http://hz.redwolf501.top/gtpkfvrtyb.html

================================================================================
来源：http://hz.jqgufenzy.top/gtmipijdjb.html

[I01] 判断是否匹配
来源：http://hz.xinyue.icu/gtjxklafno.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gtblxalpek.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zycfv.cn/gtdwbnrtlf.html

JS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtuakedwwt.html

TS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtbkanpcoz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gogol.net.cn/gttaasxcvn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ivvv.top/gtlnqqoulc.html

Ruby: s.match?(/\d+/)
来源：http://hz.shangyingyoupin.top/gtjfwczfkh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cdnleiting.top/gtyqdrzwoi.html

[I02] 提取所有匹配
来源：http://hz.yueranfly.top/gtccuqdwth.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zycfv.cn/gtwjgvrjqk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jiagoushi.top/gtnevhpnkx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cqqwz.cn/gtojdfenmz.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangkeji.top/gtoxkvhjen.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.smart0.xyz/gtnqftgjwl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtgnobxkjv.html

Ruby: s.scan(/\d+/)
来源：http://hz.fzhhl.top/gtpeoovvue.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtmwozwfax.html

[I03] 提取捕获分组
来源：http://hz.yongpay.top/gtkfzjmudr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.smart0.xyz/gtvnycludt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gtbkaowaoe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ybcxt.top/gtvkyadshn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxuanxn.top/gtpidhqixq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangshuangyany.cn/gthwiybkdb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tanke756.top/gthayehqvf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hongshengwenyu.top/gtyjqjkymn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.c1oappe.top/gtwonskpgr.html

[I04] 正则替换
来源：http://hz.316326.xyz/gtvdfsigzy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hammf.cn/gtmlnxpwtw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.52xcode.cn/gtxhayfcwj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gttwwnchsx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.wangdashe.top/gtaxradhpx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhijiandao.cn/gtopeukgme.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangshuangyany.cn/gtehjtdgaf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yanxiufei.cn/gtrqtbsqoy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xinyue.icu/gtsbkdhkaw.html

[I05] 按正则拆分
来源：http://hz.zhaomingkeji.xyz/gttiuoahte.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuetiantiany.cn/gtjvcqbddk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenlongwang.top/gtoopsyhdq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtnilmlhzk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtgpqrcrgj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hywenlv.cn/gtlyryiash.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhixingplan.top/gtyfgogojf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gttimgsjfp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ybcxt.top/gtuqmmpexd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sysykeji.top/gttsngfdhm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gthbrrvsos.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yvedp.cn/gtthqujmrn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtdqhefkrb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gtdskgmfgo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yuanzhike.top/gtkuhmcnxn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtivjvszuu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangshuangyany.cn/gtkcgkuqpf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtslbysqus.html

[I07] 忽略大小写与多行模式
来源：http://hz.sufxvd.cn/gthtdktfnf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yangfankeji.com/gtnwvzyayk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sufxvd.cn/gtqabytjnx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jiagoushi.top/gtkalyzfcm.html

TS:   /error/gim
来源：http://hz.quarkkingdee.top/gtguoxwsze.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.316326.xyz/gtkkkpwssk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yueranfly.top/gtszbzsqfl.html

Ruby: s.scan(/error/i)
来源：http://hz.zhixingplan.top/gthzznxmwi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jiagoushi.top/gtwkzjcsti.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtgelzsdkt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hnxiangtu.top/gtmgijxefe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj202588.top/gtloyknfxa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtozblfihz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenjidiqi.icu/gtuulrewuc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtpgsldplk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhijiandao.cn/gtewhizggi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gtunhbxxdp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gogol.net.cn/gtubptpuqw.html

================================================================================
来源：http://hz.jianghu66.top/gthauzxynn.html

J. 日期与时间
来源：http://hz.mhx1999.top/gtrhvhpuxa.html

================================================================================
来源：http://hz.wangdashe.top/gtyruahhbc.html

[J01] 获取当前时间
来源：http://hz.zhongyouzk.top/gtduxslobt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangkeji.top/gtlnsjkkwu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gtftgtcthp.html

JS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtopeydeoc.html

TS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtrawuypbr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gotoacloud.top/gtfxhaiwcb.html

Go:   time.Now()
来源：http://hz.xziqi.cn/gthdkhsplc.html

Ruby: Time.now
来源：http://hz.c1oappe.top/gtaryqlmfr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangtech.top/gtsfkihmow.html

[J02] 格式化输出
来源：http://hz.snrcjt.cn/gtmycotoww.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtlebkbvyo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtzuvocatx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhongyouzk.top/gtbtwemcwc.html

TS:   d.toISOString()
来源：http://hz.hongshengwenyu.top/gttzzkysdn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yangfankeji.com/gtxtdtfatb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinyuanbaomall.cn/gtzdhikqen.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gthdbzeghg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenzaomai.com/gtunsefwrd.html

[J03] 字符串解析为日期
来源：http://hz.kuanghao11.cn/gtukctyokx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangtech.top/gtbnnfdvtj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.bjfxy.top/gttpwceuoe.html

JS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtscbpyzvl.html

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtynnvoqie.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtbopvxilo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sufxvd.cn/gtshkzoxyn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtltdfwxyr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shanyushiyangkeji.top/gtvjoxemwd.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtpquaokpm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.guannengcc.top/gtmzfuefmy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangkeji.top/gtschzqrto.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gaohongyu789.top/gtgklvpgxs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yonumen.top/gtuyljxfit.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cdnleiting.top/gtsbhjpudr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aizwys.cn/gtrtyxcwvv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.birdmap.top/gtizxrjqzh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daxiang520.top/gtldzqhjia.html

[J05] 时间加减（加 7 天）
来源：http://hz.mhx1999.top/gtbhexjwtn.html

Py:   now + timedelta(days=7)
来源：http://hz.guowangkeji.top/gtdyumeksw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tanke756.top/gtegqkejnr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtcusmqwze.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtnykvtgsv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenlongwang.top/gtdczbdxre.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.dashuyun.cn/gtumagftrt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinyuanbaomall.cn/gtiwnndozj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.bjfxy.top/gtmxpyqxin.html

[J06] 计算两时间之差
来源：http://hz.cheryme.top/gtwknextly.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gtakvljdsd.html

PHP:  $end->diff($start)->days;
来源：http://hz.wangshuangyany.cn/gtclfwofwn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhiwuduotai.top/gtrqezdiwg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.fzhhl.top/gtbcpwvujz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuanzx.com/gtemiymiwa.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinghuilouyu.cn/gtlybknovf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xuanzx.com/gtbuvvsodn.html

C#:   (end - start).TotalSeconds
来源：http://hz.shuidangran.top/gthyzefufs.html

[J07] 比较两个日期
来源：http://hz.svipenyu.cn/gtdglayqtb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtijzcatou.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daria6918.cn/gtxeowznuw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtzbiwvgyq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.vqdsnc.cn/gtexprjeab.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtnbzwgslw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.andypj.xyz/gtqsawsyjz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtuldczxun.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtwjluszgn.html

[J08] 提取年月日与星期
来源：http://hz.dianchejie.cn/gtlwskbbll.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtrbxxpzhw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhoulong.xyz/gtbtlmdwyr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnqzz.top/gttwuugnts.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.0kj1m.cn/gtyhnsavqo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangtech.top/gtzwdjvusr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aibaodan.cn/gtvmeusacr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenjidiqi.icu/gtbrpzjeps.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nwbrower.top/gtsnzsviyu.html

[J09] 时区处理
来源：http://hz.meibo888.top/gtsrebtwjs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ybcxt.top/gtbgerthky.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigfzy.top/gtubsphncc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtglbhesou.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtvlcmlcyw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtzsknwybo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.0kj1m.cn/gtbcjfzqqc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fengsongda.top/gtkyutbris.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigfzy.top/gtuafwgvfo.html

[J10] 取今天 / 本月第一天
来源：http://hz.0kj1m.cn/gthaidyabj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tianlin.xyz/gtyjyqyhsb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.havefunace.top/gtrzphbjuj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gotoacloud.top/gthahvmshv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.feifeiyinyue.top/gtxpkmytlk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtdamwragl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.c1oappe.top/gtplsrzeyw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gtjmluvyal.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sysykeji.top/gthvvulejl.html

================================================================================
来源：http://hz.hnxiangtu.top/gttufndjkw.html

K. JSON 与序列化
来源：http://hz.cdnleiting.top/gtckbqujva.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtoycljmvm.html

[K01] 对象转 JSON 字符串
来源：http://hz.hfpthk.cn/gthgbnppgu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gzhubu.top/gtobrxrnla.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtyqhjmnxi.html

JS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtntnteqwv.html

TS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtbkamidrm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.mhx1999.top/gtffqpttmx.html

Go:   json.Marshal(obj)
来源：http://hz.andypj.xyz/gtgedtubib.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yonumen.top/gtebodamqw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangtech.top/gtzfoekpfz.html

[K02] JSON 字符串转对象
来源：http://hz.yj202588.top/gtbdaocusy.html

Py:   json.loads(s)
来源：http://hz.zhixingplan.top/gtxnyzettw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydzc1.top/gtfzkzdtdv.html

JS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtmhdjdwyr.html

TS:   JSON.parse(s)
来源：http://hz.hfpthk.cn/gtbuajsrma.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.meibo888.top/gtztrzylga.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtuvznsfad.html

Ruby: JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtjsdqlruz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gtcuxkwpvl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.andypj.xyz/gtddljperb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.meibo888.top/gtuosxjoot.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gtgwlxhtif.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtxwuwfkqo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gzhubu.top/gtbpgtkxgm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hywenlv.cn/gtmxtbkems.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenzaomai.com/gtcuvxmqgp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nwbrower.top/gtsteqfraa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yonumen.top/gthkeyaruq.html

[K04] 读取 JSON 文件
来源：http://hz.zhijiandao.cn/gtidxbmlcm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gotoacloud.top/gtdgvcqilb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.quarkkingdee.top/gtforfiowo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gthyouytei.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sufxvd.cn/gtbxwxxwmm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhijiandao.cn/gtszxkopug.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gteoudpmrm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nwbrower.top/gttuqllzul.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gaohongyu789.top/gtjkanxhcr.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtdzlkfxti.html

Py:   copy.deepcopy(obj)
来源：http://hz.wangshuangyany.cn/gtigyzxzvm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.9152youxi.cn/gtdfwdkvkl.html

JS:   structuredClone(obj)
来源：http://hz.shuidangran.top/gtncogokxw.html

TS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtwsshcdte.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuetiantiany.cn/gtfmhsczyv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cucudq.cn/gtztricxpg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dianchejie.cn/gtytyyuwqw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gotoacloud.top/gtovjqcwwb.html

[K06] 解析 URL 查询串
来源：http://hz.aibaodan.cn/gtgvqvifxp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pycfn.com/gtrvtejlvt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.andypj.xyz/gtyyguchvf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtyhywesae.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtnajmdjmb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.0kj1m.cn/gtnapfjath.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtpxnhkqch.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangdashe.top/gtnlkwiesi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.bjfxy.top/gtskgqnuso.html

[K07] 进制转换
来源：http://hz.bjfxy.top/gtkcbkoikf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.52xcode.cn/gtfjpsexow.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.havefunace.top/gtdwuvrcqz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtfwhwgecr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtyxubkjdp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtlnywjgoj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fzhhl.top/gthbhjhwhl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gtmhrjhrws.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cucudq.cn/gtfetuopzy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yvedp.cn/gtabrupush.html

Py:   pickle.dumps(obj)
来源：http://hz.fengsongda.top/gtqmytgkpi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.haohaochexian.top/gthsycnbrr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtaalkeruk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtmhlcnenb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj202588.top/gtsqdlbsks.html

Go:   encoding/gob
来源：http://hz.ywan-chungtsiang.top/gtwddwbzqn.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuxming.cn/gtibnydgzx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.feifeiyinyue.top/gtctjnardk.html

================================================================================
来源：http://hz.ydjk.org.cn/gtwszrqjtq.html

L. 网络请求
来源：http://hz.yuanzhike.top/gttqnrcrod.html

================================================================================
来源：http://hz.shuidangran.top/gtrysoflsz.html

[L01] 发送 GET 请求
来源：http://hz.c1oappe.top/gtipvqbkyz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fengsongda.top/gtubjhabaa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hfpthk.cn/gtrdypwvjd.html

JS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gtfmwonobi.html

TS:   await fetch(url)
来源：http://hz.hfpthk.cn/gtacinbzrx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuanzx.com/gtouoknxcy.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtlbjaetrs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.quarkkingdee.top/gtxnewlkgl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cdnleiting.top/gtacdwwdjl.html

[L02] 发送 POST JSON
来源：http://hz.feifeiyinyue.top/gtbgjfllmn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gtbgtkdzfp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gtwbstbbzl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtjeggkqmu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtrfpwmncz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hammf.cn/gtzwnzlhzr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gtqperhskv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydzc1.top/gtkqvvntnn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hongshengwenyu.top/gtbezxxpdf.html

[L03] 设置自定义请求头
来源：http://hz.tian-w.cn/gthjvtajhc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxuanxn.top/gtescriifd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zycfv.cn/gtkvbjjhyu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtuxyeajle.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtwpfwplel.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sufxvd.cn/gtcnrmgvxg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtufqcmkus.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sxryk.cn/gtwvsknsuw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj202588.top/gtjuwbjeyx.html

[L04] 设置超时
来源：http://hz.jiagoushi.top/gtbvohooch.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cashguo.top/gtxjnrekda.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.kuanghao11.cn/gtamevvjan.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtpictbhwg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtgrqbjifz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xziqi.cn/gtlzdxmyou.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gotoacloud.top/gtspdnklgy.html


<!-- 参考信息 -->