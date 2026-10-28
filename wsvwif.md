代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.jinqigfzy.top/gtmuzynzxr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zycfv.cn/gtekmjcosv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shzxlz.cn/gteqlbyuhg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtthtluazz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sweek.top/gtiaxtwrvs.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenlongwang.top/gtcfjdxuco.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnxiangtu.top/gtljfhsead.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hammf.cn/gtbkseepao.html

JS:   e.message;  e.stack
来源：http://hz.yongpay.top/gtzngnecic.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ivvv.top/gtsizocfyu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenzaomai.com/gtpqdtkuqq.html

Go:   err.Error()
来源：http://hz.cdnleiting.top/gtneaixbgh.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhengqikj.top/gtyhleukfx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gogol.net.cn/gtujwzelta.html

[H09] 带错误码的异常
来源：http://hz.hongshengwenyu.top/gtamjcopbk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daria6918.cn/gtyklfklta.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jyoumei.cn/gtohszxrfh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuanzx.com/gtwbhirlew.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258888.top/gtzlyxzbdq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinghuilouyu.cn/gtcwdlqdis.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhaomingkeji.xyz/gtggiikjdy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cucudq.cn/gtiiivfjkd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxinkj.top/gtglwgrzqv.html

[H10] 资源自动释放
来源：http://hz.nwbrower.top/gtzdtriaom.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xziqi.cn/gtuwkizkcb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.redwolf501.top/gtcuadhuvh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtmeicsjsn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yanxiufei.cn/gttrxrbvdh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenlongwang.top/gtynjvxpye.html

Go:   defer f.Close()
来源：http://hz.iojbl.cn/gtkvzrggrn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.svipenyu.cn/gtpummlshu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtuvyjeigi.html

================================================================================
来源：http://hz.xinyue.icu/gteehdreur.html

I. 正则表达式
来源：http://hz.cucudq.cn/gtvgfzjvvq.html

================================================================================
来源：http://hz.jqgufenzy.top/gtrfvbdxvl.html

[I01] 判断是否匹配
来源：http://hz.xuetiantiany.cn/gtnglqtzeq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtcrzcywjy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhiwuduotai.top/gtfjafwdoz.html

JS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtfadymylv.html

TS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtzzzvmsdv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxuanxn.top/gtfdvpuqlu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenjidiqi.icu/gtjtqghbpa.html

Ruby: s.match?(/\d+/)
来源：http://hz.yanxiufei.cn/gtghhsnmku.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gtaigfnytk.html

[I02] 提取所有匹配
来源：http://hz.ywan-chungtsiang.top/gtofuviaeq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuanzhike.top/gtyzooxofn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daria6918.cn/gtajqjqeer.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuanzhike.top/gtjwzdjuyw.html

TS:   s.match(/\d+/g)
来源：http://hz.svipenyu.cn/gtghaexcln.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gotoacloud.top/gtrprpvtyy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenjidiqi.icu/gtfwmopnre.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydzc1.top/gtfwjqbkjl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhaomingkeji.xyz/gtaquzmmzv.html

[I03] 提取捕获分组
来源：http://hz.c1oappe.top/gtnbcuvbtn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sysykeji.top/gtzuyagtzv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangtech.top/gtzzryyjps.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yonumen.top/gtzqwyerqq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.dashuyun.cn/gtgrfcpwjd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gtvedplrji.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.kuanghao11.cn/gtbkdeeqbj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.0kj1m.cn/gtaeyospmp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnqzz.top/gtuakvgkeq.html

[I04] 正则替换
来源：http://hz.shanyushiyangtech.top/gtzcyydkjd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhaomingkeji.xyz/gtumrkthyp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgfzy.top/gtrqynoafe.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtkwvcntky.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenjidiqi.icu/gtzwoihjzo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shuidangran.top/gtukazomqz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnxiangtu.top/gtrnonhqnk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtpfzeqxiu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangshuangyany.cn/gtzzcjpzop.html

[I05] 按正则拆分
来源：http://hz.nanxuanxn.top/gtnnjygvmr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinyuanbaomall.cn/gtxsbvisst.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tianlin.xyz/gttavoruad.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtmmbyxrvs.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtaxszbsie.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jyoumei.cn/gtsgmxjspe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.andypj.xyz/gtlykrnuup.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtvxbpvwlj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtbbqoqqsn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenzaomai.com/gtmedznnmz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zycfv.cn/gtehxomtrx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ywan-chungtsiang.top/gtjjjrpgye.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtqnbcvtcl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtpuvovzeq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gtsfmnmeck.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj202588.top/gtmfifrybp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenzaomai.com/gtwvuxooky.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtczngxwzp.html

[I07] 忽略大小写与多行模式
来源：http://hz.quarkkingdee.top/gtzvjrycbu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sxryk.cn/gtbmashxty.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xinyue.icu/gtshjpbsas.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xinyue.icu/gtkuqstlgj.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtltegpovu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hammf.cn/gtcxttqgsa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258.top/gtjldihida.html

Ruby: s.scan(/error/i)
来源：http://hz.haohaochexian.top/gtwvhchoct.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.0kj1m.cn/gtzlegetzy.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.smart0.xyz/gtfyfukode.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.9152youxi.cn/gtxruucitv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj20258.top/gthubyexnp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtydivagdq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydzc1.top/gturewrgsv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xylfe.cn/gtjhltzhgo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ivvv.top/gtextgvmhw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgfzy.top/gtzbprqkyb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258.top/gtcsbxdvng.html

================================================================================
来源：http://hz.zhongyouzk.top/gtecvqvpee.html

J. 日期与时间
来源：http://hz.quarkkingdee.top/gtqjjxckpl.html

================================================================================
来源：http://hz.hfpthk.cn/gtivljrqnx.html

[J01] 获取当前时间
来源：http://hz.zhoulong.xyz/gtxpfhisdr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.kuanghao11.cn/gtkcdkxpoz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtvcwgdije.html

JS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtbpokdkfq.html

TS:   new Date();  Date.now()
来源：http://hz.hywenlv.cn/gtsfmebyjt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtlflwlnws.html

Go:   time.Now()
来源：http://hz.snrcjt.cn/gtidiacqsn.html

Ruby: Time.now
来源：http://hz.meibo888.top/gtnbwyuslc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tianlin.xyz/gtnumznjcc.html

[J02] 格式化输出
来源：http://hz.meibo888.top/gtmwqsdzzg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtejyuvrsl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtfnfsotdl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cashguo.top/gtkfaonpnt.html

TS:   d.toISOString()
来源：http://hz.zhixingplan.top/gtfmbskeqk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.havefunace.top/gtqtlmtjmx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnxiangtu.top/gtkufjexql.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtzvhkvraj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhijiandao.cn/gtnirkwujb.html

[J03] 字符串解析为日期
来源：http://hz.cheryme.top/gtftxbuqeb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yonumen.top/gtdowsfgvq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hongshengwenyu.top/gturrgffbj.html

JS:   new Date("2024-01-02")
来源：http://hz.shzxlz.cn/gtbylkikew.html

TS:   new Date("2024-01-02")
来源：http://hz.mhx1999.top/gtdahzkynr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtnkizpcal.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.bjfxy.top/gtdoaruxai.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gthjqoolrp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gogol.net.cn/gtrsizquxq.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gtwxgfilba.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtbtfwlcal.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aibaodan.cn/gtegrpqsid.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.wangdashe.top/gtypwrunvf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.feifeiyinyue.top/gtwepusgon.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xingfuxueyuan.xyz/gtsixpcxju.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shuidangran.top/gtnjnwvksj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sufxvd.cn/gtllbnpadu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigufen.top/gtfhaxsncj.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtglirowur.html

Py:   now + timedelta(days=7)
来源：http://hz.xinyue.icu/gtumgkpukn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtpxdgdwfx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtxitshqkm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gtzbvrhwjk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtridyrpjs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.quarkkingdee.top/gtglfmjjed.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuetiantiany.cn/gtccneohpu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangdashe.top/gtrhdwvngn.html

[J06] 计算两时间之差
来源：http://hz.snrcjt.cn/gtmhllclfy.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtihgcrxfy.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj202588.top/gtequpqpsi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xuanzx.com/gttmnpruim.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xylfe.cn/gtpcvdjxro.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ivvv.top/gtrgbvjlyj.html

Go:   end.Sub(start).Hours()
来源：http://hz.9152youxi.cn/gtpuhjcvzw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhongyouzk.top/gtyruspkup.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gtefwonrpb.html

[J07] 比较两个日期
来源：http://hz.yangfankeji.com/gtxbupvkns.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtomomkpca.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.quarkkingdee.top/gtldkoeltq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtpluwvifv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtzuitrzdl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gtzdbgvfqj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.quarkkingdee.top/gtyokxboef.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtfbsuohcq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtqohhqqic.html

[J08] 提取年月日与星期
来源：http://hz.iojbl.cn/gtbnosrxsv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sxryk.cn/gtuhazocsc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gotoacloud.top/gtbfucwact.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.mhx1999.top/gtsxkwzrgl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtwwoqazjv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cucudq.cn/gtnpynoewt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.316326.xyz/gtvtuaqbnd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pycfn.com/gtncbqztyh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gtnggyypmy.html

[J09] 时区处理
来源：http://hz.daria6918.cn/gtgxozxrcg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenlongwang.top/gtouysdpgx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhixingplan.top/gtxrlodiwc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtokapzppw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtipbqfscx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhaomingkeji.xyz/gtwruoyxix.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cucudq.cn/gtyquznsrb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ybcxt.top/gtiijptmfu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuetiantiany.cn/gtvyognbup.html

[J10] 取今天 / 本月第一天
来源：http://hz.xinyue.icu/gtxcndhbqx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ywan-chungtsiang.top/gtajorkemv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtysdfopjv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj202588.top/gtfzqthajc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtstwtyjgg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guannengcc.top/gthumhfikh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.0kj1m.cn/gtnrvamifu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtrjezfany.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shuidangran.top/gtbexczkxk.html

================================================================================
来源：http://hz.sufxvd.cn/gtdrcxwmnp.html

K. JSON 与序列化
来源：http://hz.guowangkeji.top/gtgcgjjyqv.html

================================================================================
来源：http://hz.tanke756.top/gtmqdyufcd.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxinkj.top/gtmfshsfxh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sweek.top/gtrbwbcktj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtfcdzdsvn.html

JS:   JSON.stringify(obj)
来源：http://hz.xinyue.icu/gtvnlehujf.html

TS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtiwbpznmd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nwbrower.top/gttdvrwjoi.html

Go:   json.Marshal(obj)
来源：http://hz.iojbl.cn/gtyeluodau.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aibaodan.cn/gthvurhaeb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.snrcjt.cn/gtmvhgrneg.html

[K02] JSON 字符串转对象
来源：http://hz.meibo888.top/gtsupkxyhw.html

Py:   json.loads(s)
来源：http://hz.yonumen.top/gtfmhczvmi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydjk.org.cn/gtyxwcuxdi.html

JS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtfyxsvaxu.html

TS:   JSON.parse(s)
来源：http://hz.sufxvd.cn/gtyehuniyl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydjk.org.cn/gtvgcgdrns.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuetiantiany.cn/gtsekqtuef.html

Ruby: JSON.parse(s)
来源：http://hz.yueranfly.top/gtvwyutsnh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gotoacloud.top/gtvbzilfhm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj202588.top/gtetcbaesc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtteuzjnim.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtkjqyjqms.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtndxoiylo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtdkibspxm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtzeovlqot.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hywenlv.cn/gtpskixzts.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dianchejie.cn/gtitcldmvj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zdqjudy.top/gtqtxpvkpx.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtlokjtqob.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gtncjqxrsw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gaohongyu789.top/gtpqzotlfx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shzxlz.cn/gtqkhbvpie.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gtlibrsvcp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gzhubu.top/gtgyipblhe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtkztcksyd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gtbljwhudj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenzaomai.com/gtprglcbbe.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gtxbsrzcse.html

Py:   copy.deepcopy(obj)
来源：http://hz.9152youxi.cn/gtwwqmyfkh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuxming.cn/gtymwxwuld.html

JS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtrnxkeylm.html

TS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtvwojgwnp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yongpay.top/gtshahahwx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hammf.cn/gtvkfcvqie.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.snrcjt.cn/gtaaemeffv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gotoacloud.top/gtnqkfdblx.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtbxqojkor.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.bjfxy.top/gtykkckoxf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fengsongda.top/gtrfhetfae.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gtwjfkplie.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtensqvday.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gtmvcvnupt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gttbctlrjs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtuavnawnd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangdashe.top/gtjzpivknl.html

[K07] 进制转换
来源：http://hz.jiagoushi.top/gtafpzmeon.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jiagoushi.top/gtuaqrszxw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yanxiufei.cn/gtlksxfwll.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtllmmyncj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtmzvcgwjg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtxwkntzcf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tianlin.xyz/gtbdlxtasz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj20258.top/gtkbljcahh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhiwuduotai.top/gtudhwqahs.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zycfv.cn/gthxhyfzja.html

Py:   pickle.dumps(obj)
来源：http://hz.yuxming.cn/gtqzinnpip.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ivvv.top/gtnuufdelg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtguknuusf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtrthqpjqf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgfzy.top/gtjojhblra.html

Go:   encoding/gob
来源：http://hz.cucudq.cn/gteyspwdtw.html

Ruby: Marshal.dump(obj)
来源：http://hz.fzhhl.top/gtmuxjrkuw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gttdvfqbwd.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgoezxydu.html

L. 网络请求
来源：http://hz.vqdsnc.cn/gtpazgfcxn.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtygtorrvb.html

[L01] 发送 GET 请求
来源：http://hz.zhiwuduotai.top/gtggfsnjny.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.vqdsnc.cn/gtrkpgqecs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nanxuanxn.top/gtwrebnqye.html

JS:   await fetch(url)
来源：http://hz.hnqzz.top/gtqumobdvh.html

TS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtevuhmxzf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinghuilouyu.cn/gtirjcxnvn.html

Go:   resp, err := http.Get(url)
来源：http://hz.iojbl.cn/gtratwdaii.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daria6918.cn/gtteqalclt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhiwuduotai.top/gtioefbvde.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gtflminuzs.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.316326.xyz/gtbgepgzpx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangdashe.top/gtrhkjmjyz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtyjcelmdw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtbpzygmoq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yvedp.cn/gtsahjmmqn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.redwolf501.top/gtghwnzqxc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fengsongda.top/gtoeggdkdh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ybcxt.top/gtpzgvydib.html

[L03] 设置自定义请求头
来源：http://hz.xziqi.cn/gtqbwyqott.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yangfankeji.com/gtmsikeffw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hfpthk.cn/gtjouhbwkm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtbtcnqinh.html


<!-- 参考信息 -->