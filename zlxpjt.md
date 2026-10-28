代发 wailian999

[H07] 断言
来源：http://hz.sweek.top/gtxpienafd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zycfv.cn/gtbhrkgjoc.html

PHP:  assert($x > 0);
来源：http://hz.tianlin.xyz/gttepdtcoq.html

JS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtfmsxosww.html

TS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtgaawjzzi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yanxiufei.cn/gtjmcxlvsx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nwbrower.top/gtgdsurwmz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zycfv.cn/gtpauknluc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.andypj.xyz/gtaqesyfnq.html

[H08] 获取错误信息与堆栈
来源：http://hz.hywenlv.cn/gtacnwjfwl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258888.top/gtigpdxpzs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.316326.xyz/gtxvognmwp.html

JS:   e.message;  e.stack
来源：http://hz.shangyingyoupin.top/gtfjjwojvm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.redwolf501.top/gtytvklfpz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hammf.cn/gtwwchzjjc.html

Go:   err.Error()
来源：http://hz.havefunace.top/gtjajdhaps.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgufenzy.top/gtzjcrzubg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtkghkivjt.html

[H09] 带错误码的异常
来源：http://hz.jinqigufen.top/gtbgmobjuu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258.top/gtijcqardw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenlongwang.top/gtyuwqvkju.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.quarkkingdee.top/gtjxihxaxh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxuanxn.top/gtsoonzdsq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.svipenyu.cn/gtyosmgfcu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ppjwa.cn/gtygghmwik.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sxryk.cn/gtrewqdlet.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.haohaochexian.top/gtfrdxenqf.html

[H10] 资源自动释放
来源：http://hz.jlsjyb.cn/gtcdezghvf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cucudq.cn/gtalgncrrq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.havefunace.top/gtjtvfelrk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtmiezihlf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtboqolkgg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daxiang520.top/gtkphipxmg.html

Go:   defer f.Close()
来源：http://hz.mhx1999.top/gtidjsseij.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.birdmap.top/gtvuoovwgc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nwbrower.top/gtmucnglds.html

================================================================================
来源：http://hz.hnxiangtu.top/gtyidptuxq.html

I. 正则表达式
来源：http://hz.hongshengwenyu.top/gtlmxthgix.html

================================================================================
来源：http://hz.yj20258888.top/gtdaxbcthk.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtprxckqax.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ybcxt.top/gtgccuvswv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.birdmap.top/gtxvddcleh.html

JS:   /\d+/.test(s)
来源：http://hz.sysykeji.top/gtyivhltyg.html

TS:   /\d+/.test(s)
来源：http://hz.daria6918.cn/gtxcikrawg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinyuanbaomall.cn/gtbypicncz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinghuilouyu.cn/gtwmzcmbkw.html

Ruby: s.match?(/\d+/)
来源：http://hz.feifeiyinyue.top/gtmfxhyyln.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenzaomai.com/gtlzgeumhu.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtzhsjfvnv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tianlin.xyz/gtrxmjoisc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigufen.top/gtqnhbklpz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangdashe.top/gtjybqwxxm.html

TS:   s.match(/\d+/g)
来源：http://hz.shangyingyoupin.top/gtijcskhww.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tian-w.cn/gtclimvueu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ydzc1.top/gtvutbaqbv.html

Ruby: s.scan(/\d+/)
来源：http://hz.c1oappe.top/gtwdjcptnv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gaohongyu789.top/gtyxpocnrk.html

[I03] 提取捕获分组
来源：http://hz.hywenlv.cn/gtcnzyzzdp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sweek.top/gtvhnwaqwo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhijiandao.cn/gteoiqsels.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dianchejie.cn/gtwrefzkzq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yonumen.top/gtgovjvesj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tian-w.cn/gtpoxfzomb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nwbrower.top/gtaosjpdcg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenlongwang.top/gtouavddqm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhaomingkeji.xyz/gtypqrorxq.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtoqcgfkpz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yonumen.top/gtyearqkho.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuetiantiany.cn/gtjduezcne.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gtsvekbasp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtttnvhake.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxuanxn.top/gtplvvzsrz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydzc1.top/gtiodmbqmu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xinyue.icu/gtvjjyymxg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sweek.top/gtauougwdy.html

[I05] 按正则拆分
来源：http://hz.jinqigufen.top/gtkjqhmtix.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ywan-chungtsiang.top/gtjhxervcy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.quarkkingdee.top/gtyuwbnybp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtbvzyjphi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtxtdgmyqf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aibaodan.cn/gtwzwjhwvk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nwbrower.top/gtbpfpntxa.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtpmrawcxm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cucudq.cn/gtxjhegxbj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenzaomai.com/gtgnotlmzb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtkkywyxmu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtnlqeoszv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtmdnixhso.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gtchvtztzt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258.top/gtbkivqpgb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenlongwang.top/gtbpjiqyvk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shzxlz.cn/gtcbwnchps.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtfopnlivy.html

[I07] 忽略大小写与多行模式
来源：http://hz.quarkkingdee.top/gtppkndvzs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ivvv.top/gtdekoeryj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gtznkzgfcc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fengsongda.top/gtptbmfeds.html

TS:   /error/gim
来源：http://hz.birdmap.top/gtvpepbxml.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xylfe.cn/gtviwpssfv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.52xcode.cn/gtvlcgfowj.html

Ruby: s.scan(/error/i)
来源：http://hz.ydjk.org.cn/gtdbfxmecs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.vqdsnc.cn/gttnzkqodf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangshuangyany.cn/gteyxywvup.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.quarkkingdee.top/gtjhlasaxu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nwbrower.top/gtxdkbeeij.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtlvowizww.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gtdtcmpivi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gthhcqiejr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gthelusvnf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigfzy.top/gtdcdgiheq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtqjrqtipz.html

================================================================================
来源：http://hz.sysykeji.top/gtudsgzkms.html

J. 日期与时间
来源：http://hz.hfpthk.cn/gthnxyfhfc.html

================================================================================
来源：http://hz.shuidangran.top/gtlyhaaizw.html

[J01] 获取当前时间
来源：http://hz.sxryk.cn/gtywfqlonk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pycfn.com/gtkwcvyazh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtebidykaw.html

JS:   new Date();  Date.now()
来源：http://hz.zhijiandao.cn/gtqympleiq.html

TS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtlhuzadnp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxuanxn.top/gtqwpdstme.html

Go:   time.Now()
来源：http://hz.wangshuangyany.cn/gtarjbjmcr.html

Ruby: Time.now
来源：http://hz.xinyue.icu/gtwvkagvhv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jianghu66.top/gtmdhwicdy.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gtyzfxxiot.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinyuanbaomall.cn/gtawhvjgxn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gtmuixofrd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhongyouzk.top/gtcizmbbhj.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangtech.top/gtfehobbcu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shuidangran.top/gtoxuwyguv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sxryk.cn/gtbtqajqqk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtptilmoia.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hammf.cn/gtmdumpnzz.html

[J03] 字符串解析为日期
来源：http://hz.wangdashe.top/gtkvsufect.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtkqowdzgt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.snrcjt.cn/gtzgxixcgf.html

JS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gthhmlopdy.html

TS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtmsjeckfd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hywenlv.cn/gtlbwcbhgy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtcdatptco.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtstpusnrc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.quarkkingdee.top/gthnvguxqb.html

[J04] 时间戳与日期互转
来源：http://hz.yongpay.top/gtnbxfiomw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ywan-chungtsiang.top/gtoakdnbem.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yangfankeji.com/gtxkpvsvvf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yongpay.top/gtoalqsowy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnxiangtu.top/gtspihcsqy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxuanxn.top/gtxhnllcba.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yonumen.top/gtjggjksrl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zdqjudy.top/gtcmgqbahn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jianghu66.top/gtiduxxrpp.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgufenzy.top/gtcbnovizp.html

Py:   now + timedelta(days=7)
来源：http://hz.gaohongyu789.top/gtlzgzrucm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yangfankeji.com/gtmietydhz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtmknleytg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtzhffzcha.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtavzizqfn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yvedp.cn/gtmmhqpugh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hfpthk.cn/gtscrxbazp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.meibo888.top/gtclaxblkr.html

[J06] 计算两时间之差
来源：http://hz.cashguo.top/gtqarsyfjn.html

Py:   (end - start).total_seconds()
来源：http://hz.birdmap.top/gtiqahsifi.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhaomingkeji.xyz/gtohiblemy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gaohongyu789.top/gtrtddnrox.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xinyue.icu/gtoeltffrr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zdqjudy.top/gtjgagwndf.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinyuanbaomall.cn/gtvjigxvpy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.redwolf501.top/gtsvpwoiyw.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhengqikj.top/gtmterecyx.html

[J07] 比较两个日期
来源：http://hz.guannengcc.top/gtbhxumccn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtipznbcfp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.haohaochexian.top/gtfcxcaifl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtiuguiquq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgfzy.top/gtmlebzmyn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258.top/gtarbeabhr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenlongwang.top/gtvucsjvgc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtmtpkpace.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtidiqofdn.html

[J08] 提取年月日与星期
来源：http://hz.ybcxt.top/gtwonrpejp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.feifeiyinyue.top/gtzvbggrml.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yongpay.top/gtdazmsliu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhongyouzk.top/gtfntsvate.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtsqxpnfor.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtyzhvtqen.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sysykeji.top/gtbwuibkgu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cashguo.top/gtrwcikcxj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhongyouzk.top/gtgcpyunkj.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtouszwlzk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gtlgmnieqh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhongyouzk.top/gtxxzjdwwx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtzirlkkdy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtvowlrejg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgfzy.top/gtkqddphna.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.svipenyu.cn/gtylaqdrxu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtbrenagin.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinghuilouyu.cn/gtafejmcwf.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtfrzwivwi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gtlswujymz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinyuanbaomall.cn/gtfvivonco.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jiagoushi.top/gtdhzkqjmn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtxrdiqirq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gtxtetexsm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gtkzvqnycv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtypjhawkx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gthybcvpdp.html

================================================================================
来源：http://hz.fzhhl.top/gtzxwwjzug.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gtklgmdbow.html

================================================================================
来源：http://hz.dianchejie.cn/gtjkfmrqyx.html

[K01] 对象转 JSON 字符串
来源：http://hz.shuidangran.top/gtkvbvqwzr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sxryk.cn/gteyjdjhzv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtvhmszqdu.html

JS:   JSON.stringify(obj)
来源：http://hz.shangyingyoupin.top/gtyqqnyzto.html

TS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtaywcmgpg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hysaishi.cn/gttvzdkamj.html

Go:   json.Marshal(obj)
来源：http://hz.dashuyun.cn/gtglwxhmqv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aibaodan.cn/gtjguxpohj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sysykeji.top/gtmysqlwif.html

[K02] JSON 字符串转对象
来源：http://hz.c1oappe.top/gtzqkkpbnx.html

Py:   json.loads(s)
来源：http://hz.gotoacloud.top/gtihugtvzk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhiwuduotai.top/gtkweokxzr.html

JS:   JSON.parse(s)
来源：http://hz.havefunace.top/gthoehzsev.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtqgzknnak.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ehwqpu.com/gtqzdnpckh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtblselfhz.html

Ruby: JSON.parse(s)
来源：http://hz.andypj.xyz/gtlwgsjavr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yongpay.top/gtqmgpftkj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hywenlv.cn/gtdzfhqflq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtosxfeuvo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtvmhmxvke.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtjecydesr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xziqi.cn/gtoeobxewx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.316326.xyz/gtmpeeretx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.meibo888.top/gtdqmauzlw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aizwys.cn/gtfpvpezjn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.snrcjt.cn/gtzsbmqrpu.html

[K04] 读取 JSON 文件
来源：http://hz.pengpengdd.cyou/gtmwxtwxgo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gzhubu.top/gtsbdyfmzf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gtqcdudqja.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtsdnxnqmg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtpbiqdoci.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xinyue.icu/gtzuymohgv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtlcibkllo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xylfe.cn/gtfpyfhkqs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ehwqpu.com/gtbtgbtbdq.html

[K05] 深拷贝对象
来源：http://hz.yongpay.top/gtvgebqhdy.html

Py:   copy.deepcopy(obj)
来源：http://hz.feifeiyinyue.top/gtlyftcxsv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gaohongyu789.top/gteoecogxx.html

JS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtaghfnegh.html

TS:   structuredClone(obj)
来源：http://hz.hnqzz.top/gtvylhlxzu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cucudq.cn/gthqdjacrh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gogol.net.cn/gtfidfrzgg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hfpthk.cn/gtkwpwjpql.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.iojbl.cn/gtkbusrqai.html

[K06] 解析 URL 查询串
来源：http://hz.fengsongda.top/gtokpldder.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ivvv.top/gtsitrihma.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cashguo.top/gtzmwlrndd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gtcbbtdbri.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtkgqkacec.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zycfv.cn/gtfbvoxlak.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258888.top/gthtgtfzjg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtgsboctzh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtruxkrzcq.html

[K07] 进制转换
来源：http://hz.sxryk.cn/gtepyrlsfn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.haohaochexian.top/gtfuxuhjsd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigufen.top/gthsdogwoe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtnqrflvdj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtwybrvjvt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtysjgvkfx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guannengcc.top/gtvkcrguzu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ywan-chungtsiang.top/gtvifhidzt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gogol.net.cn/gtcpncyuwo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jlsjyb.cn/gtaftvwbay.html

Py:   pickle.dumps(obj)
来源：http://hz.hysaishi.cn/gtryugkfhw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ehwqpu.com/gtrbrbywzw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtwvfrnipg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtcdfelwrl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yvedp.cn/gtwwujdcwz.html

Go:   encoding/gob
来源：http://hz.gotoacloud.top/gtfproribf.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258.top/gtpedoeqbc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cashguo.top/gtzpfkmvas.html

================================================================================
来源：http://hz.gaohongyu789.top/gtchbybzhs.html

L. 网络请求
来源：http://hz.jinqigufen.top/gtyfzedbzn.html

================================================================================
来源：http://hz.wangdashe.top/gtitizaald.html

[L01] 发送 GET 请求
来源：http://hz.vqdsnc.cn/gtcigcyieb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xylfe.cn/gtlrevzovu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ywan-chungtsiang.top/gtlikghofp.html

JS:   await fetch(url)
来源：http://hz.mhx1999.top/gtvjauouzd.html

TS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtwnhizqjx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jianghu66.top/gtppztmmuj.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gthoyzpgvf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jyoumei.cn/gtqbejuipc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daria6918.cn/gtxpfszqpc.html

[L02] 发送 POST JSON
来源：http://hz.yj202588.top/gthvtfrqrd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtarcwavjq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.redwolf501.top/gthptfbbil.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daxiang520.top/gtcehojklt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gtibfjgwxc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.kuanghao11.cn/gteozwkece.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.andypj.xyz/gthykyzuhs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xingfuxueyuan.xyz/gtgzpxfhdr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtsphffwzv.html


<!-- 参考信息 -->