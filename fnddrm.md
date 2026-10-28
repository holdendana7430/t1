代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ivvv.top/gtlufroxeg.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtklaoqghl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinyuanbaomall.cn/gtqlsnyerc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nwbrower.top/gtzygzxmgs.html

================================================================================
来源：http://hz.vqdsnc.cn/gtklmzehub.html

I. 正则表达式
来源：http://hz.feifeiyinyue.top/gtxqntdnql.html

================================================================================
来源：http://hz.yj202588.top/gtifrytfhy.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtqtlwgmwy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shuidangran.top/gtgfhtxzyt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinghuilouyu.cn/gtdyepkomo.html

JS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtsnmuqbav.html

TS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtiyxlxppg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xuanzx.com/gtnpmgsqxw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hongshengwenyu.top/gtbbsgqirc.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtzdkwksea.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sysykeji.top/gtnwbcudhe.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gtglupuzxb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuxming.cn/gtrcnvwzje.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xinyue.icu/gtcjlgetvh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cucudq.cn/gtxcecmehj.html

TS:   s.match(/\d+/g)
来源：http://hz.yvedp.cn/gtkgxmbymw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yangfankeji.com/gtmcjznfqv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hnqzz.top/gtccdfxtnh.html

Ruby: s.scan(/\d+/)
来源：http://hz.ehwqpu.com/gtmomglabj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhiwuduotai.top/gtcypnftxd.html

[I03] 提取捕获分组
来源：http://hz.jinqigfzy.top/gtvuoebuvp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cashguo.top/gtooxnusrk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.fzhhl.top/gtdfkgnkyw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jianghu66.top/gtisfkhwet.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hysaishi.cn/gtoevptyzq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.snrcjt.cn/gtpgxoevqx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gtwdnjiaep.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cashguo.top/gtoczemzjo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtmfyihexm.html

[I04] 正则替换
来源：http://hz.xuanzx.com/gtbisterkj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.iojbl.cn/gtrfomxatj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtnwwzfzmg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtrefpqkxy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtfpudfwtc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gogol.net.cn/gtystopftn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tian-w.cn/gtlhsgmewk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.quarkkingdee.top/gttbxzienf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj202588.top/gtnfpastza.html

[I05] 按正则拆分
来源：http://hz.quarkkingdee.top/gtcdgppamc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.meibo888.top/gtswtjffkp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhiwuduotai.top/gtyyegvhng.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtnxargpft.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtibwrhzti.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hongshengwenyu.top/gturfnaojk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuxming.cn/gtjbaethsg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtntqwuyxl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuanzhike.top/gtxrvppdce.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shangyingyoupin.top/gtpfblczcp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gtsoifddtm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nanxinkj.top/gtsxjucnpy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtodvgqmqk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gttxmbniou.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hammf.cn/gtjbiqqsmu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yanxiufei.cn/gtybhnbfuh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hammf.cn/gtreqaelaq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuxming.cn/gtcgjymdaq.html

[I07] 忽略大小写与多行模式
来源：http://hz.nanxuanxn.top/gtcfinvpji.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinqigfzy.top/gtijwoqqku.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.haohaochexian.top/gtodbstrlj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tanke756.top/gtnqmhdonv.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtzanfxmwi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gtlyreiglz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tian-w.cn/gtvhijwvoe.html

Ruby: s.scan(/error/i)
来源：http://hz.guowangkeji.top/gtanzqlxom.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ywan-chungtsiang.top/gtwofvfozz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gthyunmqrp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.kuanghao11.cn/gtpconlfcy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangdashe.top/gttsjrxebw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gttgwkuaov.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtnkpkufvr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtbswvxkdn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.svipenyu.cn/gtpsegjngy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.smart0.xyz/gtxtelhsgk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xinyue.icu/gtrocgbeth.html

================================================================================
来源：http://hz.c1oappe.top/gtkjcgtncj.html

J. 日期与时间
来源：http://hz.pengpengdd.cyou/gtppvumehv.html

================================================================================
来源：http://hz.dashuyun.cn/gtvhlykxnl.html

[J01] 获取当前时间
来源：http://hz.kuanghao11.cn/gtigrreewc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daxiang520.top/gtlyalhiyt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daxiang520.top/gtrxmiuabs.html

JS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtiefqkrfq.html

TS:   new Date();  Date.now()
来源：http://hz.jyoumei.cn/gtruywqucs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dashuyun.cn/gtrofiptxv.html

Go:   time.Now()
来源：http://hz.redwolf501.top/gtxphmcyzk.html

Ruby: Time.now
来源：http://hz.jyoumei.cn/gtmkchgkrj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhengqikj.top/gtoaapayqs.html

[J02] 格式化输出
来源：http://hz.jinghuilouyu.cn/gtzlomepmp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtibbifpqu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtsisgikoe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sweek.top/gtcwycfgmq.html

TS:   d.toISOString()
来源：http://hz.nanxuanxn.top/gtoqtdwdmq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jyoumei.cn/gtnqczlsyn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.feifeiyinyue.top/gttxnrtalr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtcijtvgqc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.birdmap.top/gtmhbyqkjt.html

[J03] 字符串解析为日期
来源：http://hz.tanke756.top/gtlltyibev.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigfzy.top/gtetomueyz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yonumen.top/gteerdjlnp.html

JS:   new Date("2024-01-02")
来源：http://hz.ehwqpu.com/gtlcwwhoox.html

TS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtykhjiqdn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtjsdfzcic.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ybcxt.top/gtnzsaywrc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtufuytuql.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jianghu66.top/gtdtmhdatc.html

[J04] 时间戳与日期互转
来源：http://hz.kuanghao11.cn/gtlfuwwsvw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.haohaochexian.top/gtokspwozl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sxryk.cn/gthveynsgi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258.top/gtazigqeoy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxuanxn.top/gtnwnppzgu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuxming.cn/gtazqkctau.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhaomingkeji.xyz/gtlsjshfrb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtfhiqhrmp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.andypj.xyz/gtztfpwwsb.html

[J05] 时间加减（加 7 天）
来源：http://hz.tian-w.cn/gtcforaxdk.html

Py:   now + timedelta(days=7)
来源：http://hz.xziqi.cn/gtxzoqkbhi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxinkj.top/gtzkgdcbiy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gtueeoehfz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jyoumei.cn/gtbjiemfti.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hammf.cn/gtqgglgzzb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.birdmap.top/gtfdamsqra.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxinkj.top/gtgsgudpsw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangtech.top/gtewrtapvm.html

[J06] 计算两时间之差
来源：http://hz.yongpay.top/gtbmwqtnwe.html

Py:   (end - start).total_seconds()
来源：http://hz.jyoumei.cn/gtngvxmlgn.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gtdfgscwtl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jlsjyb.cn/gtafzipsfb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtzsnnyrpr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fzhhl.top/gtredwefab.html

Go:   end.Sub(start).Hours()
来源：http://hz.hfpthk.cn/gtndqzxdqe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.316326.xyz/gtoqzklffu.html

C#:   (end - start).TotalSeconds
来源：http://hz.xingfuxueyuan.xyz/gtjalvrzuy.html

[J07] 比较两个日期
来源：http://hz.cqqwz.cn/gthevtkkpg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtznbjyycc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenjidiqi.icu/gtvkwymzft.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtmlhcyuwy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtjjjhodwf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.bjfxy.top/gtvwlpcrrj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gotoacloud.top/gtcvazrkko.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gthjeckfad.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtnvihxbtn.html

[J08] 提取年月日与星期
来源：http://hz.redwolf501.top/gtaoiyoiqe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daria6918.cn/gthmqctosr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinghuilouyu.cn/gtejwehhqx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj202588.top/gtfsojysjq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gzhubu.top/gtxkocyzja.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.andypj.xyz/gtpugwthmm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258.top/gtiuuvylut.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cqqwz.cn/gtwdyjfqug.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.havefunace.top/gtqztorxii.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtqsfoohkp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sxryk.cn/gtzducngqr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuetiantiany.cn/gtioasoaiq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gtdmgobdqp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gtcfhotabx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.iojbl.cn/gtpjstlemh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shangyingyoupin.top/gtfismzrxz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aibaodan.cn/gtzerwmflj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sweek.top/gtuatirghp.html

[J10] 取今天 / 本月第一天
来源：http://hz.svipenyu.cn/gtmhkgycwl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cucudq.cn/gtgevekucw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sxryk.cn/gttdzgjora.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnqzz.top/gtqomytwup.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zdqjudy.top/gtqlsouqtf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenjidiqi.icu/gtesjjkjxz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nwbrower.top/gtmmowqrrk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hongshengwenyu.top/gtciksqyie.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hfpthk.cn/gtqiroeoga.html

================================================================================
来源：http://hz.ybcxt.top/gtlbekmsui.html

K. JSON 与序列化
来源：http://hz.shangyingyoupin.top/gthuvsxmto.html

================================================================================
来源：http://hz.zhixingplan.top/gtmzzplago.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenzaomai.com/gtnqrngoof.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtjhvrbwrw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gtiygnvike.html

JS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtajzoydtj.html

TS:   JSON.stringify(obj)
来源：http://hz.dashuyun.cn/gtmmufhxum.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cheryme.top/gtyulyiaob.html

Go:   json.Marshal(obj)
来源：http://hz.jinghuilouyu.cn/gtghcbcaax.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.havefunace.top/gtbapsvbqi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gogol.net.cn/gtujajgojp.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtiztvyvim.html

Py:   json.loads(s)
来源：http://hz.zhoulong.xyz/gtlbeedmwx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhoulong.xyz/gtycqcunbd.html

JS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtjbsdgpoe.html

TS:   JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtqufqwcql.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.9152youxi.cn/gtarjnuczw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yuxming.cn/gtxsutmjgq.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gteeeseouy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zdqjudy.top/gtqcczvjaa.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtzdvcelzg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cqqwz.cn/gtwrfnsuog.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtefamhbvk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xziqi.cn/gtszicdjzb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtzhzfmxlz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj202588.top/gtfpkyslxv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tanke756.top/gtsxbdeyrn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj202588.top/gtfbknysbu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.redwolf501.top/gtdvqmazbt.html

[K04] 读取 JSON 文件
来源：http://hz.hongshengwenyu.top/gtzopvnhvg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hfpthk.cn/gtlhvjwiur.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.c1oappe.top/gtkxratqht.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gtvwplpbqg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydjk.org.cn/gtswznlrln.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xziqi.cn/gtttcxdqqe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtnriubapp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fzhhl.top/gtakeifxzb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xinyue.icu/gtrwtntttg.html

[K05] 深拷贝对象
来源：http://hz.yuanzhike.top/gttmktswfm.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhengqikj.top/gtixredqhi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hfpthk.cn/gtpdcbcozr.html

JS:   structuredClone(obj)
来源：http://hz.meibo888.top/gthjkobogi.html

TS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtxanhxypa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gotoacloud.top/gtyrfnhdgv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jyoumei.cn/gtzyyzivbq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtueocnqxb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenlongwang.top/gtbbkoddiq.html

[K06] 解析 URL 查询串
来源：http://hz.chenlongwang.top/gtdpurhfop.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhengqikj.top/gtkmeindtt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ppjwa.cn/gtymjsrkzf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtdttvekdq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gzhubu.top/gtztgqshrq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yonumen.top/gtlhndxuqn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gaohongyu789.top/gttwmuvunq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtzfkhjmjs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hysaishi.cn/gtgwwiiwnz.html

[K07] 进制转换
来源：http://hz.kuanghao11.cn/gtqzjxkklp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hywenlv.cn/gtxlntpmor.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258.top/gtkuljxgwk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtulgauaiv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtaowjbkpz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtqigzlnpp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydzc1.top/gtjzlcdmql.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.snrcjt.cn/gtkdhoejro.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuanzx.com/gttdujpfyk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.0kj1m.cn/gttqqwrimm.html

Py:   pickle.dumps(obj)
来源：http://hz.haohaochexian.top/gtwzzfqoqd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nanxuanxn.top/gtttwufwvz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhiwuduotai.top/gtadpakymh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gtybzvbfts.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tianlin.xyz/gtfeapzeqx.html

Go:   encoding/gob
来源：http://hz.hongshengwenyu.top/gtxllizdlq.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinghuilouyu.cn/gtgaquiscd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sweek.top/gttllowejt.html

================================================================================
来源：http://hz.jianghu66.top/gtzykfcftf.html

L. 网络请求
来源：http://hz.zhengqikj.top/gttxrdqiip.html

================================================================================
来源：http://hz.yj20258888.top/gtsamvemwb.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtzlrezpzj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinyuanbaomall.cn/gtepjulkga.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gaohongyu789.top/gtmlgqbnwj.html

JS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtferjfkfo.html

TS:   await fetch(url)
来源：http://hz.zhixingplan.top/gtmopijllj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guowangkeji.top/gtnlgtgdhv.html

Go:   resp, err := http.Get(url)
来源：http://hz.jlsjyb.cn/gtrivitorc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pycfn.com/gtxvfenkib.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuanzhike.top/gtytghyjtu.html

[L02] 发送 POST JSON
来源：http://hz.ybcxt.top/gtdmhtbawl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.0kj1m.cn/gtqydofwud.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xinyue.icu/gtzzfurpka.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtcvrmgate.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtbvgvrsvu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ywan-chungtsiang.top/gtsvwmtbfm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daria6918.cn/gtvkxmejln.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.birdmap.top/gtvrcuxewi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxinkj.top/gtfxdzqsau.html

[L03] 设置自定义请求头
来源：http://hz.zhengqikj.top/gtilubnxja.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgufenzy.top/gtymnsgkxf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.quarkkingdee.top/gtxtgwzkaw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtapkwmwmp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gthelntish.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aibaodan.cn/gtpoayysqm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cdnleiting.top/gttemnxqea.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ywan-chungtsiang.top/gtmfqdqabb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.guowangkeji.top/gtsngufpfg.html

[L04] 设置超时
来源：http://hz.xylfe.cn/gtjtixwqfw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangdashe.top/gtoceibirv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gtrtmcwdma.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtegmepqph.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtxfpisfbl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yvedp.cn/gtglukdlfm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pengpengdd.cyou/gtlenktsie.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydjk.org.cn/gtwyhgzhmd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgfzy.top/gtuhutkuxf.html

[L05] 上传文件（multipart）
来源：http://hz.xinyue.icu/gtvlamfsdg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cdnleiting.top/gthhwnmwbk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.iojbl.cn/gtoylhnsto.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtypzugkau.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtinpipnlz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhongyouzk.top/gtxpqlfkgo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aizwys.cn/gthndxkmbg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hammf.cn/gtphrdikpc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daria6918.cn/gttkjwcicu.html

[L06] 解析响应为 JSON
来源：http://hz.cucudq.cn/gtzzyccjrx.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtbyacsneb.html

PHP:  json_decode($body, true);
来源：http://hz.snrcjt.cn/gtbalpqthy.html

JS:   await resp.json()
来源：http://hz.vqdsnc.cn/gtblbbdgat.html

TS:   await resp.json()
来源：http://hz.snrcjt.cn/gtvlzmqcpw.html


<!-- 参考信息 -->