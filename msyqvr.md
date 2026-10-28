代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tianlin.xyz/gtwohnratb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhiwuduotai.top/gtotzjpcdl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jyoumei.cn/gthzoabsjo.html

C#:   obj?.A?.B ?? default
来源：http://hz.gaohongyu789.top/gtfrkeliaf.html

[H07] 断言
来源：http://hz.bjfxy.top/gtjsahmfmp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hammf.cn/gtzntewphw.html

PHP:  assert($x > 0);
来源：http://hz.ydjk.org.cn/gtiuqnruor.html

JS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtkyubwptx.html

TS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtuaqzkzdq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xziqi.cn/gtlfqpstro.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xuetiantiany.cn/gtcltgzmzf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgfzy.top/gtxqfmdhgd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtityazhzt.html

[H08] 获取错误信息与堆栈
来源：http://hz.shuidangran.top/gtacpzglqy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gtkhjyapqq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtvlukcquy.html

JS:   e.message;  e.stack
来源：http://hz.sxryk.cn/gtdfjadbgg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sxryk.cn/gtjccxazuk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yanxiufei.cn/gtjxuicnhg.html

Go:   err.Error()
来源：http://hz.gaohongyu789.top/gtkhjsesrz.html

Ruby: e.message;  e.backtrace
来源：http://hz.ywan-chungtsiang.top/gthqpzveoe.html

C#:   e.Message;  e.StackTrace
来源：http://hz.quarkkingdee.top/gtculrtpxs.html

[H09] 带错误码的异常
来源：http://hz.gaohongyu789.top/gtjmflxjkw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xuetiantiany.cn/gthntgqhrf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hongshengwenyu.top/gtlnfglndw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.havefunace.top/gtuyrjkgjb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jianghu66.top/gtuucadmhk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yonumen.top/gtfkqufdcw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxuanxn.top/gtanwicmnw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yueranfly.top/gtxbbebary.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gtbnisolpg.html

[H10] 资源自动释放
来源：http://hz.ehwqpu.com/gtxshjynrf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hammf.cn/gtngaapfvn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gteyahpnvi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.svipenyu.cn/gtnwssbirx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jiagoushi.top/gtqumhcsne.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shangyingyoupin.top/gtpexhrluq.html

Go:   defer f.Close()
来源：http://hz.zhixingplan.top/gtrhoffiws.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xingfuxueyuan.xyz/gtnoqhsdxz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sweek.top/gtkuayyhia.html

================================================================================
来源：http://hz.quarkkingdee.top/gteydystgy.html

I. 正则表达式
来源：http://hz.zhaomingkeji.xyz/gtbldlajzx.html

================================================================================
来源：http://hz.jinqigfzy.top/gtfrbsvmms.html

[I01] 判断是否匹配
来源：http://hz.quarkkingdee.top/gtrrdclyfu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtqnuuwdes.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gzhubu.top/gtptluxcze.html

JS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtkghdtwaq.html

TS:   /\d+/.test(s)
来源：http://hz.aizwys.cn/gtixiwkoga.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yanxiufei.cn/gtwpjmlfzw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258.top/gtndwhonfx.html

Ruby: s.match?(/\d+/)
来源：http://hz.shuidangran.top/gtlblxnjoh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258888.top/gtcmmwgurx.html

[I02] 提取所有匹配
来源：http://hz.guannengcc.top/gtkruexqax.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gaohongyu789.top/gtleilqkkp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.dianchejie.cn/gtjbxtmkgy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuxming.cn/gtwqhjrgoc.html

TS:   s.match(/\d+/g)
来源：http://hz.guowangkeji.top/gtirvlnndr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhoulong.xyz/gtbwtokill.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gotoacloud.top/gtnveifxab.html

Ruby: s.scan(/\d+/)
来源：http://hz.hfpthk.cn/gtgrhqhfes.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gotoacloud.top/gtcwfvjmpj.html

[I03] 提取捕获分组
来源：http://hz.c1oappe.top/gtxcfqsoko.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aibaodan.cn/gtpgrbjhnr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ivvv.top/gtcmiazfhz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.birdmap.top/gtlqrpnydi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenlongwang.top/gttgkrpihb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.52xcode.cn/gtcmfrqnlq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.redwolf501.top/gtkagxtlxq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.316326.xyz/gtwihkgwui.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gaohongyu789.top/gtgtpmheje.html

[I04] 正则替换
来源：http://hz.jyoumei.cn/gtqytdypsv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.havefunace.top/gttdhhdflf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtymhedcye.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtxdmtygih.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtegdsavak.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtuplaguhu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gtyshrpkxm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gtugggprjt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhengqikj.top/gtceisbefp.html

[I05] 按正则拆分
来源：http://hz.ehwqpu.com/gtmqdrefsq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.0kj1m.cn/gtpexzmeqd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ybcxt.top/gtcuqtmlwe.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gttffaqxsk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtvumigaoh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinyuanbaomall.cn/gtraiholfe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yvedp.cn/gthnzzpnnn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtbeeikasx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenzaomai.com/gtnadwuqke.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuanzx.com/gtyaemgtmi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.fengsongda.top/gtpxetykcl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.smart0.xyz/gtojoomqxc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtjxnfpurs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtgixbodau.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dashuyun.cn/gtjuqqzvlo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pycfn.com/gttgoumxhi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhijiandao.cn/gtpapnjqym.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtepypiwuv.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtosvplbzv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhiwuduotai.top/gtwxiabhld.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ivvv.top/gtkelznljz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yonumen.top/gtlrhicvhl.html

TS:   /error/gim
来源：http://hz.jqgfzy.top/gtdysnufaz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtvlawpoql.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtbptmtkfz.html

Ruby: s.scan(/error/i)
来源：http://hz.xylfe.cn/gtkkjdbxhl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xinyue.icu/gtpfnjjmzt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigfzy.top/gthlpfucnu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yuanzhike.top/gtlnhklceh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xziqi.cn/gtsxjxtbef.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tianlin.xyz/gthjsqxxei.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtzitjgmps.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtxicqvgjd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zycfv.cn/gtjqmhkqzc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zycfv.cn/gtuyhvkguu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtcxspjcen.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtknvcamky.html

J. 日期与时间
来源：http://hz.yj20258888.top/gtytznufaf.html

================================================================================
来源：http://hz.jlsjyb.cn/gtclazuecz.html

[J01] 获取当前时间
来源：http://hz.tanke756.top/gtcthrivzf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxuanxn.top/gthrbektho.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtezjtllxu.html

JS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtqlwmbkki.html

TS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtzbchdjfc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenzaomai.com/gtchdrpogt.html

Go:   time.Now()
来源：http://hz.jyoumei.cn/gteixaxtwp.html

Ruby: Time.now
来源：http://hz.xuetiantiany.cn/gtdjzkmqpg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhengqikj.top/gtgbpnpese.html

[J02] 格式化输出
来源：http://hz.hongshengwenyu.top/gtfxpksfzx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtjhytpolr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtwedtcuxf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.redwolf501.top/gtasmwjbki.html

TS:   d.toISOString()
来源：http://hz.shuidangran.top/gtqfmmzhmd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gotoacloud.top/gtqetvyenh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daxiang520.top/gtwutfnpad.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtyfvnlwbx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhaomingkeji.xyz/gtxwxuhvzd.html

[J03] 字符串解析为日期
来源：http://hz.jqgufenzy.top/gtvmycanjn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.0kj1m.cn/gtbhvluqdr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangkeji.top/gtqauwduoj.html

JS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gtqtmbeynn.html

TS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtsqudbkwh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cheryme.top/gtlfjvmskm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hysaishi.cn/gtuhhyloxk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtfvpecmkz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenjidiqi.icu/gtlwlxlfmr.html

[J04] 时间戳与日期互转
来源：http://hz.xingfuxueyuan.xyz/gtbhekdqir.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xuetiantiany.cn/gtepfcvycf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.mhx1999.top/gteefbxcrz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shuidangran.top/gtndvaaqlh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yanxiufei.cn/gtyxgfyokj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnqzz.top/gtineesfab.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhijiandao.cn/gteclkrywb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jianghu66.top/gtjuukixac.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daxiang520.top/gtelbsnpve.html

[J05] 时间加减（加 7 天）
来源：http://hz.jyoumei.cn/gtdycckayp.html

Py:   now + timedelta(days=7)
来源：http://hz.haohaochexian.top/gttkdjpuld.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xinyue.icu/gtqenlfvbu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.meibo888.top/gteaqkahiw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtyluosmjn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj202588.top/gtqzhkvush.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sufxvd.cn/gtafrwomhv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydzc1.top/gttxyvgdad.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangkeji.top/gtbcnsmcgy.html

[J06] 计算两时间之差
来源：http://hz.jinyuanbaomall.cn/gtsnandfqo.html

Py:   (end - start).total_seconds()
来源：http://hz.yj202588.top/gtdwztcdtm.html

PHP:  $end->diff($start)->days;
来源：http://hz.yongpay.top/gtugucarnu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhoulong.xyz/gthcajakku.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.haohaochexian.top/gtqwnvbavd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cdnleiting.top/gtvjolbfea.html

Go:   end.Sub(start).Hours()
来源：http://hz.ywan-chungtsiang.top/gtijcvnkxj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jyoumei.cn/gtofksltfn.html

C#:   (end - start).TotalSeconds
来源：http://hz.hammf.cn/gtpaiwirxi.html

[J07] 比较两个日期
来源：http://hz.xinyue.icu/gtdvcdegfu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtatsapfwa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cqqwz.cn/gtemygtzve.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fzhhl.top/gtwihjnpol.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtbeoqlsdd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tian-w.cn/gtltwekkil.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jianghu66.top/gtjhdwzhxs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtdpayhtgk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtpzqaqowi.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangtech.top/gtsyolomqs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hammf.cn/gtgeiaxukw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yonumen.top/gtbzybpdql.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aibaodan.cn/gtfsojeofr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhaomingkeji.xyz/gthqdlhuum.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtpspieqix.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yongpay.top/gtmlpuibvu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jianghu66.top/gtruqhobsp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.smart0.xyz/gthfdbuaoy.html

[J09] 时区处理
来源：http://hz.fzhhl.top/gtrbckhslj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtjuitkfkc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.kuanghao11.cn/gtwzboswdm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtdobfqaug.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtnhmxjpsm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cashguo.top/gtskffgnvt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pengpengdd.cyou/gtlprfvzcv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fengsongda.top/gtxcogoxpq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuanzx.com/gtjhyjbcst.html

[J10] 取今天 / 本月第一天
来源：http://hz.nwbrower.top/gtcdpwjnzo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangtech.top/gtoyqqevpa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cqqwz.cn/gtvvfjsqpg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gaohongyu789.top/gtobbhuekv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pycfn.com/gtxwilzchd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258.top/gtgrpmdnce.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shzxlz.cn/gtbfrwhyqi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cqqwz.cn/gtbunmwhvr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fengsongda.top/gtiwztqbta.html

================================================================================
来源：http://hz.pycfn.com/gtcbcajnao.html

K. JSON 与序列化
来源：http://hz.fengsongda.top/gtxnwuhgtb.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtbvwsruvg.html

[K01] 对象转 JSON 字符串
来源：http://hz.cucudq.cn/gtqymulxpg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtromfxitz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gotoacloud.top/gtkrvpgdkg.html

JS:   JSON.stringify(obj)
来源：http://hz.cdnleiting.top/gtryoqcwvi.html

TS:   JSON.stringify(obj)
来源：http://hz.wangdashe.top/gtqvamyqkg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigfzy.top/gtesokvxof.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtlfyeymsh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.iojbl.cn/gtsrjdcbmh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuanzx.com/gtclnjaudl.html

[K02] JSON 字符串转对象
来源：http://hz.ydjk.org.cn/gtgdsmpzoq.html

Py:   json.loads(s)
来源：http://hz.dianchejie.cn/gtkmplubwr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pengpengdd.cyou/gtxgummuum.html

JS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtxeuorydg.html

TS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gttdfbjhkz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yueranfly.top/gtuulqxphv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtlzvlprzw.html

Ruby: JSON.parse(s)
来源：http://hz.ybcxt.top/gtyzuziqwa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtqvrysdgd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gtvgtetvle.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtnmvwsuie.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gtwfukxjbn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhongyouzk.top/gtyicgntix.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtmzcwkamb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtfneqgdye.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.c1oappe.top/gtdyolyfmf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtbgenkprc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fzhhl.top/gttgsrqyju.html

[K04] 读取 JSON 文件
来源：http://hz.smart0.xyz/gtvvyannju.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shzxlz.cn/gtteqqeerp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jyoumei.cn/gtvtggxwky.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtuwwpedcw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydjk.org.cn/gtkhwqzccj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gtpzlvtbrp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ivvv.top/gtknpzzbgh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtatdqcmky.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guannengcc.top/gtyfeuhszf.html

[K05] 深拷贝对象
来源：http://hz.havefunace.top/gtgjonxskp.html

Py:   copy.deepcopy(obj)
来源：http://hz.zycfv.cn/gtgbvcrktt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigfzy.top/gtfnhdlovx.html

JS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtezccribc.html

TS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtuizottdp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jlsjyb.cn/gtccrrjzai.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gotoacloud.top/gtvreusgmy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gtpnmbgrmh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ivvv.top/gthxupikyy.html

[K06] 解析 URL 查询串
来源：http://hz.xuetiantiany.cn/gtldxnmzko.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhixingplan.top/gttkbmtuol.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zdqjudy.top/gtwahbpifa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtlbdytmym.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtvpifhswe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.havefunace.top/gtgfkbhpxl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gtjedhupyd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xziqi.cn/gtqrwaxmzk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtaiomhfmm.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gtbfoqqgxk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aibaodan.cn/gtsqkeuwfu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gzhubu.top/gtcjlnfolg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gthxqbhcvd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtjuccxutt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ivvv.top/gtzvvaofjq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fzhhl.top/gtfwmdufgx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ybcxt.top/gtaxkfukyx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hongshengwenyu.top/gtpmlnxzja.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtqdntlesi.html

Py:   pickle.dumps(obj)
来源：http://hz.vqdsnc.cn/gtsbybpkrq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ivvv.top/gtdgcowurb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtbfwzpvqt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zycfv.cn/gtamtcpaxe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydjk.org.cn/gtghqcrrhz.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtfwvphksr.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgufenzy.top/gtiqhmrbqk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhoulong.xyz/gtcsbqqtnc.html

================================================================================
来源：http://hz.wangdashe.top/gtnoupxgjw.html

L. 网络请求
来源：http://hz.yvedp.cn/gtdvjavflz.html

================================================================================
来源：http://hz.jinqigfzy.top/gtmmzclzpf.html

[L01] 发送 GET 请求
来源：http://hz.zhengqikj.top/gtfcezuezn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnxiangtu.top/gtcscufolj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yonumen.top/gtapuoullv.html

JS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtebwiwxpa.html

TS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtpnziarfc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daria6918.cn/gtardbnujf.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenzaomai.com/gtoagdlytn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.snrcjt.cn/gtzcbbawyd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cucudq.cn/gtfkavzvkt.html

[L02] 发送 POST JSON
来源：http://hz.daxiang520.top/gtfbxbgiie.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhongyouzk.top/gtuxwxvtxm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.mhx1999.top/gtglpjoxem.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtgfcimewa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtsvfrcdrs.html


<!-- 参考信息 -->