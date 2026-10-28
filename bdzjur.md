代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtqyubfvgx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hongshengwenyu.top/gtfcplvudp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.andypj.xyz/gtinfbwwmz.html

C#:   obj?.A?.B ?? default
来源：http://hz.vqdsnc.cn/gtorwvulxq.html

[H07] 断言
来源：http://hz.smart0.xyz/gthqvsjdkf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xylfe.cn/gtgkdxyacm.html

PHP:  assert($x > 0);
来源：http://hz.xziqi.cn/gtducavfyd.html

JS:   console.assert(x > 0);
来源：http://hz.tian-w.cn/gttiogdzdh.html

TS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtbzgvkuyr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.quarkkingdee.top/gtoryzmnne.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangshuangyany.cn/gtryctlvwn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jyoumei.cn/gtxgxuwrer.html

C#:   Debug.Assert(x > 0);
来源：http://hz.316326.xyz/gthosujcia.html

[H08] 获取错误信息与堆栈
来源：http://hz.zycfv.cn/gtuwnssafl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhengqikj.top/gthtgcrkme.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.bjfxy.top/gtiemqhqbx.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gtjzmwydtg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigfzy.top/gthbpcemae.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pycfn.com/gtnrkvtxrd.html

Go:   err.Error()
来源：http://hz.feifeiyinyue.top/gtsyxknonq.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgfzy.top/gtsgxdugef.html

C#:   e.Message;  e.StackTrace
来源：http://hz.svipenyu.cn/gtgmalhoab.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtcfuvnkqk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sxryk.cn/gtdlcbdaar.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gttpgdsubl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xylfe.cn/gtivdxyohl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gaohongyu789.top/gthenfoftj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtywmopqej.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fengsongda.top/gtmcolrtni.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jlsjyb.cn/gtvdqrhgbq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.feifeiyinyue.top/gtvuizmcaj.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtujhmlcqb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gtfkssordg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ehwqpu.com/gtjdxqkhxw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenjidiqi.icu/gtesircyhv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ivvv.top/gtfjylvkme.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xylfe.cn/gtowumpgze.html

Go:   defer f.Close()
来源：http://hz.cqqwz.cn/gtjoaxdyld.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hywenlv.cn/gtbeissmyf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tanke756.top/gtbanjyrgh.html

================================================================================
来源：http://hz.dianchejie.cn/gttgrvuihf.html

I. 正则表达式
来源：http://hz.nanxinkj.top/gtjqxeumxr.html

================================================================================
来源：http://hz.guowangkeji.top/gtrtnehvqi.html

[I01] 判断是否匹配
来源：http://hz.yj20258.top/gtxxiqpghc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtjhzqlhzn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhoulong.xyz/gtuuabcudn.html

JS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtpgqvryri.html

TS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtktphsufr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zycfv.cn/gtarjbvvxg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnxiangtu.top/gtcvskxdql.html

Ruby: s.match?(/\d+/)
来源：http://hz.tanke756.top/gtlebbacxr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hysaishi.cn/gtounokblj.html

[I02] 提取所有匹配
来源：http://hz.bjfxy.top/gtvqlipwhr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fzhhl.top/gtrkqcaefm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.svipenyu.cn/gtckzuhlfp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gtfvnlmayy.html

TS:   s.match(/\d+/g)
来源：http://hz.jiagoushi.top/gtdcjvgnuk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ivvv.top/gtzzkkfcui.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuxming.cn/gtwurbnmqv.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnxiangtu.top/gtlcbxvsjz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gogol.net.cn/gtsfuxurds.html

[I03] 提取捕获分组
来源：http://hz.hysaishi.cn/gthubexwxr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cashguo.top/gtvxijtgku.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sufxvd.cn/gtmetqjpjf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yvedp.cn/gtyseoiphq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hfpthk.cn/gtzmzzvojx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ydzc1.top/gttprlumkm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenjidiqi.icu/gtieeiszwo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhaomingkeji.xyz/gttwrniyln.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhixingplan.top/gtooebdanp.html

[I04] 正则替换
来源：http://hz.yanxiufei.cn/gtffsgakuy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtprutwvpk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtcdvymaea.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fzhhl.top/gtrqqbnucd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.daxiang520.top/gtdvdlmwtu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangdashe.top/gtveaxjhnd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhijiandao.cn/gtvceoesdd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daria6918.cn/gttqyvfdom.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zycfv.cn/gtnhmkrftz.html

[I05] 按正则拆分
来源：http://hz.gzhubu.top/gtjduydvdg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhixingplan.top/gtahhjtgdv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dashuyun.cn/gtkhwztepa.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtlzgaztao.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtkjjsseis.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zdqjudy.top/gtcgjjryql.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.quarkkingdee.top/gtjklqxqrm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtspossjvm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigfzy.top/gtitgfnihd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yonumen.top/gtmleoepmv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtapmpbbki.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhaomingkeji.xyz/gttsdadrkm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtddqllxax.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gttdwunbyt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtmvgzzkyj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shanyushiyangkeji.top/gtelwaaita.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.0kj1m.cn/gtlxfiustr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtaltahpri.html

[I07] 忽略大小写与多行模式
来源：http://hz.dashuyun.cn/gtrlkuzvhw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenjidiqi.icu/gtsfmmllmr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtdltwtvku.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnxiangtu.top/gtzbfcymdk.html

TS:   /error/gim
来源：http://hz.daria6918.cn/gtcgyjcmwi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xylfe.cn/gtqlwojwsx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.iojbl.cn/gtbronhqbo.html

Ruby: s.scan(/error/i)
来源：http://hz.chenzaomai.com/gtgsqbbnne.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.52xcode.cn/gtqjuytxrj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gogol.net.cn/gtdzzlpajv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydzc1.top/gtedchzeyi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.52xcode.cn/gtycxbtmnw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtsffswsqm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtfcoebevr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtiaqoxslg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jlsjyb.cn/gtpfolhkpa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenzaomai.com/gttjprfgpy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.316326.xyz/gtzhpalwpe.html

================================================================================
来源：http://hz.snrcjt.cn/gttqdnuaoy.html

J. 日期与时间
来源：http://hz.gogol.net.cn/gtrrprtknx.html

================================================================================
来源：http://hz.aibaodan.cn/gtdsopmmdy.html

[J01] 获取当前时间
来源：http://hz.zhoulong.xyz/gtruvhlqho.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shzxlz.cn/gtutfunjmq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sysykeji.top/gtybjjpnvc.html

JS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtgqmjhdvy.html

TS:   new Date();  Date.now()
来源：http://hz.gotoacloud.top/gtergiheox.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinyuanbaomall.cn/gttvzvhmrc.html

Go:   time.Now()
来源：http://hz.jqgfzy.top/gtjjfukqos.html

Ruby: Time.now
来源：http://hz.xingfuxueyuan.xyz/gtmzigsupk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgfzy.top/gtszcvkjrl.html

[J02] 格式化输出
来源：http://hz.ivvv.top/gtcgxuwugp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gtlbnbhfvh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gthybmocuv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj202588.top/gtxeiaseqt.html

TS:   d.toISOString()
来源：http://hz.xuanzx.com/gtrcsescbk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hfpthk.cn/gtibfwrlxt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xylfe.cn/gtpppunefk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gtpcvmdiam.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yueranfly.top/gtllhokwvz.html

[J03] 字符串解析为日期
来源：http://hz.birdmap.top/gthtzfjctj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.bjfxy.top/gtqjxiwqof.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hysaishi.cn/gtftiwvyoq.html

JS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gtbasdsoxm.html

TS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtqvtdqjue.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtbndffpjv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.fengsongda.top/gtcxmnqigq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ydjk.org.cn/gtvwpciavt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cashguo.top/gtuvrtltis.html

[J04] 时间戳与日期互转
来源：http://hz.ybcxt.top/gtuikklivu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sxryk.cn/gtnqkvnqxi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ivvv.top/gtypxiwwwr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.svipenyu.cn/gtczgvupmb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydjk.org.cn/gtbtcezqjn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cashguo.top/gttxtrwpep.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258.top/gtlcuezmxj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guannengcc.top/gtlbnpgowj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.aizwys.cn/gtclsaruqi.html

[J05] 时间加减（加 7 天）
来源：http://hz.gogol.net.cn/gtudvysssy.html

Py:   now + timedelta(days=7)
来源：http://hz.nanxinkj.top/gtbhffwfyy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hysaishi.cn/gtmiiijyjc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gtpwqdmxrn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtlwsytrfz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tianlin.xyz/gtzwaqkvgx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cheryme.top/gtvqbctkzu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhiwuduotai.top/gtklncpujx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.guannengcc.top/gtqxbfmlkq.html

[J06] 计算两时间之差
来源：http://hz.shzxlz.cn/gtzefxrcgq.html

Py:   (end - start).total_seconds()
来源：http://hz.gotoacloud.top/gtwmteplsh.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgfzy.top/gtnkucbhgu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ybcxt.top/gtxqqrxhii.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.fzhhl.top/gtjldpjpqa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gtbijgkkxb.html

Go:   end.Sub(start).Hours()
来源：http://hz.feifeiyinyue.top/gthaeyflqy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shuidangran.top/gtnmuzlgom.html

C#:   (end - start).TotalSeconds
来源：http://hz.ywan-chungtsiang.top/gtvjfysbph.html

[J07] 比较两个日期
来源：http://hz.hywenlv.cn/gtxzscpdcq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtmgzuzfak.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.haohaochexian.top/gtaxjxdofh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtszaghvkp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtolonisib.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ppjwa.cn/gtthavwfio.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydjk.org.cn/gtyqxvumav.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtlelfpvtd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtdmejautr.html

[J08] 提取年月日与星期
来源：http://hz.zhixingplan.top/gtkkuxvwll.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ydzc1.top/gtpixgphyd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wangdashe.top/gtdnzqmbag.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhengqikj.top/gtmzyfavpz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj202588.top/gtzezvdiso.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ehwqpu.com/gtydajpopd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gogol.net.cn/gtcnitqmvc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtmjjvfxog.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258.top/gtjzbtxehq.html

[J09] 时区处理
来源：http://hz.yongpay.top/gtbxrikujy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhaomingkeji.xyz/gtyzyjkeiv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtjmpumoge.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtjrgticxf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gthqpzlgvq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gogol.net.cn/gtpjssjrla.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guannengcc.top/gtjynsqhri.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.c1oappe.top/gtevtfjagg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yongpay.top/gtjbnrdizo.html

[J10] 取今天 / 本月第一天
来源：http://hz.mhx1999.top/gtuoyovolw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hfpthk.cn/gtsjecrkpk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.c1oappe.top/gtglpxwtin.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.bjfxy.top/gtmaphwohc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tianlin.xyz/gtckajfbmv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gtwllbwmht.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cheryme.top/gtbgionopm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhiwuduotai.top/gtqmqazpyy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydzc1.top/gtlhalpyof.html

================================================================================
来源：http://hz.andypj.xyz/gtyfbkqmsp.html

K. JSON 与序列化
来源：http://hz.ppjwa.cn/gtxtiqtanr.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtspawwvcg.html

[K01] 对象转 JSON 字符串
来源：http://hz.316326.xyz/gtmxgeerau.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pycfn.com/gttnarainh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtelzejohr.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtuqkxphpj.html

TS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtvddrkiuy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj20258888.top/gtnikyjvvj.html

Go:   json.Marshal(obj)
来源：http://hz.0kj1m.cn/gtagdeptyy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.iojbl.cn/gtamqxpqzu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.0kj1m.cn/gtyffjoeph.html

[K02] JSON 字符串转对象
来源：http://hz.ywan-chungtsiang.top/gtffabsjiy.html

Py:   json.loads(s)
来源：http://hz.shangyingyoupin.top/gtfngawwtr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guannengcc.top/gtdfgfhquo.html

JS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtfnustmkt.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gttyloutij.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tianlin.xyz/gtfhbmtmqg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tianlin.xyz/gtrzinrdmd.html

Ruby: JSON.parse(s)
来源：http://hz.nanxinkj.top/gttqnwjnfg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigfzy.top/gtvojjinvw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinyuanbaomall.cn/gtsabwfnzd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtvfxdduxs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtkfecdibf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gthceqsvcm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtogffmyas.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhixingplan.top/gtapfnkoub.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zycfv.cn/gtqrnmhavt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daxiang520.top/gtobwifvuf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.havefunace.top/gtkrtdmuci.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtgdopstai.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.redwolf501.top/gtlnxtntcs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.feifeiyinyue.top/gtelsnqbxx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtknpxxhys.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gthdglkwvp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.quarkkingdee.top/gtombjmsyc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtxojpsdgz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shangyingyoupin.top/gtnbiodzfe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yangfankeji.com/gtfscnmhnw.html

[K05] 深拷贝对象
来源：http://hz.redwolf501.top/gtbhvfhjwa.html

Py:   copy.deepcopy(obj)
来源：http://hz.cheryme.top/gteermykcu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.meibo888.top/gtplowsbge.html

JS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtninzaenm.html

TS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtjfghcmja.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cdnleiting.top/gthljmhukb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.0kj1m.cn/gtbxkdnske.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgufenzy.top/gtwxkxacdm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhijiandao.cn/gthueyrmlk.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtkyfhqztc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shuidangran.top/gtbpeklfle.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtwhdowedc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gttmnbyqpp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtcoizaxsu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tian-w.cn/gtsktxlkog.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cqqwz.cn/gtkxlwutth.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtcaysmulp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pengpengdd.cyou/gtofyuubtl.html

[K07] 进制转换
来源：http://hz.dashuyun.cn/gtbpyovtqo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.0kj1m.cn/gtbmlisxgj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daria6918.cn/gtgzvtugwe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtiguedzbc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtbnyxiftt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zycfv.cn/gthalwkkhv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.snrcjt.cn/gtbwqlzlmn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtrdeutmwy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daxiang520.top/gtduoijkqe.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgufenzy.top/gtbcczudnw.html

Py:   pickle.dumps(obj)
来源：http://hz.daria6918.cn/gtcgxcpsmn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ivvv.top/gtqgklxckj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtttjungfa.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtinivgxzy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tianlin.xyz/gtbrsdogjw.html

Go:   encoding/gob
来源：http://hz.guowangkeji.top/gtjkgbjkpo.html

Ruby: Marshal.dump(obj)
来源：http://hz.hfpthk.cn/gtaqsouvyy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yonumen.top/gtnlfhphxp.html

================================================================================
来源：http://hz.sxryk.cn/gtqljdbhhl.html

L. 网络请求
来源：http://hz.jinqigfzy.top/gtgjtyahlk.html

================================================================================
来源：http://hz.snrcjt.cn/gtoqwtfeqx.html

[L01] 发送 GET 请求
来源：http://hz.svipenyu.cn/gtluvuxyly.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhijiandao.cn/gtanrjmnwu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cqqwz.cn/gtyrqxejyl.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtoyfqokcq.html

TS:   await fetch(url)
来源：http://hz.0kj1m.cn/gtcjqldzxq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.mhx1999.top/gtcwngztue.html

Go:   resp, err := http.Get(url)
来源：http://hz.dianchejie.cn/gtzfrgdxvk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sxryk.cn/gtuuglylyx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gogol.net.cn/gtyqqcqcsh.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtdbhnompb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj202588.top/gthpdfnhuq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ivvv.top/gthfebcgig.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtuceydsxs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtbrkshriw.html


<!-- 参考信息 -->