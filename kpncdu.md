代发 wailian999

[H07] 断言
来源：http://hz.yj202588.top/gtsyoxbfjp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gtmfyghsop.html

PHP:  assert($x > 0);
来源：http://hz.zhongyouzk.top/gtqggrpjcz.html

JS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtwbresgyt.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtwtjhlksg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sysykeji.top/gtoaofyjrz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxinkj.top/gtkhzezgbe.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenzaomai.com/gtqafarxdg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jianghu66.top/gtdtnxuoqf.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhengqikj.top/gtjqnnrxnp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.kuanghao11.cn/gtrnkahwba.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yangfankeji.com/gtucjgucba.html

JS:   e.message;  e.stack
来源：http://hz.xuetiantiany.cn/gtqyyvjvjo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhijiandao.cn/gtadjqgteo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenlongwang.top/gtiwizvckg.html

Go:   err.Error()
来源：http://hz.zhengqikj.top/gtoiaudvur.html

Ruby: e.message;  e.backtrace
来源：http://hz.ivvv.top/gtfhfntchx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hammf.cn/gtbkksekck.html

[H09] 带错误码的异常
来源：http://hz.tianlin.xyz/gthchvdhzp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuanzhike.top/gtsnyngyei.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hysaishi.cn/gtiznhivqg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtyhzedjqt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.haohaochexian.top/gtxamlnebj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gogol.net.cn/gtrsvnxgga.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj202588.top/gtsfhbdlkt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hfpthk.cn/gtcwomgvqv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shangyingyoupin.top/gtgwbfnfhv.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtcfpcmson.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.feifeiyinyue.top/gtiuaalwcz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yonumen.top/gtiiqqnyjx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gttcodwvrs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtqzquicij.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hammf.cn/gtzofaqtll.html

Go:   defer f.Close()
来源：http://hz.nanxuanxn.top/gtadpaqqxy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtbkmrbxib.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ehwqpu.com/gtbmfkpihu.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtyfkddbky.html

I. 正则表达式
来源：http://hz.snrcjt.cn/gtijdsreiv.html

================================================================================
来源：http://hz.yj20258.top/gtzihwaudo.html

[I01] 判断是否匹配
来源：http://hz.ydzc1.top/gtlmwouwnu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nwbrower.top/gtxxdmbfnu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yangfankeji.com/gtjajsjsqk.html

JS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gthlgbejoi.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtrmhmpjvo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhengqikj.top/gttguswyhz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cashguo.top/gttovwjkaj.html

Ruby: s.match?(/\d+/)
来源：http://hz.ivvv.top/gtqrvuflga.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.guannengcc.top/gtzkhcampf.html

[I02] 提取所有匹配
来源：http://hz.mhx1999.top/gtslcidevb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtlppscsij.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.meibo888.top/gtjkazeuxp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinghuilouyu.cn/gtgmofqtjc.html

TS:   s.match(/\d+/g)
来源：http://hz.ywan-chungtsiang.top/gtxxkxoboq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.316326.xyz/gtuieutizt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuxming.cn/gtsajsgrtq.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gtcuwnsbzc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnqzz.top/gtkeffpghs.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangkeji.top/gtoagbicvm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sufxvd.cn/gthtrcdkku.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigufen.top/gtqrdpgzfn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tanke756.top/gtlaohozjf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.52xcode.cn/gtuhkwxusi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.0kj1m.cn/gtehuzjfnu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cucudq.cn/gtpluqxchj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xinyue.icu/gtteghhmag.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj202588.top/gtcrzcxbnm.html

[I04] 正则替换
来源：http://hz.c1oappe.top/gtdkkckqms.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jyoumei.cn/gttpwlueoq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.vqdsnc.cn/gtcjxevhmg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fzhhl.top/gtgzpplhwr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.meibo888.top/gtjoreqyyg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.feifeiyinyue.top/gtwcysrwnr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yonumen.top/gtwioetphg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gteoccnfjj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj20258.top/gthffdxbjq.html

[I05] 按正则拆分
来源：http://hz.yonumen.top/gtaqzzvgfj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yangfankeji.com/gtmrpxfeqz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cashguo.top/gtvxpmemzq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtmmdfmwud.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtuycxpnbw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hfpthk.cn/gtgdnrvhrl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gaohongyu789.top/gtxkzmrwyj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtoktxmeka.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cucudq.cn/gtjbhdwcsk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydzc1.top/gtvjplryjm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtfypfgkik.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cqqwz.cn/gtlzwstulj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtxllrkbqf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtulrmmzkn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cucudq.cn/gtdwdexniz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.dianchejie.cn/gthydwhhgd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuanzhike.top/gtylpavvdq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtfcpqmeiu.html

[I07] 忽略大小写与多行模式
来源：http://hz.gogol.net.cn/gtfkvvotyl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gtpquwhjpu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.andypj.xyz/gtfccjzidv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zycfv.cn/gtjtizkhrm.html

TS:   /error/gim
来源：http://hz.ybcxt.top/gteyqtkxyv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangkeji.top/gtdhkfskxc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhiwuduotai.top/gthgdvojgc.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxuanxn.top/gtmigzjwja.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tianlin.xyz/gtobtmujxu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtcsehawzn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinghuilouyu.cn/gtntsqsbrq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hammf.cn/gtwericobg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtfiuprdup.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtoogmazva.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jianghu66.top/gtkfeehjhj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.birdmap.top/gtrlvhthga.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gotoacloud.top/gtqfmliwaa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtafeescwb.html

================================================================================
来源：http://hz.yonumen.top/gtdwtcxugu.html

J. 日期与时间
来源：http://hz.hfpthk.cn/gthlguykff.html

================================================================================
来源：http://hz.sweek.top/gttzmiuvvo.html

[J01] 获取当前时间
来源：http://hz.jinqigfzy.top/gtfhpemlyo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gtsqpsaxiz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtonkronrs.html

JS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gtlbwcvqlf.html

TS:   new Date();  Date.now()
来源：http://hz.yanxiufei.cn/gtgrqdmmei.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sxryk.cn/gtvqbttbat.html

Go:   time.Now()
来源：http://hz.iojbl.cn/gtlkwrhagn.html

Ruby: Time.now
来源：http://hz.fengsongda.top/gtlahtduqa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dashuyun.cn/gtzoqyhkvh.html

[J02] 格式化输出
来源：http://hz.iojbl.cn/gtwomzeopg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtdyafiols.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtlyfltcah.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258.top/gtfkdxgavy.html

TS:   d.toISOString()
来源：http://hz.jinyuanbaomall.cn/gtvogqrjxd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tanke756.top/gtkimgdhfl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gtmiguxpmr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtjukjvmqw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aizwys.cn/gtjfrbzvzr.html

[J03] 字符串解析为日期
来源：http://hz.hfpthk.cn/gttnrkcdus.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hfpthk.cn/gtauosxevi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.52xcode.cn/gtjdjnmrdp.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gttirgsiif.html

TS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gttbfwfwxa.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtanoesqgm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.pycfn.com/gtgdnwjckw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtlyharjmo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.mhx1999.top/gtlbswobsk.html

[J04] 时间戳与日期互转
来源：http://hz.ywan-chungtsiang.top/gtgzgqzcor.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gzhubu.top/gtcslfygop.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fengsongda.top/gtfgyzkuec.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydjk.org.cn/gtramrizdz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxuanxn.top/gtpvwvxcxw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.kuanghao11.cn/gtftowknpb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.bjfxy.top/gtmfrqpivv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ybcxt.top/gtygadvjne.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jiagoushi.top/gtjqmtrvqk.html

[J05] 时间加减（加 7 天）
来源：http://hz.yuxming.cn/gtmtpoimpt.html

Py:   now + timedelta(days=7)
来源：http://hz.feifeiyinyue.top/gtpnaskhva.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yueranfly.top/gtxuazkmoo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtgflwxcpw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtsbzfwtqe.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenlongwang.top/gtyhbrqbsb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ehwqpu.com/gtooulhvyr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.andypj.xyz/gttemugost.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fzhhl.top/gtbhpemssz.html

[J06] 计算两时间之差
来源：http://hz.meibo888.top/gtxjgxhlct.html

Py:   (end - start).total_seconds()
来源：http://hz.ydzc1.top/gtpnjwobdm.html

PHP:  $end->diff($start)->days;
来源：http://hz.tianlin.xyz/gtszbnuvgk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jqgufenzy.top/gtgbbuimoo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hfpthk.cn/gttlfddylc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guowangkeji.top/gturcsmwvw.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhaomingkeji.xyz/gtjszbnxvr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtkmzeeebs.html

C#:   (end - start).TotalSeconds
来源：http://hz.ywan-chungtsiang.top/gtdcphgumr.html

[J07] 比较两个日期
来源：http://hz.sxryk.cn/gtbhjmhlbl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtikxyysyh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhongyouzk.top/gtgsgefzko.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtznwkildp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtgyjxslcs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aizwys.cn/gtdzwtocic.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenlongwang.top/gtqytgzyji.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtennxasfc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtyicaagqx.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangtech.top/gtqqrcsuph.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnxiangtu.top/gtxaldayxk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cucudq.cn/gtaflccyli.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.52xcode.cn/gtpdsoowdh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydjk.org.cn/gtzhbadlag.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pengpengdd.cyou/gthmgmqior.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gthgmxjemz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tianlin.xyz/gtjknfpimr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gtyyxleojg.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtmbozxcsm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dianchejie.cn/gtusjoobkl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zycfv.cn/gtcnrirjnw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtgxsgjchl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtrlcifexw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gogol.net.cn/gtwfjxhago.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gaohongyu789.top/gtjlslugxs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnxiangtu.top/gtkjxhzrji.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenjidiqi.icu/gthkffjhcw.html

[J10] 取今天 / 本月第一天
来源：http://hz.yongpay.top/gtwpkkhuir.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinyuanbaomall.cn/gttifbwunb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gtcxplmuwe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ybcxt.top/gtvurhkjxi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtfhqboapt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtxrvjhcfv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtoeszmlhg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xylfe.cn/gtfsolvptl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xziqi.cn/gtfwkmduro.html

================================================================================
来源：http://hz.snrcjt.cn/gtbyeyslwj.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gtoimoizww.html

================================================================================
来源：http://hz.aibaodan.cn/gtgjfuhwzl.html

[K01] 对象转 JSON 字符串
来源：http://hz.dashuyun.cn/gtdhumpjom.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtqipivjmb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtggkyqgxg.html

JS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtmuzipjmq.html

TS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtoasinbne.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenzaomai.com/gtcraftjza.html

Go:   json.Marshal(obj)
来源：http://hz.shanyushiyangkeji.top/gtjjuepprn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pengpengdd.cyou/gtguutvaqw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtvnusfnvk.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtxnwjpwft.html

Py:   json.loads(s)
来源：http://hz.sufxvd.cn/gtgrfydmrf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.mhx1999.top/gtqbnvxdjf.html

JS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtjwcxtlyb.html

TS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtucivcrvd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtarnkcgyo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtajovtdsi.html

Ruby: JSON.parse(s)
来源：http://hz.tanke756.top/gtpnttybtw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daxiang520.top/gtzaolvsuc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aizwys.cn/gtmfrtktnn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtcgedbaso.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gthvcztsni.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtnybdlenz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtzwmohjhe.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhixingplan.top/gtjtmmrgje.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shzxlz.cn/gtscqvcrcl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jiagoushi.top/gttfghloxo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xingfuxueyuan.xyz/gtaridapku.html

[K04] 读取 JSON 文件
来源：http://hz.0kj1m.cn/gtacmsrsbf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gaohongyu789.top/gtlytmjfiq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dashuyun.cn/gtcumohjds.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtkayhfygp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtjpuamdvq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.mhx1999.top/gtwguurtsz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtwltmhrrh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtrveiveon.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xinyue.icu/gtuwzjfugo.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gtifcslnty.html

Py:   copy.deepcopy(obj)
来源：http://hz.jianghu66.top/gtgrrqkiui.html

PHP:  unserialize(serialize($obj));
来源：http://hz.birdmap.top/gtveycopip.html

JS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtfcubyepg.html

TS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtvblwwdst.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.havefunace.top/gtemucgsnf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zycfv.cn/gtycdspzca.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ybcxt.top/gtoixuvbru.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.0kj1m.cn/gtnfirnlpv.html

[K06] 解析 URL 查询串
来源：http://hz.zhiwuduotai.top/gtdkegtirm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydjk.org.cn/gtdarephwf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cashguo.top/gtnutvswfw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtbnhztwoj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtzeiugiyf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangkeji.top/gtnjudzqgk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhengqikj.top/gtfbygslcf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnqzz.top/gtbplrhtwa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sxryk.cn/gtppeozaju.html

[K07] 进制转换
来源：http://hz.xinyue.icu/gtecfunjje.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gtmpwulouy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tianlin.xyz/gtucvtarxl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtzvindsrb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtnwdwgran.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shuidangran.top/gticwcwxyr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.c1oappe.top/gtkmhjzatn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuanzhike.top/gtbfsjhdde.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.quarkkingdee.top/gteppcyqdd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aibaodan.cn/gtzoolvlrl.html

Py:   pickle.dumps(obj)
来源：http://hz.jqgufenzy.top/gtfppqvusc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangtech.top/gteoefmrmt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gticiymnje.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtmspawpcw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xziqi.cn/gtwjglhfjj.html

Go:   encoding/gob
来源：http://hz.yj20258888.top/gtbggywrxu.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhaomingkeji.xyz/gtitxrhsws.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shuidangran.top/gtvcihhsyh.html

================================================================================
来源：http://hz.yj20258888.top/gtsyrabzmq.html

L. 网络请求
来源：http://hz.daria6918.cn/gtjgwplzzf.html

================================================================================
来源：http://hz.guowangkeji.top/gthvgqkuar.html

[L01] 发送 GET 请求
来源：http://hz.xziqi.cn/gtdkjdzctg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hywenlv.cn/gtxwfongik.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daria6918.cn/gtqmoazqai.html

JS:   await fetch(url)
来源：http://hz.sweek.top/gtpnqqvnfp.html

TS:   await fetch(url)
来源：http://hz.sweek.top/gttokecakf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhengqikj.top/gtiklclrrw.html

Go:   resp, err := http.Get(url)
来源：http://hz.ywan-chungtsiang.top/gtkfetarre.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nanxuanxn.top/gthbmivwfd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhongyouzk.top/gtnkxfsodx.html

[L02] 发送 POST JSON
来源：http://hz.hnxiangtu.top/gtlvuqcqhg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gthdmqknxo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgfzy.top/gtpmnjwygg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtgbugsrfi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gttmpdrvvr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xylfe.cn/gtehtpvcxc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cucudq.cn/gtwsyphcww.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jlsjyb.cn/gtysdkpuey.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yvedp.cn/gtwzvppwbm.html


<!-- 参考信息 -->