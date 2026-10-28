代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nanxinkj.top/gtqquhovuk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daxiang520.top/gtfwfanvty.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shangyingyoupin.top/gtzngvejyh.html

C#:   obj?.A?.B ?? default
来源：http://hz.gogol.net.cn/gtjyjitmag.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gtvhpsmoly.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhixingplan.top/gtcnwekcju.html

PHP:  assert($x > 0);
来源：http://hz.yj202588.top/gthtagphkw.html

JS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtiscmeomr.html

TS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtrtbtpqku.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuetiantiany.cn/gtitipyngl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shzxlz.cn/gtgqqpalqv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtlodguues.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtonysuqbo.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258.top/gtsalvyeis.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.havefunace.top/gtzjetrpmm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.meibo888.top/gtkpbhffjn.html

JS:   e.message;  e.stack
来源：http://hz.yvedp.cn/gtzmtqpntj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gthqtvnhfp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.kuanghao11.cn/gtodnajlwy.html

Go:   err.Error()
来源：http://hz.tian-w.cn/gtxpvzdwsi.html

Ruby: e.message;  e.backtrace
来源：http://hz.daria6918.cn/gtusgtlllp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.havefunace.top/gtftyrsonc.html

[H09] 带错误码的异常
来源：http://hz.zdqjudy.top/gtmryxjcrk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhoulong.xyz/gtilflyrfr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangkeji.top/gtoomfspbp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.iojbl.cn/gtwhdyrtpp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xylfe.cn/gttofpjted.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxuanxn.top/gtjqajgvtm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.52xcode.cn/gtoqhrplzq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daria6918.cn/gtexlqagpc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydjk.org.cn/gtishfupnb.html

[H10] 资源自动释放
来源：http://hz.gzhubu.top/gtazqxqmtv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cheryme.top/gteszhtasq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cheryme.top/gtjedtfngd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtzasraznq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yangfankeji.com/gtibftfnii.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenjidiqi.icu/gtnagkxfox.html

Go:   defer f.Close()
来源：http://hz.nanxinkj.top/gttlakickn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenlongwang.top/gtwetsmaub.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gtsqsneclx.html

================================================================================
来源：http://hz.zhongyouzk.top/gtxgblkwcn.html

I. 正则表达式
来源：http://hz.hongshengwenyu.top/gtxhdiorws.html

================================================================================
来源：http://hz.ehwqpu.com/gtxdygmxhj.html

[I01] 判断是否匹配
来源：http://hz.chenlongwang.top/gtcesndzzw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ivvv.top/gtandpyaqs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenlongwang.top/gtnlkccydt.html

JS:   /\d+/.test(s)
来源：http://hz.tian-w.cn/gtjpqelesp.html

TS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gtvkjothzp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenjidiqi.icu/gtnmrpzznj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cdnleiting.top/gtrlihymus.html

Ruby: s.match?(/\d+/)
来源：http://hz.316326.xyz/gtytewpiwm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cheryme.top/gtrbuumoxx.html

[I02] 提取所有匹配
来源：http://hz.cashguo.top/gttypxegsd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.52xcode.cn/gtcwwraqhv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.iojbl.cn/gthnacyedy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.kuanghao11.cn/gtnstewblj.html

TS:   s.match(/\d+/g)
来源：http://hz.hongshengwenyu.top/gtrehpuxqf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj202588.top/gtnclkgxqe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gogol.net.cn/gtajoptpkb.html

Ruby: s.scan(/\d+/)
来源：http://hz.gogol.net.cn/gtpouaqqdg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.iojbl.cn/gttvlwgpgn.html

[I03] 提取捕获分组
来源：http://hz.cqqwz.cn/gtmjfmtlba.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hammf.cn/gtwsbkczwi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zdqjudy.top/gtjdbberwp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gaohongyu789.top/gtsjdssdof.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gzhubu.top/gtogvumkem.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shuidangran.top/gtqjvugrty.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yonumen.top/gtsyxiofgm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.andypj.xyz/gtyrervnyc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sysykeji.top/gtvgzfwrse.html

[I04] 正则替换
来源：http://hz.jlsjyb.cn/gtdwnbtepm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gtbommjrhk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuxming.cn/gtrpansqwi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtefgqjjkd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtymbautbv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.vqdsnc.cn/gtxyreanoi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.redwolf501.top/gtaekwkgkw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtxhtxobqx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sxryk.cn/gtdzgorxow.html

[I05] 按正则拆分
来源：http://hz.haohaochexian.top/gtrrosmjix.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.daria6918.cn/gtrgucrczh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jyoumei.cn/gtzzcnmxbg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gthdtquqwr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtjssxfcdc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.52xcode.cn/gtptqnlspe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aizwys.cn/gtfxzvqlcr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtzvwwxvgx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gzhubu.top/gtzpnhnzow.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhongyouzk.top/gtqqtrjzry.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtnczishxc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pengpengdd.cyou/gtovwuhucq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.quarkkingdee.top/gtskbovvhx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hammf.cn/gtntricqgu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aizwys.cn/gtueehdlwj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nwbrower.top/gtsdgcwojz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgufenzy.top/gtpcqhcsld.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tanke756.top/gtoxbaaosi.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtjszgjgmj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xuetiantiany.cn/gtaxjalqfe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cqqwz.cn/gthpvrbtiw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cqqwz.cn/gtnnawrlbw.html

TS:   /error/gim
来源：http://hz.jiagoushi.top/gtrexpgygp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.c1oappe.top/gthebxknbe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.guowangkeji.top/gtbjvfimfc.html

Ruby: s.scan(/error/i)
来源：http://hz.tianlin.xyz/gtmjyerxro.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yonumen.top/gtytvzkjew.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cashguo.top/gtsnfeoyxo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yanxiufei.cn/gtswrmxcrx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ivvv.top/gtxqfngrtc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxuanxn.top/gtlcngwqsi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtxmhxstoo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tanke756.top/gtmeuvqxea.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.smart0.xyz/gtbehfkgdn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shuidangran.top/gtyvuqgihp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ydjk.org.cn/gtaqqsabgc.html

================================================================================
来源：http://hz.jlsjyb.cn/gtsygsfuit.html

J. 日期与时间
来源：http://hz.daria6918.cn/gtvapcyiwc.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtfhhwdwos.html

[J01] 获取当前时间
来源：http://hz.hfpthk.cn/gthozpkybq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xingfuxueyuan.xyz/gtqqqhhgjc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtttwusebe.html

JS:   new Date();  Date.now()
来源：http://hz.daria6918.cn/gtuxnixtfd.html

TS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtbmfwcsta.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnqzz.top/gttultiura.html

Go:   time.Now()
来源：http://hz.zhiwuduotai.top/gtmntlqeut.html

Ruby: Time.now
来源：http://hz.shanyushiyangtech.top/gtmhonvkio.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.fengsongda.top/gtnlfdifxh.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtfcacywww.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gteeffbvdp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtvwemzxjr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tian-w.cn/gtuqnidwky.html

TS:   d.toISOString()
来源：http://hz.shangyingyoupin.top/gtidoqubcw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.birdmap.top/gtyuoioomc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dashuyun.cn/gtfbqucrqc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtmcjbmrbp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cashguo.top/gtbrycvavy.html

[J03] 字符串解析为日期
来源：http://hz.redwolf501.top/gtpuxokkfm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xylfe.cn/gthvmumfbs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daria6918.cn/gtqnmrjquu.html

JS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtijjqrfet.html

TS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtdlsomojf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtiavysiup.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigfzy.top/gtmocpjloq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtzmagdfnw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnqzz.top/gtwuyyhcmh.html

[J04] 时间戳与日期互转
来源：http://hz.nanxuanxn.top/gtrvyqbonj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ppjwa.cn/gtuyrfdhec.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.vqdsnc.cn/gtprghkrkx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydjk.org.cn/gtyzxxuipa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xziqi.cn/gtnihqjrsm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhengqikj.top/gtttxdtvqo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuanzhike.top/gtgatbmgyo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xinyue.icu/gtdoyejztb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinghuilouyu.cn/gtcrtrcqkp.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258.top/gtokuouekj.html

Py:   now + timedelta(days=7)
来源：http://hz.0kj1m.cn/gtxhgrqxai.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cqqwz.cn/gtkbwtoigh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gtbwxrlxhx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgfzy.top/gtyryvmrlv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.haohaochexian.top/gtribiktpq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.feifeiyinyue.top/gtfgdlsqeu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnqzz.top/gtugmygajc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jianghu66.top/gtxmxiperk.html

[J06] 计算两时间之差
来源：http://hz.vqdsnc.cn/gttdkyoqre.html

Py:   (end - start).total_seconds()
来源：http://hz.sxryk.cn/gtdsasigcr.html

PHP:  $end->diff($start)->days;
来源：http://hz.c1oappe.top/gtolqdlcip.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenjidiqi.icu/gtantsafpp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhoulong.xyz/gtgcmqusnh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sweek.top/gtmxuavquf.html

Go:   end.Sub(start).Hours()
来源：http://hz.xinyue.icu/gtalcgkdzq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.havefunace.top/gttsvfufjh.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhengqikj.top/gtnzrmszgy.html

[J07] 比较两个日期
来源：http://hz.fzhhl.top/gtsncmzywq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtgxaaoqud.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydjk.org.cn/gtakopswwd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtxuisajtt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtigxuotyj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gtpekstmpc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnxiangtu.top/gtdqihhqif.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtljgzzucz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtirlupkdh.html

[J08] 提取年月日与星期
来源：http://hz.jqgufenzy.top/gtnrxpebql.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj202588.top/gtctwuuxbl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gtwqqwavuc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangkeji.top/gtmdozwzzh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.birdmap.top/gtipwjbwmv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hongshengwenyu.top/gthmvasdwi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhengqikj.top/gtrrmisqdj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhaomingkeji.xyz/gtvaojqjic.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hnxiangtu.top/gtyzyqvnzd.html

[J09] 时区处理
来源：http://hz.cheryme.top/gtxucdgqsc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jlsjyb.cn/gtxomprckc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hywenlv.cn/gtbqxlmnvy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtpywxuqpk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtrebtgxtt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cheryme.top/gtynjocmug.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aibaodan.cn/gthnsbpoxm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shzxlz.cn/gtujjtdwoy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shangyingyoupin.top/gteqgygvaq.html

[J10] 取今天 / 本月第一天
来源：http://hz.daria6918.cn/gtzfyuinrd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258.top/gtzxhyqdpk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pengpengdd.cyou/gtviwdwvfc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxinkj.top/gtgsrtdpgz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangshuangyany.cn/gtcdlkkwak.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.fzhhl.top/gtslcidzwp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnxiangtu.top/gtrwqvhhju.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aibaodan.cn/gticbqmpyg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgufenzy.top/gtmazuhyst.html

================================================================================
来源：http://hz.zhijiandao.cn/gttusmftum.html

K. JSON 与序列化
来源：http://hz.xylfe.cn/gteqlgcnzn.html

================================================================================
来源：http://hz.cqqwz.cn/gthfdalohj.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangshuangyany.cn/gtbqbultbb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtlqtnqhhv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gttdvbates.html

JS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtjyinowwi.html

TS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtaxeztztl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hywenlv.cn/gtrjmenifp.html

Go:   json.Marshal(obj)
来源：http://hz.shzxlz.cn/gthifcqagc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guannengcc.top/gthxbkxvvo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ppjwa.cn/gtkmeueohb.html

[K02] JSON 字符串转对象
来源：http://hz.svipenyu.cn/gtbrdglvdf.html

Py:   json.loads(s)
来源：http://hz.zhaomingkeji.xyz/gtkkbkqtdc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.bjfxy.top/gttoovdssh.html

JS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gthzrudxza.html

TS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtrbaxrqpg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pengpengdd.cyou/gtioeqpise.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtwqcbiutb.html

Ruby: JSON.parse(s)
来源：http://hz.birdmap.top/gttjapmfmz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sxryk.cn/gtppjlcrxn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yonumen.top/gtdhdfyquq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtebcwptho.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtglamfcbq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtofgqjakx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtlpinxnvi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gthzetjwam.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhoulong.xyz/gtozlrgtut.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dashuyun.cn/gtzbgeoooz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhixingplan.top/gthmmruyis.html

[K04] 读取 JSON 文件
来源：http://hz.bjfxy.top/gtlkkbgply.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gogol.net.cn/gtbsjgxggg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guannengcc.top/gtehretcxb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtguzlakqo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtatovzxbz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jqgufenzy.top/gtijujqovv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cqqwz.cn/gtodpdvojk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgfzy.top/gtykpvectk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jqgfzy.top/gtkofmkdse.html

[K05] 深拷贝对象
来源：http://hz.chenlongwang.top/gtgzsxzknu.html

Py:   copy.deepcopy(obj)
来源：http://hz.shuidangran.top/gtpqmcgcah.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhijiandao.cn/gtiiktmtgd.html

JS:   structuredClone(obj)
来源：http://hz.gzhubu.top/gtmfiactxg.html

TS:   structuredClone(obj)
来源：http://hz.yonumen.top/gteirovmdc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gtfwbuaqta.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.wangshuangyany.cn/gtexhlewhl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.birdmap.top/gtllkkfofi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sweek.top/gtmcqfdniz.html

[K06] 解析 URL 查询串
来源：http://hz.bjfxy.top/gtxnjfzvsb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hysaishi.cn/gtfnastcdi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinyuanbaomall.cn/gtwyukhknf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtdfvmsggs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtndfharpp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinyuanbaomall.cn/gtxcyhahhr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gtrerjtdyn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgfzy.top/gtytjjhyys.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tianlin.xyz/gtmgjegbmo.html

[K07] 进制转换
来源：http://hz.zhixingplan.top/gtfsqbtznl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxuanxn.top/gthtzhvdhj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gogol.net.cn/gtxahyiywt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtcgkmyxyu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtviwtdtpc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtbkzsyeml.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yonumen.top/gtbvurzovh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jianghu66.top/gtpxubvcur.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.mhx1999.top/gtmiwnygdh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.andypj.xyz/gtmdjukyif.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gtuzljfkss.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hnqzz.top/gtimkzmboj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtpqvossaf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tianlin.xyz/gtgxoajald.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ybcxt.top/gtegdqvpee.html

Go:   encoding/gob
来源：http://hz.gogol.net.cn/gtxdncwbir.html

Ruby: Marshal.dump(obj)
来源：http://hz.shuidangran.top/gtvlbrvbhi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuetiantiany.cn/gtzultwmbp.html

================================================================================
来源：http://hz.yanxiufei.cn/gttubzugfy.html

L. 网络请求
来源：http://hz.52xcode.cn/gtwclxoiub.html

================================================================================
来源：http://hz.sufxvd.cn/gtlbfqbojg.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gtvtoovjhe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xingfuxueyuan.xyz/gtkikihoog.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sufxvd.cn/gtsrmustwe.html

JS:   await fetch(url)
来源：http://hz.zdqjudy.top/gtpvwfpebf.html

TS:   await fetch(url)
来源：http://hz.gzhubu.top/gtepkgfcpx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.svipenyu.cn/gtjjqfcepl.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhiwuduotai.top/gtdynnnbuu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.quarkkingdee.top/gtqepklqqm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.andypj.xyz/gtycuqpmju.html

[L02] 发送 POST JSON
来源：http://hz.cheryme.top/gtgfjcxccp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtxpowinid.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aizwys.cn/gtmrmylbqi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtbmcuqekf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtpcwfmman.html


<!-- 参考信息 -->