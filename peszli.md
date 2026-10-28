代发 wailian999

[H07] 断言
来源：http://hz.fzhhl.top/gtuladremi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinghuilouyu.cn/gtvtjhxmju.html

PHP:  assert($x > 0);
来源：http://hz.wangshuangyany.cn/gtyryeyelb.html

JS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtxgytkvzh.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtsgyonxqu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cheryme.top/gtuvnmstkb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daria6918.cn/gthssvuuvk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gogol.net.cn/gttkxhvjvn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aibaodan.cn/gtzgcunagm.html

[H08] 获取错误信息与堆栈
来源：http://hz.52xcode.cn/gtxgyxcemm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gaohongyu789.top/gtszfzjcko.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtwmbhfxtt.html

JS:   e.message;  e.stack
来源：http://hz.yj20258.top/gtsfyhotcn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenlongwang.top/gtuoyfhybt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxuanxn.top/gtcziaefsn.html

Go:   err.Error()
来源：http://hz.havefunace.top/gtqktjrxgm.html

Ruby: e.message;  e.backtrace
来源：http://hz.guannengcc.top/gtlzzpnmwg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenjidiqi.icu/gtpvxzzild.html

[H09] 带错误码的异常
来源：http://hz.hnxiangtu.top/gtovjwtcxd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.0kj1m.cn/gtypcscoeh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.9152youxi.cn/gtaorarpnb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yueranfly.top/gtouzgrmyv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.feifeiyinyue.top/gtahtczhjc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.0kj1m.cn/gtlcxntvza.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dashuyun.cn/gtztupkqyh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgfzy.top/gtxmwpnoic.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gotoacloud.top/gtkqknsyum.html

[H10] 资源自动释放
来源：http://hz.haohaochexian.top/gtshbymqym.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangkeji.top/gtyrcexfzo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangdashe.top/gtkjhatpeh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhongyouzk.top/gtdeqmadwm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtjtvtwnal.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gzhubu.top/gtjsauozpl.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gttwvkwjwi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xingfuxueyuan.xyz/gtdoczqgue.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gotoacloud.top/gtyppjmcpt.html

================================================================================
来源：http://hz.hysaishi.cn/gtbrhycacr.html

I. 正则表达式
来源：http://hz.tanke756.top/gtcoxqqwaj.html

================================================================================
来源：http://hz.zhijiandao.cn/gtrywjdwbi.html

[I01] 判断是否匹配
来源：http://hz.hfpthk.cn/gtfqovpubn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtdvjxvzjy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtrogofxbe.html

JS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtjwziqllg.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gthccoysfn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.havefunace.top/gtcelhjvgg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nwbrower.top/gtcdmmkdkj.html

Ruby: s.match?(/\d+/)
来源：http://hz.sweek.top/gtizrloece.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sweek.top/gtvwklwjxd.html

[I02] 提取所有匹配
来源：http://hz.jinyuanbaomall.cn/gtrfhaboyz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.c1oappe.top/gtiqbqxqll.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sysykeji.top/gtzuhfwumd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenlongwang.top/gtlkuvxszv.html

TS:   s.match(/\d+/g)
来源：http://hz.iojbl.cn/gtejpzrtky.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pengpengdd.cyou/gtresqtncj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgfzy.top/gtxjiklaal.html

Ruby: s.scan(/\d+/)
来源：http://hz.cqqwz.cn/gtkkzwainl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xziqi.cn/gtvukzaosx.html

[I03] 提取捕获分组
来源：http://hz.shuidangran.top/gtkdmvcinv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.316326.xyz/gtuyifgdsh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ywan-chungtsiang.top/gtnikzyhao.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinghuilouyu.cn/gtxyjhgvtm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yuxming.cn/gtsqwqqwip.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sweek.top/gtfbvrjtrr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cqqwz.cn/gtlomzmtfh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtgatqttgu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.pengpengdd.cyou/gtdskchobh.html

[I04] 正则替换
来源：http://hz.jinyuanbaomall.cn/gtsidftrwx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daria6918.cn/gthvnhbrep.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ivvv.top/gtjwwshzwt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtoffddhbd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtjbcbilgf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.haohaochexian.top/gtsvsdqlqz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinqigfzy.top/gtlogxnynq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fengsongda.top/gtejkesgkp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hnqzz.top/gtenmqgzbu.html

[I05] 按正则拆分
来源：http://hz.shzxlz.cn/gtvywcnrvn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gzhubu.top/gtdzohjrui.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhoulong.xyz/gtxlcbushr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtvfpzcguh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtabcyqplk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cheryme.top/gtkcsviihp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgufenzy.top/gthazocslm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtekmtfepj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gtojlfgvyn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hammf.cn/gtbpupvuvs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sufxvd.cn/gtybequizn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cucudq.cn/gtzqbuhzjq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtqsqwwhuz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtozvyeypz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cheryme.top/gtiwnkmppu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenzaomai.com/gtjgyvbosw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cucudq.cn/gtfwurcnrp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtxtaieiox.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtbrtfgsjf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gtbrgwelia.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuanzx.com/gtdgjybgkw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.kuanghao11.cn/gtiklkdvld.html

TS:   /error/gim
来源：http://hz.xuetiantiany.cn/gtbznozopv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.smart0.xyz/gtelzorblk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yanxiufei.cn/gtfdptewbd.html

Ruby: s.scan(/error/i)
来源：http://hz.birdmap.top/gthzyfiuun.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuanzhike.top/gtcezboowj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sysykeji.top/gtacxzewxf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fzhhl.top/gtxyerskxx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zdqjudy.top/gtdswpkoec.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtibwkfkmb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj202588.top/gtzowoeogo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtssmzbltf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.havefunace.top/gtzlxpxpxi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxuanxn.top/gtzqeuniyf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtamayfjiw.html

================================================================================
来源：http://hz.xziqi.cn/gtnbklcxoj.html

J. 日期与时间
来源：http://hz.shangyingyoupin.top/gtgzyphllj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtxrwmxydw.html

[J01] 获取当前时间
来源：http://hz.ydzc1.top/gtzmifbwpn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jqgufenzy.top/gtabfigajl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gthcygvffk.html

JS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gtiwxvjqqr.html

TS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtbuzhuzia.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hammf.cn/gtmqpewjac.html

Go:   time.Now()
来源：http://hz.hammf.cn/gtnhpgxdos.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtydoqiuzn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yvedp.cn/gtlpkrhccf.html

[J02] 格式化输出
来源：http://hz.yangfankeji.com/gtpiuoqdws.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtforqdsxv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gtrrwekfbr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zycfv.cn/gtsvuxnxjh.html

TS:   d.toISOString()
来源：http://hz.zhoulong.xyz/gtghnntgzx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zdqjudy.top/gtstfollaa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xingfuxueyuan.xyz/gtdqshtsga.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtlgemfrzu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daria6918.cn/gtpxqhgwxr.html

[J03] 字符串解析为日期
来源：http://hz.gaohongyu789.top/gtvdtpyvfl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ppjwa.cn/gthbeesuhm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.haohaochexian.top/gtdbdcsglc.html

JS:   new Date("2024-01-02")
来源：http://hz.tian-w.cn/gtxiwddhmx.html

TS:   new Date("2024-01-02")
来源：http://hz.zhongyouzk.top/gtwosrpigh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtfgltsdqa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj202588.top/gthofxhmzg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tian-w.cn/gtvgwjmepb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgfzy.top/gtvyklbwmx.html

[J04] 时间戳与日期互转
来源：http://hz.zhiwuduotai.top/gttazkvrho.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.bjfxy.top/gtqfypewyp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yongpay.top/gtplknapxf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ybcxt.top/gtfflhevkh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gtkoqsbhxd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtkltwuqtg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fengsongda.top/gtkyynteay.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydzc1.top/gtbqatrjnf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.316326.xyz/gtecieydel.html

[J05] 时间加减（加 7 天）
来源：http://hz.yongpay.top/gtsaejlwdp.html

Py:   now + timedelta(days=7)
来源：http://hz.guannengcc.top/gtavvhhwik.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj20258888.top/gtqfvdhtan.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtqywvblyu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtnjrkgxqc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dashuyun.cn/gtzdbweocw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangshuangyany.cn/gtjqjdktsx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhaomingkeji.xyz/gtnhxhnfvy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtnipjfrdc.html

[J06] 计算两时间之差
来源：http://hz.zhixingplan.top/gtqznvsjyx.html

Py:   (end - start).total_seconds()
来源：http://hz.yongpay.top/gtrhwqaqdi.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinyuanbaomall.cn/gtfwvovwhk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cucudq.cn/gtfsvgybcc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xuetiantiany.cn/gtxoqdpdjo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.havefunace.top/gtajpfufzh.html

Go:   end.Sub(start).Hours()
来源：http://hz.birdmap.top/gtxroqbupb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guannengcc.top/gtranktvef.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gthyfmvjfs.html

[J07] 比较两个日期
来源：http://hz.guannengcc.top/gtsabdbotf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtpcelhspk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxinkj.top/gtpijwihfi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtptebrjqq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtuyxwzref.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xinyue.icu/gtmotizmde.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtbxlwzgkd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtttctqrtw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gthoaeivda.html

[J08] 提取年月日与星期
来源：http://hz.hongshengwenyu.top/gtncvxqvze.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.52xcode.cn/gtkjdbhccp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tanke756.top/gtknerezzi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gtmudlydaz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.svipenyu.cn/gtqhyezjbh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhengqikj.top/gtanhbnlsj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zycfv.cn/gtqfyigrjq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tian-w.cn/gtrgmwgtgb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangkeji.top/gtceolhzhw.html

[J09] 时区处理
来源：http://hz.havefunace.top/gtdvbyucgd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ehwqpu.com/gtnkgbdhno.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258.top/gtmscdqtrp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtepnmsedu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtaxknizji.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.vqdsnc.cn/gtspuucbut.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gzhubu.top/gtvyozlrja.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj202588.top/gtnhhnyjhl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuanzx.com/gtpfiwkkgf.html

[J10] 取今天 / 本月第一天
来源：http://hz.sysykeji.top/gtorucsrwr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cashguo.top/gtzvhcymot.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aibaodan.cn/gtjcsttxdh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xziqi.cn/gtyfgdmlyi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ybcxt.top/gtbivnpbjg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ehwqpu.com/gtcpqcyxmq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gzhubu.top/gtqbibgisb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xingfuxueyuan.xyz/gthwysixhz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ppjwa.cn/gtmecmexxs.html

================================================================================
来源：http://hz.daxiang520.top/gtetjkboyv.html

K. JSON 与序列化
来源：http://hz.xingfuxueyuan.xyz/gttivuaksv.html

================================================================================
来源：http://hz.gotoacloud.top/gtexrnpodb.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnxiangtu.top/gtwmhhtaoo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gttaqaysek.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gtyjyogoto.html

JS:   JSON.stringify(obj)
来源：http://hz.sufxvd.cn/gtnpqpkhrs.html

TS:   JSON.stringify(obj)
来源：http://hz.zdqjudy.top/gtomvjapib.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhengqikj.top/gtbbpgghlb.html

Go:   json.Marshal(obj)
来源：http://hz.sweek.top/gtjfghkizb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.snrcjt.cn/gtlxydmong.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenlongwang.top/gtxdzyrmvp.html

[K02] JSON 字符串转对象
来源：http://hz.hnqzz.top/gtfzonwftl.html

Py:   json.loads(s)
来源：http://hz.c1oappe.top/gtendvnfnc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dianchejie.cn/gtjdkygkbd.html

JS:   JSON.parse(s)
来源：http://hz.hammf.cn/gtsabynnvh.html

TS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtwlrskjkm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jqgfzy.top/gtafhqjncz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtnwehswdj.html

Ruby: JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtwxozinlx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yueranfly.top/gtfnhqjlji.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenzaomai.com/gtqkwnrzef.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtutyyzqic.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtlfazovty.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtsdbtrkwq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtboxzmvdx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dianchejie.cn/gtdpwsxhkv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenzaomai.com/gtkhbtqayw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenzaomai.com/gtdxeyptsl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.316326.xyz/gtsxiypkez.html

[K04] 读取 JSON 文件
来源：http://hz.snrcjt.cn/gtfzusfjpd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hfpthk.cn/gtxmovvrxu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhengqikj.top/gtqtjnqqaq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtzifzeygt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daxiang520.top/gtobeiepke.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aibaodan.cn/gtcsstbyzl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.wangdashe.top/gtghmrbsgk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zycfv.cn/gterykrlyt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.vqdsnc.cn/gtvnzmzvkg.html

[K05] 深拷贝对象
来源：http://hz.nanxinkj.top/gtfgsdfwxb.html

Py:   copy.deepcopy(obj)
来源：http://hz.daria6918.cn/gtmoxqhvno.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnxiangtu.top/gtadvegciv.html

JS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gthobyhsdm.html

TS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtozsblzcr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yongpay.top/gtbhansshl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.smart0.xyz/gtflwsayik.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cashguo.top/gtxyxxogaf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xziqi.cn/gtkgpcsbyk.html

[K06] 解析 URL 查询串
来源：http://hz.andypj.xyz/gtprdxpdum.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jiagoushi.top/gtxrbvjyjg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhiwuduotai.top/gttpublnrt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtxsxelrnh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.quarkkingdee.top/gtqmrhwbuf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ehwqpu.com/gtmbdlaiqn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnqzz.top/gtytjxbqqo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gteiozjndh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hysaishi.cn/gtmmkgujms.html

[K07] 进制转换
来源：http://hz.hfpthk.cn/gtuytavctw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258.top/gtlcdywjtm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangkeji.top/gtrecbpdkm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtcbtzepcp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtngpuskub.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtqdozgisz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuetiantiany.cn/gtxdnhuunx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cqqwz.cn/gtpvantjhi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.kuanghao11.cn/gtqlgbvbzf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhijiandao.cn/gtunrwpqyi.html

Py:   pickle.dumps(obj)
来源：http://hz.yongpay.top/gtqtmhrftk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtpcgryetj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gthrrnkzsn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.vqdsnc.cn/gtibyntmeq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hongshengwenyu.top/gtnlqhouho.html

Go:   encoding/gob
来源：http://hz.zhiwuduotai.top/gtclpbenzb.html

Ruby: Marshal.dump(obj)
来源：http://hz.yanxiufei.cn/gtaqxuoysm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.snrcjt.cn/gtwgalvajw.html

================================================================================
来源：http://hz.sweek.top/gtgluqhpwh.html

L. 网络请求
来源：http://hz.smart0.xyz/gtpvkfrqtb.html

================================================================================
来源：http://hz.nanxuanxn.top/gtjxrllhep.html

[L01] 发送 GET 请求
来源：http://hz.cheryme.top/gtjovbmnuw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gotoacloud.top/gtwdupefyk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.svipenyu.cn/gtxykavgmi.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtitpimreu.html

TS:   await fetch(url)
来源：http://hz.jqgfzy.top/gttoexukzp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtylolmwbn.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtogihmdng.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.vqdsnc.cn/gtytxhcwsa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.meibo888.top/gtwcacjrvv.html

[L02] 发送 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtxyducqjo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cucudq.cn/gtncpkbtzl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ivvv.top/gtmkzihhpw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtfwruncsf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gttmvjibav.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xziqi.cn/gtmoiikrxh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xylfe.cn/gtznzupnty.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.quarkkingdee.top/gtvwgbshkn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yangfankeji.com/gtpajiaekc.html


<!-- 参考信息 -->