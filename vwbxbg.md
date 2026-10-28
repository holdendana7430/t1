代发 wailian999

Py:   value = d.get("k") or default
来源：http://hz.hysaishi.cn/gtxzwszdny.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtsfufvgvw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtpertzvsj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtngikbjfo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.meibo888.top/gtdvzxzhue.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangshuangyany.cn/gtoinbqvhs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cashguo.top/gtbnyttjqq.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhixingplan.top/gtzpdqyadm.html

[H07] 断言
来源：http://hz.yuxming.cn/gttgslziee.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jlsjyb.cn/gtjufohprh.html

PHP:  assert($x > 0);
来源：http://hz.pycfn.com/gtqdperfta.html

JS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtcgafakvk.html

TS:   console.assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtkyqpfpao.html

Java: assert x > 0 : "必须为正";
来源：http://hz.redwolf501.top/gtzclsqrcc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.quarkkingdee.top/gtatnganhl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtcksjaslj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtkvvthkrg.html

[H08] 获取错误信息与堆栈
来源：http://hz.sufxvd.cn/gtlbjpxlbq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuanzx.com/gtpfuinfux.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tian-w.cn/gthccvtwos.html

JS:   e.message;  e.stack
来源：http://hz.ppjwa.cn/gtxlompgui.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.iojbl.cn/gtnflzqkph.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dashuyun.cn/gtvubqnmrm.html

Go:   err.Error()
来源：http://hz.hammf.cn/gtsuaaapgq.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigfzy.top/gtvtawdtmi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtxvjkjwkc.html

[H09] 带错误码的异常
来源：http://hz.svipenyu.cn/gtplhpbdwq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.kuanghao11.cn/gtyhfnsbre.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinyuanbaomall.cn/gtggidkjqa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj202588.top/gtsvtjyuyl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnqzz.top/gtosyyboyc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.feifeiyinyue.top/gtdyjondhs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtqxbazbfh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gogol.net.cn/gtecbyvohb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnqzz.top/gtatzthpjt.html

[H10] 资源自动释放
来源：http://hz.snrcjt.cn/gtiendmeji.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtbfscerut.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hongshengwenyu.top/gtxfctkcbk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shuidangran.top/gtslmcnuel.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gteqlcacif.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gzhubu.top/gthehzhlkz.html

Go:   defer f.Close()
来源：http://hz.zdqjudy.top/gtdhtctvpl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cqqwz.cn/gtajlufutp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigufen.top/gtxqgvfnri.html

================================================================================
来源：http://hz.shzxlz.cn/gtioytlqpl.html

I. 正则表达式
来源：http://hz.sweek.top/gtdqzxpwxk.html

================================================================================
来源：http://hz.zhiwuduotai.top/gthzxfnjiy.html

[I01] 判断是否匹配
来源：http://hz.yanxiufei.cn/gtclmtcgyb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yuanzhike.top/gtzbsacokm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gtbqthobvp.html

JS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gthfpohqvk.html

TS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtrudusflf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dianchejie.cn/gtibyqutdz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhaomingkeji.xyz/gtaaiagzxz.html

Ruby: s.match?(/\d+/)
来源：http://hz.gogol.net.cn/gtbphwzmpj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pengpengdd.cyou/gtgwpoejmw.html

[I02] 提取所有匹配
来源：http://hz.sysykeji.top/gttrlyfzvm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.snrcjt.cn/gtpnhiikaw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gthgyptncb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jiagoushi.top/gtzsucwksu.html

TS:   s.match(/\d+/g)
来源：http://hz.yangfankeji.com/gtyypokfej.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangshuangyany.cn/gteuoxkujk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yangfankeji.com/gtszcrvssy.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxuanxn.top/gtbwrsgjlk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.c1oappe.top/gtghiwvhar.html

[I03] 提取捕获分组
来源：http://hz.shuidangran.top/gtyejrpdcm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yueranfly.top/gtnkavsqzw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guannengcc.top/gtptmypydg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.9152youxi.cn/gtgcduxaff.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.9152youxi.cn/gtaupxyewf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gtztoyoxhg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hongshengwenyu.top/gtyungqxvv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtxgvwrbyt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wangdashe.top/gtczptfpzf.html

[I04] 正则替换
来源：http://hz.ydjk.org.cn/gtqehawvvp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xuetiantiany.cn/gtrwylpivp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtwtyybfic.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuanzhike.top/gtzetjbxox.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gttxugytsg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pycfn.com/gtipzylbeq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hongshengwenyu.top/gtvpwntcwz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.316326.xyz/gtsydvgpoc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.redwolf501.top/gtoohehxst.html

[I05] 按正则拆分
来源：http://hz.pycfn.com/gtdhtzfuma.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tian-w.cn/gtfepkkckq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.birdmap.top/gtmlgptiwf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtjjcnxths.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtcqhyuprs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuetiantiany.cn/gtutcpeeld.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daria6918.cn/gtlovwkeog.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtwemksdpy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.0kj1m.cn/gtkuvoaybk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yanxiufei.cn/gtasxlfwmx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtfwbtxjdp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ywan-chungtsiang.top/gtuidombab.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtknssoeww.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtlptlzokc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.316326.xyz/gtrmkhstms.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shanyushiyangkeji.top/gtpgebwfde.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aibaodan.cn/gtyeamzwmf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gtjphamsfo.html

[I07] 忽略大小写与多行模式
来源：http://hz.dianchejie.cn/gtyjlhqguy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jiagoushi.top/gtcgudbcga.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenzaomai.com/gtrpbukwen.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nwbrower.top/gtfhiupctv.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gtukoakcll.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gtatrllmlx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hongshengwenyu.top/gtahfdghyh.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtdqzohyjt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtbnebtrfa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cqqwz.cn/gtxbpdazxa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.bjfxy.top/gtdxabvraa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.vqdsnc.cn/gtyjtgztbp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gthbdyfvwh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtevnrwjpv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aibaodan.cn/gtgmotaoiv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj202588.top/gtscsbbaqo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guannengcc.top/gtoryemboc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tanke756.top/gtembhasuk.html

================================================================================
来源：http://hz.meibo888.top/gtitxwzeax.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtoehsjqrw.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtwlmulmmp.html

[J01] 获取当前时间
来源：http://hz.cheryme.top/gtfzibwsfi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jianghu66.top/gtfpwabxpx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtfvtrelks.html

JS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtdslwwtjk.html

TS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gtaxuohrad.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fengsongda.top/gtepuuyqcw.html

Go:   time.Now()
来源：http://hz.zhijiandao.cn/gtbtwuranw.html

Ruby: Time.now
来源：http://hz.shanyushiyangkeji.top/gtwnzijuis.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhijiandao.cn/gtewbdvsjc.html

[J02] 格式化输出
来源：http://hz.guowangkeji.top/gtfuljdbmy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xingfuxueyuan.xyz/gtdwutftsd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtwhedhusc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hysaishi.cn/gtrabjshkq.html

TS:   d.toISOString()
来源：http://hz.hywenlv.cn/gtizzvelni.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sysykeji.top/gtmegitrmc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.aizwys.cn/gtzlikahtg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtfklgdecm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pengpengdd.cyou/gtynnkgcpi.html

[J03] 字符串解析为日期
来源：http://hz.cashguo.top/gtnrvygoyl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gttwkxmogo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinyuanbaomall.cn/gtdpmwwtbn.html

JS:   new Date("2024-01-02")
来源：http://hz.jqgufenzy.top/gtolewbmmd.html

TS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtsahxavhc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.redwolf501.top/gthgnvsawq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guowangkeji.top/gtmikiaiva.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtqcszbhox.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jyoumei.cn/gtroaxvwss.html

[J04] 时间戳与日期互转
来源：http://hz.cashguo.top/gtqfvsdlcz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtcivtlqaz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.havefunace.top/gtjayqbrdv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pycfn.com/gtsahacddj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sweek.top/gtvinxmzsx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigfzy.top/gtxfsomuyk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sxryk.cn/gtapecdfeb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jyoumei.cn/gtegibfnfc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jyoumei.cn/gttyoukerx.html

[J05] 时间加减（加 7 天）
来源：http://hz.shangyingyoupin.top/gtazoxqupt.html

Py:   now + timedelta(days=7)
来源：http://hz.c1oappe.top/gtqnwfgego.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yueranfly.top/gtxbhnzkba.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtflehciea.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtipkfczwj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yangfankeji.com/gtxptubjbj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydjk.org.cn/gtexvhppin.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daxiang520.top/gtlwwopdcf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jiagoushi.top/gteirpvwrm.html

[J06] 计算两时间之差
来源：http://hz.sweek.top/gtdpzdehsk.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangkeji.top/gtbdlgnnqu.html

PHP:  $end->diff($start)->days;
来源：http://hz.52xcode.cn/gtcsiadsof.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydzc1.top/gtcjyfejds.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jiagoushi.top/gtcvtlqerv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.redwolf501.top/gtxtkwrlbe.html

Go:   end.Sub(start).Hours()
来源：http://hz.zycfv.cn/gteizvqgis.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtvzydaimk.html

C#:   (end - start).TotalSeconds
来源：http://hz.mhx1999.top/gtxacskwde.html

[J07] 比较两个日期
来源：http://hz.cqqwz.cn/gtlsnxagdr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtzpqqohfb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangshuangyany.cn/gtwhbdqwga.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtpfpuoaey.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.smart0.xyz/gtohrdfqwq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhoulong.xyz/gtoyeneoqe.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.haohaochexian.top/gtxkyidplf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtpindiwkb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtltquhsky.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gtyrndrynn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jlsjyb.cn/gtildfhbrx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.9152youxi.cn/gtsgrpcvar.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guannengcc.top/gtxevhyaxf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tian-w.cn/gtcpjosdnp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yongpay.top/gtdeylazih.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.smart0.xyz/gtfbcoecto.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dashuyun.cn/gtjpjoffis.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cucudq.cn/gthltjdujq.html

[J09] 时区处理
来源：http://hz.chenzaomai.com/gtrzwwexuu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yongpay.top/gtfwjsaxdu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yanxiufei.cn/gtmaqnkdaa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtutvunufs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtsbrriakn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtecjnqegc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yuxming.cn/gtldiszfev.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shuidangran.top/gtpikzejxr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.vqdsnc.cn/gtzxxwnvfo.html

[J10] 取今天 / 本月第一天
来源：http://hz.316326.xyz/gtlkiknflm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gzhubu.top/gtnjkpuecm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.redwolf501.top/gtfzihocsg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnxiangtu.top/gtzrvefurt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xylfe.cn/gtgdncsnow.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.birdmap.top/gthwgqylia.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zdqjudy.top/gtpqrqgzww.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yangfankeji.com/gtgeeuhvtp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.snrcjt.cn/gtdqlpmetm.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtidbwbrqf.html

K. JSON 与序列化
来源：http://hz.ppjwa.cn/gtfsphtaif.html

================================================================================
来源：http://hz.vqdsnc.cn/gthqhcbqvl.html

[K01] 对象转 JSON 字符串
来源：http://hz.zdqjudy.top/gtyniryugn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gthnpofhbh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gttkbixjpz.html

JS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtyyslfaso.html

TS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtpsbeshaj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuetiantiany.cn/gtmdqzvseq.html

Go:   json.Marshal(obj)
来源：http://hz.sxryk.cn/gtanirbluk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yueranfly.top/gtlgdyvums.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hfpthk.cn/gtnvvryaox.html

[K02] JSON 字符串转对象
来源：http://hz.aizwys.cn/gtvdjpuwlw.html

Py:   json.loads(s)
来源：http://hz.ydzc1.top/gtftgmgxcc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.bjfxy.top/gtswxakrpp.html

JS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtwqipuius.html

TS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtympemhqp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhijiandao.cn/gtntsuhnfc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gthxxjfyyz.html

Ruby: JSON.parse(s)
来源：http://hz.andypj.xyz/gtplzwpskf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gtkotvosqz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhixingplan.top/gtjfmhxiib.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtbxdnjryl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gtevwgkmso.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtsagdtagu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtpkamirnl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258888.top/gtkhexkfon.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cqqwz.cn/gtbfaqwfnv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydjk.org.cn/gtseknjyki.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shangyingyoupin.top/gtadnkrhku.html

[K04] 读取 JSON 文件
来源：http://hz.yangfankeji.com/gtouapqnnl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sysykeji.top/gtmqwhcpgl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.pengpengdd.cyou/gtqrlvykuw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.birdmap.top/gtyyvdlzzf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtdzkkffsf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.haohaochexian.top/gtoyxuuogd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtiqzolrzm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hammf.cn/gtxkgptrjp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ybcxt.top/gtjneailhj.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtfjfsbkoe.html

Py:   copy.deepcopy(obj)
来源：http://hz.wangdashe.top/gtwrrdbgfy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xinyue.icu/gtpqafdtfs.html

JS:   structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtwhqkthas.html

TS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtekpwkjcj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.feifeiyinyue.top/gtizpnctlv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.havefunace.top/gtgsdrxkln.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.birdmap.top/gtlnqczuds.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhixingplan.top/gtvzifonzv.html

[K06] 解析 URL 查询串
来源：http://hz.feifeiyinyue.top/gtfrotlfor.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.c1oappe.top/gtervykwxo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnqzz.top/gtvflffrnz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtlcmhsgdh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtalvwyjvw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xylfe.cn/gtavrnzsry.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtbcfelrok.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yangfankeji.com/gtwazwijxw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258.top/gtviflqzok.html

[K07] 进制转换
来源：http://hz.redwolf501.top/gtwuriqrjh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.52xcode.cn/gteygkynsx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cashguo.top/gtcuiadecl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtnhhkhzxa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtsdnkyzgb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtprnnxsjk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.0kj1m.cn/gttgerffha.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.c1oappe.top/gtqnqxmurt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jlsjyb.cn/gtbxzwpjfx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhijiandao.cn/gtorkhzdfa.html

Py:   pickle.dumps(obj)
来源：http://hz.hammf.cn/gthokxqtce.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yangfankeji.com/gtbdjxccqu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gzhubu.top/gtbnfpatmy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtppmtdojb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.andypj.xyz/gtgiintfya.html

Go:   encoding/gob
来源：http://hz.yongpay.top/gtzptbvhce.html

Ruby: Marshal.dump(obj)
来源：http://hz.guowangkeji.top/gtaqmrlmov.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nwbrower.top/gtyjgfvvbq.html

================================================================================
来源：http://hz.cashguo.top/gtjmektxmm.html

L. 网络请求
来源：http://hz.nanxuanxn.top/gtzzputxne.html

================================================================================
来源：http://hz.yuanzhike.top/gtfnseqtlt.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangkeji.top/gtjplenczi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gaohongyu789.top/gtklrndabe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shuidangran.top/gtuqpvhwir.html

JS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtqozvrfhw.html

TS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtacfursmr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnxiangtu.top/gtilocqcbv.html

Go:   resp, err := http.Get(url)
来源：http://hz.svipenyu.cn/gtkzeplsfq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jyoumei.cn/gtpqjhamsh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.316326.xyz/gtauzvrnrr.html

[L02] 发送 POST JSON
来源：http://hz.hnxiangtu.top/gtpasvwldi.html


<!-- 参考信息 -->