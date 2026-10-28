代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtrvweepkd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tianlin.xyz/gtfecmwstu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ybcxt.top/gtocaiskfs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gthjynqzzx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gotoacloud.top/gtbfkhwrub.html

[H08] 获取错误信息与堆栈
来源：http://hz.hfpthk.cn/gtggwjjley.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xinyue.icu/gtchylerka.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtkinjmhmk.html

JS:   e.message;  e.stack
来源：http://hz.ydjk.org.cn/gtuavaakss.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.daria6918.cn/gtkrcpolbk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xuetiantiany.cn/gttxtsvozl.html

Go:   err.Error()
来源：http://hz.yuanzhike.top/gtwumdneyn.html

Ruby: e.message;  e.backtrace
来源：http://hz.sufxvd.cn/gtldwjqotg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.bjfxy.top/gtkvefozvh.html

[H09] 带错误码的异常
来源：http://hz.svipenyu.cn/gtmgutospn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.guowangkeji.top/gtxnabnfyq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xuanzx.com/gtamhlrzxo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxuanxn.top/gtdxjbqkob.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yonumen.top/gthohavnhh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.pengpengdd.cyou/gtfkszmddv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj202588.top/gtdgdxcuek.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydjk.org.cn/gtobmxcaxs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shangyingyoupin.top/gtfmfdxbij.html

[H10] 资源自动释放
来源：http://hz.nwbrower.top/gterlzwplz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.fengsongda.top/gtmmkjqqkr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.kuanghao11.cn/gtbkmpqzhc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtvgadiemg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.quarkkingdee.top/gtckhfdyax.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tanke756.top/gtyvwvyvst.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gtbxiznnwz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgfzy.top/gtuxjpricr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydjk.org.cn/gtyupaewxc.html

================================================================================
来源：http://hz.ppjwa.cn/gtznipdqto.html

I. 正则表达式
来源：http://hz.jlsjyb.cn/gtsnbwmxbr.html

================================================================================
来源：http://hz.yj20258.top/gtlfqblejj.html

[I01] 判断是否匹配
来源：http://hz.tianlin.xyz/gtfvpyoxbq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.iojbl.cn/gtdpbgjomw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtvpyanoeh.html

JS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtomiuuwpr.html

TS:   /\d+/.test(s)
来源：http://hz.316326.xyz/gtrjaqiavz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gaohongyu789.top/gtfswemfur.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinyuanbaomall.cn/gtzzhktqwu.html

Ruby: s.match?(/\d+/)
来源：http://hz.hysaishi.cn/gtmvykdeba.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ppjwa.cn/gtowvjbyls.html

[I02] 提取所有匹配
来源：http://hz.yongpay.top/gteaqoemxp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.havefunace.top/gtpxprvftt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.haohaochexian.top/gtlyobqnjy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sweek.top/gtkiphvwui.html

TS:   s.match(/\d+/g)
来源：http://hz.hysaishi.cn/gtsefgrsuj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.quarkkingdee.top/gtnxhgotyo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nwbrower.top/gtluqttwnm.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuetiantiany.cn/gtmwdtaxrz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenlongwang.top/gtgruwaple.html

[I03] 提取捕获分组
来源：http://hz.chenjidiqi.icu/gtiwttjjwn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guannengcc.top/gthudrzsbb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dashuyun.cn/gtzjjxouij.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hysaishi.cn/gtpbogbrxe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gotoacloud.top/gtongkqcii.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gogol.net.cn/gttqnjpoau.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shuidangran.top/gthgatmmvt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.quarkkingdee.top/gtmkjuaqww.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydjk.org.cn/gtjlsebwmn.html

[I04] 正则替换
来源：http://hz.shanyushiyangtech.top/gtfkgdwryh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hfpthk.cn/gtjvgkdjfv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shzxlz.cn/gtlnkajvov.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuxming.cn/gtqjsubgjw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtjcqxqrdt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aibaodan.cn/gtczdvazot.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gtpryidinc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dianchejie.cn/gtlrbyaqqa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxuanxn.top/gtndhfrehe.html

[I05] 按正则拆分
来源：http://hz.shangyingyoupin.top/gtwzytwgcr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xinyue.icu/gtphmqhthz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yonumen.top/gtimtnsmau.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtgtjlbagh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtmktjhmyd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guowangkeji.top/gthsjmnrdy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenzaomai.com/gtbunjoovr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtfozkaxfk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.birdmap.top/gttsfyqldn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sweek.top/gtphtuncgr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.fengsongda.top/gtfeyddwsz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ybcxt.top/gtniefscpz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.meibo888.top/gtwxpzzckn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtvcoyrqbw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xuetiantiany.cn/gtvyhwxxzm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ywan-chungtsiang.top/gthcehbuno.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.svipenyu.cn/gtqwdjxvdq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtklundshv.html

[I07] 忽略大小写与多行模式
来源：http://hz.shzxlz.cn/gtjxbnvgmk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yonumen.top/gtjpigjdhh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sxryk.cn/gtwvmckgkw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yvedp.cn/gtkbocljiv.html

TS:   /error/gim
来源：http://hz.xinyue.icu/gtwfpqltul.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guannengcc.top/gtcdaestes.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tian-w.cn/gtrhnhktmn.html

Ruby: s.scan(/error/i)
来源：http://hz.havefunace.top/gtnlqwvfkv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydjk.org.cn/gtgsrjyhre.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gtevyswrcf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.andypj.xyz/gtygixgfll.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.9152youxi.cn/gtsygbafao.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtopidxonn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtkzdnvmhe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtaxozlyng.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xinyue.icu/gtvcpcxtma.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sxryk.cn/gtqwrvvvuz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ybcxt.top/gtpfclohvv.html

================================================================================
来源：http://hz.jqgfzy.top/gtyumfzbta.html

J. 日期与时间
来源：http://hz.ydzc1.top/gtnigqarae.html

================================================================================
来源：http://hz.hnqzz.top/gtngsxsmif.html

[J01] 获取当前时间
来源：http://hz.aibaodan.cn/gtwzhauuqu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pengpengdd.cyou/gtkjceilcw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtjqxuvmfe.html

JS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gttweszhsn.html

TS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gtlazkjwfl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cdnleiting.top/gtkgskpejv.html

Go:   time.Now()
来源：http://hz.guowangkeji.top/gtrceqeern.html

Ruby: Time.now
来源：http://hz.pengpengdd.cyou/gtkohxjbvv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tianlin.xyz/gtiefuasaq.html

[J02] 格式化输出
来源：http://hz.meibo888.top/gttisrqjdw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtqgsyyzxx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtbqkcnmhd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gzhubu.top/gteasmyfmf.html

TS:   d.toISOString()
来源：http://hz.ydzc1.top/gtptnnlthk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xylfe.cn/gtikmqauld.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangshuangyany.cn/gtfyfqbiny.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtpnxvyzjn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daria6918.cn/gtakwrosvt.html

[J03] 字符串解析为日期
来源：http://hz.fzhhl.top/gtjfgdybhp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shuidangran.top/gtfshnfvna.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.birdmap.top/gthxeokxln.html

JS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtkogluhqm.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtpcrojzom.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtozxgnrnb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.dashuyun.cn/gthbmjerjn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gtjipqijud.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258888.top/gtnqtlvsde.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gtpkpzuswf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gtadjihkpi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.andypj.xyz/gtpbhrohka.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gzhubu.top/gtbfrguhof.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hysaishi.cn/gtcxkjygnn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenjidiqi.icu/gtiqmntziy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.9152youxi.cn/gtjkawymad.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shangyingyoupin.top/gtysyurolf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.9152youxi.cn/gthplivluj.html

[J05] 时间加减（加 7 天）
来源：http://hz.ehwqpu.com/gtvunebbqf.html

Py:   now + timedelta(days=7)
来源：http://hz.yonumen.top/gtckadjdey.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gtqiouuqbq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtsquxvltg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gttypweynd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gteuswxcij.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hammf.cn/gtumkvwawe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.iojbl.cn/gtcjcxlyoi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fengsongda.top/gtnqonymvd.html

[J06] 计算两时间之差
来源：http://hz.tian-w.cn/gtchgbqeqd.html

Py:   (end - start).total_seconds()
来源：http://hz.haohaochexian.top/gtcsoknpwb.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj202588.top/gtqppshutx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gtevbzdpic.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gtucksbsup.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.0kj1m.cn/gtuxizvxfe.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgufenzy.top/gtwibhfncz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gtikycgqic.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtkkjuodmz.html

[J07] 比较两个日期
来源：http://hz.daxiang520.top/gtuvsvwyhv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gthawmetew.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tian-w.cn/gtewcjxxua.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtcjwaspuk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.redwolf501.top/gtxhcwzrpa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gtppxegxno.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zycfv.cn/gtsrvqurlp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtgthmxirc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtznnyxjcn.html

[J08] 提取年月日与星期
来源：http://hz.yangfankeji.com/gtqdqwnyix.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zycfv.cn/gtwvevfrdo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ppjwa.cn/gtepqvdkxt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj202588.top/gtvsdgjenq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hongshengwenyu.top/gtzelvwxpy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gthphsqoiv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.svipenyu.cn/gtigxfyrcl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtxhwfnwvc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ppjwa.cn/gtetrxpqph.html

[J09] 时区处理
来源：http://hz.zhiwuduotai.top/gtjenqmtpa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zdqjudy.top/gtbgtuqnsf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgufenzy.top/gtizavcbcz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtypodxbie.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtocbzsqly.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gthtsgohxe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigufen.top/gthvyglitu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinghuilouyu.cn/gtftowtwnr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cqqwz.cn/gtcifutaee.html

[J10] 取今天 / 本月第一天
来源：http://hz.yvedp.cn/gthluurmsg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gaohongyu789.top/gtmloyzafj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.daria6918.cn/gtaonerrwj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tian-w.cn/gtbvsldlki.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tanke756.top/gttajdbpah.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ivvv.top/gtlanmavua.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydjk.org.cn/gtwuawniwu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tanke756.top/gtadyxvmas.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yongpay.top/gtpsojwhvf.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvibzziix.html

K. JSON 与序列化
来源：http://hz.pengpengdd.cyou/gtwtetelsl.html

================================================================================
来源：http://hz.cashguo.top/gtqmfeeufc.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtlbfngexl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtkytfsfll.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtapqfkeoo.html

JS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtipgjxkri.html

TS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gtkqordwop.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuanzhike.top/gtzejrxkja.html

Go:   json.Marshal(obj)
来源：http://hz.cheryme.top/gtcvvirfor.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxinkj.top/gtrrsvsjno.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aizwys.cn/gtsmwcwfbf.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigfzy.top/gtleyavtlk.html

Py:   json.loads(s)
来源：http://hz.birdmap.top/gthtqgsupa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtvyxprqpo.html

JS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtwipgralq.html

TS:   JSON.parse(s)
来源：http://hz.ivvv.top/gtvexptugk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pycfn.com/gtephjkfkc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtdkzkmdfu.html

Ruby: JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtbbwavrbr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gtryezrajp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhijiandao.cn/gtwtxquxsj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.316326.xyz/gtxqbfjyor.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtfgaabuwa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gtzetnyhqv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtufkdisjc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.redwolf501.top/gtzmfaxeaj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gtefbkogas.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhijiandao.cn/gtxysiaqdy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.smart0.xyz/gtnjtbarjs.html

[K04] 读取 JSON 文件
来源：http://hz.tianlin.xyz/gtudbxrcpt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daria6918.cn/gtgfenlzsq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hnqzz.top/gtcshoycnm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtzljanhvl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtpytjcvoq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxuanxn.top/gtgstxbpag.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtfarzcxgg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.redwolf501.top/gtbidifppr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hammf.cn/gthmsqdcvx.html

[K05] 深拷贝对象
来源：http://hz.yonumen.top/gtxhcesgtt.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydzc1.top/gtsptdsomz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.kuanghao11.cn/gtjopzvimd.html

JS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtuwnwnimb.html

TS:   structuredClone(obj)
来源：http://hz.cashguo.top/gttamsadlf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.9152youxi.cn/gtwncbfqob.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.meibo888.top/gtlulybtgm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gthneoyrwa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtponhkylj.html

[K06] 解析 URL 查询串
来源：http://hz.gaohongyu789.top/gtglqbxfpz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtkngmxznv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fengsongda.top/gtirjgrhjz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtohwfigux.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtijiugfuq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aizwys.cn/gtofmvjynh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtdesdhldh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtiprztqhw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gotoacloud.top/gtkcfybxdw.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtuossrkeo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtcsuitwlq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zycfv.cn/gtnvdcxttj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtiychjyfd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtyoqtzmmt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtlutnmfkm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgfzy.top/gtfnpkqzyk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtjwyuksyn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jianghu66.top/gtfxiacbit.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xingfuxueyuan.xyz/gthxyqeisf.html

Py:   pickle.dumps(obj)
来源：http://hz.gotoacloud.top/gtvnmfxthe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xylfe.cn/gtkkloudxn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtdvrjthbu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuanzx.com/gtxtiqpshq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gzhubu.top/gtwptrirzi.html

Go:   encoding/gob
来源：http://hz.fengsongda.top/gturtvkkal.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtsrfikazk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gotoacloud.top/gtjwhmvhgr.html

================================================================================
来源：http://hz.yvedp.cn/gtstgpnlif.html

L. 网络请求
来源：http://hz.chenlongwang.top/gtjcqhumdr.html

================================================================================
来源：http://hz.shuidangran.top/gtqzaaxtou.html

[L01] 发送 GET 请求
来源：http://hz.316326.xyz/gtwjfasnwl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenzaomai.com/gtqnprvtmu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yuxming.cn/gttsywidxc.html

JS:   await fetch(url)
来源：http://hz.shuidangran.top/gtayemfiop.html

TS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gtchmrlwid.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigfzy.top/gtjecjifjw.html

Go:   resp, err := http.Get(url)
来源：http://hz.andypj.xyz/gtmeskbyln.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fzhhl.top/gtwtjezfyi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenlongwang.top/gtmkmwnzqk.html

[L02] 发送 POST JSON
来源：http://hz.aizwys.cn/gtzfkuylas.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.havefunace.top/gtgrdjvndr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj202588.top/gtafqolnzl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtegipnuar.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtrfzqdyyx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenlongwang.top/gtvjrhyrxv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.meibo888.top/gtsbhuvwfu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cheryme.top/gtkqtokprn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guannengcc.top/gtcezuqdla.html

[L03] 设置自定义请求头
来源：http://hz.dashuyun.cn/gtdxctgdsp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gtxnwvirtw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cashguo.top/gtrtsguite.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtojdejzol.html


<!-- 参考信息 -->