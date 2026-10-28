代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.jlsjyb.cn/gtsnhhotgr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cdnleiting.top/gtulgfptiz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.316326.xyz/gtuepsvtvs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xziqi.cn/gteapdmkqs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tanke756.top/gtpcgdagnh.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gtrouaqrua.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.svipenyu.cn/gtoluqswfd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.iojbl.cn/gtjqhirlib.html

JS:   e.message;  e.stack
来源：http://hz.mhx1999.top/gtldfbqijo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cucudq.cn/gtvmnxwayc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aibaodan.cn/gtherkrbzz.html

Go:   err.Error()
来源：http://hz.yuxming.cn/gtwittldqz.html

Ruby: e.message;  e.backtrace
来源：http://hz.hammf.cn/gtxnlgluuk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.snrcjt.cn/gtxngcrkqp.html

[H09] 带错误码的异常
来源：http://hz.nanxuanxn.top/gtycabvgla.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.guowangkeji.top/gtggvwodsa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.bjfxy.top/gtwviicdyg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shangyingyoupin.top/gtooxyuomr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigufen.top/gtpjkqioeh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aizwys.cn/gtnsfljcjc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cucudq.cn/gttpeivvgo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenlongwang.top/gtbyogcxhm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cheryme.top/gtiqzctczy.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtqdwkivfi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gotoacloud.top/gttkunelkn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daxiang520.top/gtggnpejrg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtevqurmtc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtypggjvrv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydjk.org.cn/gtjbgheynl.html

Go:   defer f.Close()
来源：http://hz.bjfxy.top/gtawlhpnnl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.316326.xyz/gtqlqasgly.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.quarkkingdee.top/gtvvrwgwgh.html

================================================================================
来源：http://hz.aizwys.cn/gturvkhpau.html

I. 正则表达式
来源：http://hz.aizwys.cn/gtxyxbfncl.html

================================================================================
来源：http://hz.snrcjt.cn/gtydpadywv.html

[I01] 判断是否匹配
来源：http://hz.haohaochexian.top/gtowxnktsg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtxgiszkvu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.pengpengdd.cyou/gticmgullh.html

JS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gthdulyact.html

TS:   /\d+/.test(s)
来源：http://hz.ywan-chungtsiang.top/gtofiavlzc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhixingplan.top/gttvoaplvs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nanxinkj.top/gtfazolhns.html

Ruby: s.match?(/\d+/)
来源：http://hz.jyoumei.cn/gtslohsifq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhixingplan.top/gtmwzxeqkt.html

[I02] 提取所有匹配
来源：http://hz.meibo888.top/gtudyjxkpr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gtbmcqajvd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenjidiqi.icu/gtdowfcnpx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhixingplan.top/gtzxlvhdrj.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtypuxhtvc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.kuanghao11.cn/gtkuthdmge.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.iojbl.cn/gthuutctfb.html

Ruby: s.scan(/\d+/)
来源：http://hz.wangdashe.top/gtrqkmhhui.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydzc1.top/gtigspirha.html

[I03] 提取捕获分组
来源：http://hz.hnqzz.top/gtgguenmbl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.quarkkingdee.top/gttewtsvll.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hysaishi.cn/gtapdugwnr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhoulong.xyz/gturpvyhra.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtyvukmjxm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gogol.net.cn/gtypcyfwrc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.0kj1m.cn/gtxlrhznpg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hysaishi.cn/gtrbegponc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinghuilouyu.cn/gtzlxbyzju.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtziepjcfo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangtech.top/gtxefhpzge.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.snrcjt.cn/gtbnkilnmp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtnsddjsxa.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtxatnbuge.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.svipenyu.cn/gtlnslbbdb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.bjfxy.top/gtujtfdehz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.aizwys.cn/gtqlozgwcn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.svipenyu.cn/gtvmvooqsc.html

[I05] 按正则拆分
来源：http://hz.ydjk.org.cn/gthdbehqto.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnxiangtu.top/gtcwpsnggu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yangfankeji.com/gtblfasigz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtlawivdvb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtzzavfndw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cucudq.cn/gtmhxkrvkb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sxryk.cn/gtjfasmjzs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtmkahvjfl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gzhubu.top/gtxoyrujig.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fzhhl.top/gtrzzdidta.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtyqpqdprf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.birdmap.top/gtfchtajda.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtmcjbggpi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cheryme.top/gtlxfzojmy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dashuyun.cn/gtqrwwngzr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.mhx1999.top/gtxalldpbj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ehwqpu.com/gtmjunhaaz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtfonbmjdi.html

[I07] 忽略大小写与多行模式
来源：http://hz.nwbrower.top/gtkoequcux.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sxryk.cn/gtcwrshjpz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenlongwang.top/gtrtntgnbq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gtynpxduqk.html

TS:   /error/gim
来源：http://hz.0kj1m.cn/gtvkjoztlf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtloapstqw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jianghu66.top/gtfjvntejq.html

Ruby: s.scan(/error/i)
来源：http://hz.gaohongyu789.top/gtbcifdtht.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangkeji.top/gtkwwqxaea.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.guowangkeji.top/gthvsyahmk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gtenbpogbg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yongpay.top/gtttawrmsn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtmlezfatq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtigukbrwl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtvkevfcmq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.c1oappe.top/gtyjadjpca.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.smart0.xyz/gtevujvwsn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtkxwcpgam.html

================================================================================
来源：http://hz.gogol.net.cn/gteenankfz.html

J. 日期与时间
来源：http://hz.nanxuanxn.top/gtndimwkts.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtarbnwfse.html

[J01] 获取当前时间
来源：http://hz.dashuyun.cn/gtacdxzlwh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigufen.top/gtjcfncgte.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gturwxcwzr.html

JS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtdudhcasd.html

TS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtzfdilglt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.c1oappe.top/gtrjapecap.html

Go:   time.Now()
来源：http://hz.jinyuanbaomall.cn/gtdawlxszu.html

Ruby: Time.now
来源：http://hz.yuanzhike.top/gtihehbrsv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinghuilouyu.cn/gtrfbglcjx.html

[J02] 格式化输出
来源：http://hz.hysaishi.cn/gtfdbmmmsj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtsrnprkbj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtfbhjonvm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shzxlz.cn/gtutgbvxks.html

TS:   d.toISOString()
来源：http://hz.guowangkeji.top/gtaiigumqk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yonumen.top/gtmgwjnwhv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fzhhl.top/gtnzihozmk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xylfe.cn/gtsmoaxfxf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.iojbl.cn/gtaxbaqnhv.html

[J03] 字符串解析为日期
来源：http://hz.birdmap.top/gtvmmxilcq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.iojbl.cn/gtcetlwpfb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigfzy.top/gtlqyupxbj.html

JS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtotpetszu.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtkxskizdj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtzzbxoylf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258.top/gtevjqwjhf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtnxrrytce.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuetiantiany.cn/gtfildkpzt.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtsorkuwlh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgfzy.top/gthkwnzafg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zycfv.cn/gtilhclryb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.iojbl.cn/gtdjcwaqxr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.aizwys.cn/gtadxlcoio.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnxiangtu.top/gtvkyclmkd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangkeji.top/gtfxjkmvtq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258888.top/gtatdvmswj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.svipenyu.cn/gtwnuccfuy.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangkeji.top/gtjqhxqxij.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgfzy.top/gtftbhseuu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sysykeji.top/gtkwxhwvbl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtxhmtczuv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtbcuziqjb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.feifeiyinyue.top/gttklbiyfm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnqzz.top/gtbxywvpoh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.bjfxy.top/gtychbbjkg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinyuanbaomall.cn/gtiagtqbdy.html

[J06] 计算两时间之差
来源：http://hz.svipenyu.cn/gtgtblcbeb.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gtoszrctbq.html

PHP:  $end->diff($start)->days;
来源：http://hz.yueranfly.top/gtahvxjjau.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.feifeiyinyue.top/gtqwmvxhhi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yvedp.cn/gtxrydjbam.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.52xcode.cn/gtrggxiiih.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gtkfzxxyvo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.quarkkingdee.top/gtzcfskqce.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangtech.top/gtqnkhpund.html

[J07] 比较两个日期
来源：http://hz.daxiang520.top/gtxszsngsj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtqrvqrmio.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinqigfzy.top/gtzvfkirur.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtasmxdwog.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtoipzygzu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shuidangran.top/gtdnafervd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.fzhhl.top/gttvxhjeqi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtbwlttoxx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtxnjlngwo.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gtadlfbbqf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hongshengwenyu.top/gtxpnijhoa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yuxming.cn/gtvsjemhfw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daria6918.cn/gtmxqfxjcp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtcnbazsmo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigufen.top/gtppftjutj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nwbrower.top/gtpsshroaz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuanzhike.top/gtlfoumnxy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtlociwrxq.html

[J09] 时区处理
来源：http://hz.andypj.xyz/gtlkzlrjvn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dianchejie.cn/gtewjjnhre.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cashguo.top/gthighxblw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtspnlesra.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtgdtqyrez.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guowangkeji.top/gthntihaek.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxuanxn.top/gtvovugezu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jlsjyb.cn/gtrhuhccyg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gtluxebwbb.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gtdklnwgmh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cdnleiting.top/gtzaxqnyxk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgufenzy.top/gtqabgktoz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigfzy.top/gtdlrqrrzx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.redwolf501.top/gtaspzazga.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtbzywnefs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtdlnmbbgg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.fzhhl.top/gtbwkmqqlo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.haohaochexian.top/gtnpdjaqbm.html

================================================================================
来源：http://hz.ybcxt.top/gttdgkashh.html

K. JSON 与序列化
来源：http://hz.cheryme.top/gtjrpdotcv.html

================================================================================
来源：http://hz.cashguo.top/gtanaeoqcv.html

[K01] 对象转 JSON 字符串
来源：http://hz.hammf.cn/gtbvqvresa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtxbzzagnd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtdoktcfvl.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtxusqwnmw.html

TS:   JSON.stringify(obj)
来源：http://hz.birdmap.top/gtbzcazgco.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenlongwang.top/gtnpnqtzja.html

Go:   json.Marshal(obj)
来源：http://hz.nanxinkj.top/gtxmeztpil.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xingfuxueyuan.xyz/gtdhybkayv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtwqydanah.html

[K02] JSON 字符串转对象
来源：http://hz.fengsongda.top/gthaovmypr.html

Py:   json.loads(s)
来源：http://hz.hammf.cn/gtftpewxfc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xziqi.cn/gtqucctohm.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtkimybvcg.html

TS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtzcsaynsy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cucudq.cn/gtcbwlkbsm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gttlsjpkql.html

Ruby: JSON.parse(s)
来源：http://hz.cheryme.top/gtcbjwiara.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhijiandao.cn/gtqxmfjlhm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtwbuyxcjn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtjacqehop.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtnyumhzjt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gthcsbujcr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gtssdaxaad.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.haohaochexian.top/gtxmiwedua.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuxming.cn/gtagwypvop.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gogol.net.cn/gtudidprmp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shangyingyoupin.top/gtanhmhilk.html

[K04] 读取 JSON 文件
来源：http://hz.haohaochexian.top/gtpokuyqch.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.birdmap.top/gtaaptwyvx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fengsongda.top/gtszlxyrit.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtbsevbkzi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gteixtmhqh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.c1oappe.top/gtdfceavgg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtyoungooc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.birdmap.top/gtmkasjigd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gogol.net.cn/gtkafgquvr.html

[K05] 深拷贝对象
来源：http://hz.daria6918.cn/gtpzuwanti.html

Py:   copy.deepcopy(obj)
来源：http://hz.yonumen.top/gtftvbkvle.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj20258.top/gteeexbbic.html

JS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gtzmjpmlik.html

TS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtxxpqnvck.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.0kj1m.cn/gtymtiydhr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cashguo.top/gtuqjpzmym.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jiagoushi.top/gtgiwkefvl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtckkcfhuw.html

[K06] 解析 URL 查询串
来源：http://hz.nanxuanxn.top/gteginobzs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hywenlv.cn/gtwpizfakp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cdnleiting.top/gtkvcoxbnn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtcwckmris.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gzhubu.top/gtmxhyqnyd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnxiangtu.top/gtoehxlisc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.andypj.xyz/gtklzostxi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtrcbxppsl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtymzgimam.html

[K07] 进制转换
来源：http://hz.ppjwa.cn/gtzrgfdbdt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtwytuxytk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guowangkeji.top/gthyhedjny.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gthgxiamvs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtjzqtedoa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtsjrgtllf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtnefadcmr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cheryme.top/gtqejfegyb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtgaibwweb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jyoumei.cn/gtqasckzsz.html

Py:   pickle.dumps(obj)
来源：http://hz.haohaochexian.top/gtnfqbxdkz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigufen.top/gtoodczsaz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gzhubu.top/gtxppvwxiq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtomitjcuj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnxiangtu.top/gtyumlupmz.html

Go:   encoding/gob
来源：http://hz.yvedp.cn/gtlsogukws.html

Ruby: Marshal.dump(obj)
来源：http://hz.ehwqpu.com/gtwpygkynp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.iojbl.cn/gtgvarpbok.html

================================================================================
来源：http://hz.fzhhl.top/gtirkihvbb.html

L. 网络请求
来源：http://hz.birdmap.top/gtvogazwlk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtleuwaghy.html

[L01] 发送 GET 请求
来源：http://hz.cheryme.top/gtqmdgbcrw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hammf.cn/gtmvlkwbhr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgfzy.top/gtoldnttal.html

JS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtnogmjcai.html

TS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gtvjlwvkgy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtfqxwgcpn.html

Go:   resp, err := http.Get(url)
来源：http://hz.daxiang520.top/gtqjbfcywb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigfzy.top/gtpgbsftxr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.52xcode.cn/gtofbtyaut.html

[L02] 发送 POST JSON
来源：http://hz.birdmap.top/gtfiwmliat.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gthlvbhweh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gzhubu.top/gtocdynejb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtrjywhwij.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.9152youxi.cn/gtwhrypckr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yongpay.top/gtnbdqvpne.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hysaishi.cn/gtdbievmhb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gtbfxjmjnl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daxiang520.top/gtmippwlaf.html

[L03] 设置自定义请求头
来源：http://hz.jinghuilouyu.cn/gtdhihcwry.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigfzy.top/gtccpknvpk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.dianchejie.cn/gtnkleylnw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtvvfesrby.html


<!-- 参考信息 -->