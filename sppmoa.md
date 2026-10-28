代发 wailian999

[H07] 断言
来源：http://hz.xuetiantiany.cn/gtttmogfdr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gotoacloud.top/gtwsbuzhsh.html

PHP:  assert($x > 0);
来源：http://hz.yvedp.cn/gtbmtxzqfk.html

JS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtnmjyiglr.html

TS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtdnxpupzq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hfpthk.cn/gtvwqyozcc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydjk.org.cn/gtjdqsjzkh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.daxiang520.top/gttxusdmhp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuanzhike.top/gtqqhiicbd.html

[H08] 获取错误信息与堆栈
来源：http://hz.redwolf501.top/gtdfhxxwae.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zycfv.cn/gtunwziuup.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shangyingyoupin.top/gtsfftlbam.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gtdwjiuply.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenzaomai.com/gtvvfraqha.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtohllnkbg.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtfeciwppj.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinghuilouyu.cn/gtvvamsrdi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jianghu66.top/gtaazydjsk.html

[H09] 带错误码的异常
来源：http://hz.hammf.cn/gtweyfohhq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sufxvd.cn/gtkqmovdpn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.c1oappe.top/gtqpzxhhrk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuanzhike.top/gtwpshkbux.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ivvv.top/gtyffzdrgg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.havefunace.top/gtxihsvcma.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtjfnrzzxb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.c1oappe.top/gtcqdcczlk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hammf.cn/gtckhinxhe.html

[H10] 资源自动释放
来源：http://hz.yongpay.top/gtzqjaoxxx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gotoacloud.top/gtpucoxsiq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.quarkkingdee.top/gtujdqfjwd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtgmvjcdsp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.svipenyu.cn/gtjzzaaqff.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sweek.top/gtiryaaeam.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gtjyabpiks.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daxiang520.top/gtwlrxpbwf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xinyue.icu/gtsqlbqhii.html

================================================================================
来源：http://hz.ivvv.top/gtbcylkexl.html

I. 正则表达式
来源：http://hz.cqqwz.cn/gthupkcztf.html

================================================================================
来源：http://hz.yj20258888.top/gtvdcggnvm.html

[I01] 判断是否匹配
来源：http://hz.shuidangran.top/gtlczhcxjs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sysykeji.top/gtzahmuxxd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xylfe.cn/gtlabgyfhc.html

JS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gtiihcsuvi.html

TS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtrvumqpdh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtuvvfyxjs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nanxinkj.top/gtpohdfijh.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhengqikj.top/gtxcihfirg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yongpay.top/gtwoefmwta.html

[I02] 提取所有匹配
来源：http://hz.hywenlv.cn/gtckusapun.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aibaodan.cn/gtuonpsyao.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yongpay.top/gthulvdxlj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhoulong.xyz/gtyygedxel.html

TS:   s.match(/\d+/g)
来源：http://hz.snrcjt.cn/gtezcbbbxo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jiagoushi.top/gtilnihbqx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.mhx1999.top/gtzmkdhgah.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtsxnnzjbi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangshuangyany.cn/gtptdtrjra.html

[I03] 提取捕获分组
来源：http://hz.hnxiangtu.top/gtapczwmce.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pycfn.com/gtovwzvowp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhijiandao.cn/gtueonlltm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ehwqpu.com/gtddnjyebd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangkeji.top/gtzrgcqipl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aizwys.cn/gtodwylwmt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sysykeji.top/gtaogxuhfq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgfzy.top/gtzwmilaaz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.havefunace.top/gtujaozrfe.html

[I04] 正则替换
来源：http://hz.feifeiyinyue.top/gtpszfypjb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.guannengcc.top/gtydsitwbs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtpdoxnixu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gttnwynpvc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gtlrekafnm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tian-w.cn/gtclxntlbb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gtgquoxyly.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenlongwang.top/gtynswsmxt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pycfn.com/gtxmmzsqbo.html

[I05] 按正则拆分
来源：http://hz.zycfv.cn/gtkmbpcpgg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gzhubu.top/gtcmzacfzi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhengqikj.top/gtnrpokwtt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtwzijhjqd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtwynikyvn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.dianchejie.cn/gtvxeayxlh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shzxlz.cn/gtyrbzusdc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtrvdthxuj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.bjfxy.top/gtedvgjxas.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.havefunace.top/gtpydhaokg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtzvkmdlsf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.aibaodan.cn/gthjxvinyo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gttexefzjl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtxschvsyf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hywenlv.cn/gtjzfoyxqu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtkeplgacu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daxiang520.top/gtwjxpnuyu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenjidiqi.icu/gtmwetrvql.html

[I07] 忽略大小写与多行模式
来源：http://hz.svipenyu.cn/gtpohziosc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gotoacloud.top/gtcidlzsfp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtzjfsfyhu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shangyingyoupin.top/gtuysvqdom.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtrccawamc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xinyue.icu/gttwtrfaln.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gtnmlsfhci.html

Ruby: s.scan(/error/i)
来源：http://hz.sxryk.cn/gtzogfrywl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jiagoushi.top/gtoyabhjeq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jyoumei.cn/gtqxxokwye.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hnxiangtu.top/gtrobwifbh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fengsongda.top/gtvmiubylq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinghuilouyu.cn/gthsgkcnzv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtqfmhqfcc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.52xcode.cn/gtiianpjhi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hammf.cn/gtrcyaukrb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.smart0.xyz/gtchjqwtnd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xuanzx.com/gttksciyky.html

================================================================================
来源：http://hz.yj202588.top/gtnmzdpexg.html

J. 日期与时间
来源：http://hz.feifeiyinyue.top/gtnjnuccbr.html

================================================================================
来源：http://hz.yvedp.cn/gttrnfgabw.html

[J01] 获取当前时间
来源：http://hz.zhijiandao.cn/gtbdzynera.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yanxiufei.cn/gtstlzyzdu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtudcxnkkp.html

JS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtbcrwcwqp.html

TS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtjlfvhvfg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnqzz.top/gtnqzosvek.html

Go:   time.Now()
来源：http://hz.ywan-chungtsiang.top/gtzzsplvpk.html

Ruby: Time.now
来源：http://hz.ivvv.top/gtpzikqwto.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.fzhhl.top/gtaqzqncbd.html

[J02] 格式化输出
来源：http://hz.shangyingyoupin.top/gtlxvklnek.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtdhcwiwxq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtphjyvpxg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guowangkeji.top/gtqezrlkha.html

TS:   d.toISOString()
来源：http://hz.gotoacloud.top/gtkngztuli.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hongshengwenyu.top/gtjfxxprdg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.0kj1m.cn/gtnsmfuyms.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shangyingyoupin.top/gtakzqhxan.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gogol.net.cn/gtcyjipmwl.html

[J03] 字符串解析为日期
来源：http://hz.nanxinkj.top/gtyrjdizxy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shangyingyoupin.top/gtjaaydecn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dianchejie.cn/gtrzvtowbm.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtvryoznpk.html

TS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtejleyozo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtswovzwtd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hysaishi.cn/gtossluilx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtlstrauyp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shangyingyoupin.top/gtcyvqhhgx.html

[J04] 时间戳与日期互转
来源：http://hz.chenzaomai.com/gtmjnyvqyr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sweek.top/gtrwfhxxco.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pycfn.com/gtjemikihq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258888.top/gtiyeqarpg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gzhubu.top/gtvsmsprwx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aibaodan.cn/gtaettzqgv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jiagoushi.top/gtitqbmzva.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtltkcajrb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydjk.org.cn/gtywexywrm.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnxiangtu.top/gtgilhrnwl.html

Py:   now + timedelta(days=7)
来源：http://hz.yvedp.cn/gtrfemphee.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.bjfxy.top/gtnualabnp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtucukfwjr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtggeddqns.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.meibo888.top/gtnoseunfq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jianghu66.top/gtppigxqtq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.bjfxy.top/gtzyqnptbe.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gtyvqstacw.html

[J06] 计算两时间之差
来源：http://hz.wangshuangyany.cn/gtgjqvnpqv.html

Py:   (end - start).total_seconds()
来源：http://hz.aibaodan.cn/gtuzvsuvzt.html

PHP:  $end->diff($start)->days;
来源：http://hz.tian-w.cn/gtzxscuanq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cashguo.top/gtoqpejjqm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gtfrdqmhkw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zdqjudy.top/gtcszkmmbg.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj202588.top/gtjwwlxvtc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.feifeiyinyue.top/gtyggmjtqf.html

C#:   (end - start).TotalSeconds
来源：http://hz.cqqwz.cn/gtlxgoqwtn.html

[J07] 比较两个日期
来源：http://hz.gotoacloud.top/gttkefoaae.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtddbykwlm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gzhubu.top/gtboeagdlu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtsimsgmyy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtzitazcdi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ivvv.top/gtseozrlnt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gaohongyu789.top/gtllwljddr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtebelrlqw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtorabnavo.html

[J08] 提取年月日与星期
来源：http://hz.jinghuilouyu.cn/gtcmgtukjp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangkeji.top/gtaeidwqki.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dashuyun.cn/gtillvyvcz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenjidiqi.icu/gtbzpzsnnt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ivvv.top/gtzgiamedy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtuanckccl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj202588.top/gtfcqtkcyg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenjidiqi.icu/gtwjunpsda.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gteqmsvbuj.html

[J09] 时区处理
来源：http://hz.sxryk.cn/gtjzriyvnk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cashguo.top/gtnzhcxqxx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xylfe.cn/gtnmwtnnis.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtuaeasorx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtjfhczsws.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj20258888.top/gtaqcaiywm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhijiandao.cn/gtogzuabrj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258.top/gtwsaanqyt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sysykeji.top/gtxztakupy.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtrtmnfpzn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gtlamnjqfw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangdashe.top/gteplwhsed.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxuanxn.top/gtwxkfpylm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.birdmap.top/gthusonfiq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.52xcode.cn/gtswhklkvb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxinkj.top/gtdrzvcqnt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangtech.top/gtohnwerce.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dianchejie.cn/gtvpkpnyoc.html

================================================================================
来源：http://hz.dianchejie.cn/gtkqwzmljd.html

K. JSON 与序列化
来源：http://hz.ydjk.org.cn/gtcneaaxqe.html

================================================================================
来源：http://hz.xylfe.cn/gtrbbhzoxj.html

[K01] 对象转 JSON 字符串
来源：http://hz.sufxvd.cn/gtfntrfcyj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtlizrqreq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gtzebjgukl.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtemernbwp.html

TS:   JSON.stringify(obj)
来源：http://hz.xinyue.icu/gtbctbbewq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fengsongda.top/gtbucoyhnn.html

Go:   json.Marshal(obj)
来源：http://hz.quarkkingdee.top/gtdguqeokg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangkeji.top/gtfunfkuem.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yongpay.top/gtdxnecdkk.html

[K02] JSON 字符串转对象
来源：http://hz.gzhubu.top/gtdpxxqzbb.html

Py:   json.loads(s)
来源：http://hz.xuetiantiany.cn/gteyiceiic.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhixingplan.top/gtgcxofkoq.html

JS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtuixpsusy.html

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtjewbbtgx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhixingplan.top/gtahmhktvv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtaaudxgsp.html

Ruby: JSON.parse(s)
来源：http://hz.jyoumei.cn/gtzmnfikrs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yueranfly.top/gtqfhsqfzu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yongpay.top/gttkzzlriv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.havefunace.top/gtigmrdgvu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtkmxrolvx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtjopkpqic.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtgxtgsrus.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aizwys.cn/gtysjxcnrh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxuanxn.top/gtfifvfbyi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.316326.xyz/gtqcvzeuiu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangdashe.top/gttrramvma.html

[K04] 读取 JSON 文件
来源：http://hz.jiagoushi.top/gtxsqtyqgu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.pycfn.com/gtywxvhjnt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258888.top/gtzxsoicgk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtjnvhawom.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtwtmhgdos.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtryoqyzsg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtswlhxsjy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.52xcode.cn/gtljlrvzic.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258888.top/gtbwvspnto.html

[K05] 深拷贝对象
来源：http://hz.guowangkeji.top/gttheqajzr.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinyuanbaomall.cn/gtljyucsno.html

PHP:  unserialize(serialize($obj));
来源：http://hz.fzhhl.top/gtcajpibzd.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtiynhdrqt.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtjtyblygc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ehwqpu.com/gtcyjnoifg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenzaomai.com/gtdkgpuwhh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.feifeiyinyue.top/gtejxjilmu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sufxvd.cn/gtbcyfdzrw.html

[K06] 解析 URL 查询串
来源：http://hz.smart0.xyz/gtmfnrlykk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenlongwang.top/gtsgjwgiqi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.havefunace.top/gteftusjgv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtaacoaoak.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtntguxnpf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hfpthk.cn/gtlxendzvk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gotoacloud.top/gtdxhwlqhm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yvedp.cn/gtvgjzqqyt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtdckxhaax.html

[K07] 进制转换
来源：http://hz.yongpay.top/gtmosjqray.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.vqdsnc.cn/gtcjmcifnd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtziqjwsuz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtqhotghxe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtyxvtcteg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtjksgtedt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtrwjqibak.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.0kj1m.cn/gtkbbmqeyd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fzhhl.top/gtcxuprvwe.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aizwys.cn/gthtigiwps.html

Py:   pickle.dumps(obj)
来源：http://hz.pycfn.com/gttrfodvdy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuetiantiany.cn/gtoxjqirej.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenlongwang.top/gtnxdhwsuw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtvznrdzat.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yueranfly.top/gtexhimhhp.html

Go:   encoding/gob
来源：http://hz.cheryme.top/gtibltzxlm.html

Ruby: Marshal.dump(obj)
来源：http://hz.jiagoushi.top/gtkhqxiaks.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shuidangran.top/gtmqlgylon.html

================================================================================
来源：http://hz.jqgfzy.top/gtberjmxku.html

L. 网络请求
来源：http://hz.chenzaomai.com/gtxvpbpbwd.html

================================================================================
来源：http://hz.mhx1999.top/gtiphwubvk.html

[L01] 发送 GET 请求
来源：http://hz.kuanghao11.cn/gtlrshkzyt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.0kj1m.cn/gtzptelmic.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigfzy.top/gtcckagfck.html

JS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtvznpgxlu.html

TS:   await fetch(url)
来源：http://hz.hnqzz.top/gtcnymupat.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shuidangran.top/gtxjsvfzfh.html

Go:   resp, err := http.Get(url)
来源：http://hz.yvedp.cn/gtsysioliq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.vqdsnc.cn/gtrtvsvtsn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.52xcode.cn/gtcwasahca.html

[L02] 发送 POST JSON
来源：http://hz.cashguo.top/gtjohksbnf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtrupolhgu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuxming.cn/gtwpsxyxto.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtbocrxfsz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtnpfeiiuo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.dashuyun.cn/gtbtxrizgq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtlbuqyxyd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtgbjjbetq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhixingplan.top/gtablqjucs.html


<!-- 参考信息 -->