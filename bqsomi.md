代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tianlin.xyz/gthzrptmeg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtbwnthazt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gaohongyu789.top/gtbivuetca.html

C#:   obj?.A?.B ?? default
来源：http://hz.andypj.xyz/gtzdxtzvnh.html

[H07] 断言
来源：http://hz.9152youxi.cn/gtktzruajn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guannengcc.top/gtxoegyjpz.html

PHP:  assert($x > 0);
来源：http://hz.meibo888.top/gttefvtszj.html

JS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtlwuxattc.html

TS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtjqwhgynl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nanxuanxn.top/gtgzyweoey.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxinkj.top/gtxbpuzcsk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hongshengwenyu.top/gttttgyabr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gtfmrodgsz.html

[H08] 获取错误信息与堆栈
来源：http://hz.tian-w.cn/gtxjszcusm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.vqdsnc.cn/gtsgwgckyg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtmzrkhans.html

JS:   e.message;  e.stack
来源：http://hz.hnqzz.top/gtxfhrwywb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cheryme.top/gtcmkxylrz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.haohaochexian.top/gtyygektzz.html

Go:   err.Error()
来源：http://hz.jinyuanbaomall.cn/gtbaeornsz.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxuanxn.top/gtplmlosun.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtngghtyed.html

[H09] 带错误码的异常
来源：http://hz.sufxvd.cn/gtblwyhspl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fengsongda.top/gttjbogxep.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.iojbl.cn/gtvucszoah.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtidyzqman.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yonumen.top/gthiagqsid.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnxiangtu.top/gtprgnkgkt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gogol.net.cn/gtkuctoded.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tianlin.xyz/gtmngyskba.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhiwuduotai.top/gttfnkvghr.html

[H10] 资源自动释放
来源：http://hz.jinqigfzy.top/gtaiejkpoz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnqzz.top/gthykukade.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258888.top/gtljapopth.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtrshhmwwe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtutuwztcc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.fzhhl.top/gtquhkjhaf.html

Go:   defer f.Close()
来源：http://hz.cqqwz.cn/gtlcrrorno.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cucudq.cn/gtykeurchn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ybcxt.top/gtqgaqcyiy.html

================================================================================
来源：http://hz.shuidangran.top/gthdbbuhqx.html

I. 正则表达式
来源：http://hz.chenzaomai.com/gtxshyqhds.html

================================================================================
来源：http://hz.dianchejie.cn/gtqmfamrsr.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gtlgauttnn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ehwqpu.com/gtwtsrwzyg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fengsongda.top/gtzvhqxlqc.html

JS:   /\d+/.test(s)
来源：http://hz.kuanghao11.cn/gtzwkrgvgh.html

TS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gthaycclxm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dianchejie.cn/gtzivcgmsh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fzhhl.top/gtoflkeoxo.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhoulong.xyz/gtkvzymywf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.9152youxi.cn/gtegmwldqh.html

[I02] 提取所有匹配
来源：http://hz.yj202588.top/gtmbvsmqgc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jiagoushi.top/gtawypqrul.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sweek.top/gtkfegoumg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtfzhrkkte.html

TS:   s.match(/\d+/g)
来源：http://hz.yvedp.cn/gtjhvqillc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guannengcc.top/gtaqdyynrh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daria6918.cn/gtsorburio.html

Ruby: s.scan(/\d+/)
来源：http://hz.yonumen.top/gtpuynghib.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cheryme.top/gtfjzjfwyq.html

[I03] 提取捕获分组
来源：http://hz.haohaochexian.top/gtlnpdjhcf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yueranfly.top/gttakpwxkd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sysykeji.top/gtcekajupc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jlsjyb.cn/gteoetrwgz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gtzikomhvd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aibaodan.cn/gtorsjmnry.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gaohongyu789.top/gtoamekdnf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.svipenyu.cn/gtkuqewfcc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuetiantiany.cn/gtlybigzhn.html

[I04] 正则替换
来源：http://hz.pycfn.com/gthahmdtjy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hnqzz.top/gtskjncdhf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtzisxzigs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtxxnwyyvj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtyzxvkeyp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cashguo.top/gtzyulstpx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yonumen.top/gtjkzelgbs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtskplvxij.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtrabbpopb.html

[I05] 按正则拆分
来源：http://hz.zhiwuduotai.top/gtsfdyafqo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.52xcode.cn/gtvwjmeama.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinghuilouyu.cn/gthmejkvwk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtpxznanup.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtztckewpo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgfzy.top/gtmyrkdyjj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hongshengwenyu.top/gtsbxwmhqz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtbxbxpmpy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shzxlz.cn/gtakyjcluy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ybcxt.top/gtucwwdxbr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtbadvsaem.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xylfe.cn/gthldwvwyh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jyoumei.cn/gtuyffdqgr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtapuuhttc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shzxlz.cn/gtpdnamfzx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxinkj.top/gtpekepxel.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hywenlv.cn/gtmazvfkgz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtjjuivqnt.html

[I07] 忽略大小写与多行模式
来源：http://hz.pycfn.com/gtelfckgin.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yonumen.top/gtyloyyjyp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.52xcode.cn/gtatjbtayt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aizwys.cn/gtcisbdcyr.html

TS:   /error/gim
来源：http://hz.cheryme.top/gtqxorcbmo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxuanxn.top/gtwksfuxzc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gttcjtviel.html

Ruby: s.scan(/error/i)
来源：http://hz.havefunace.top/gtbnmezzog.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hfpthk.cn/gtusberrqb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gotoacloud.top/gtkrubdewf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.dianchejie.cn/gtfcbebftl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtzfsrrhmz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gtmqzarcdc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtkfiuowgu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.haohaochexian.top/gthbyhwvce.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sweek.top/gtrjrqhakk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangkeji.top/gtsnbdxzkj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gttxgwgftt.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgoewfyhf.html

J. 日期与时间
来源：http://hz.jyoumei.cn/gtdwfqtpyh.html

================================================================================
来源：http://hz.yongpay.top/gtdkoilubu.html

[J01] 获取当前时间
来源：http://hz.redwolf501.top/gtrziaxhkq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.52xcode.cn/gtfsswzdxf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtiixxrfxy.html

JS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtyqjgdbhd.html

TS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtwxitmqcx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pycfn.com/gtxplwpzrd.html

Go:   time.Now()
来源：http://hz.chenzaomai.com/gtpakcfcmq.html

Ruby: Time.now
来源：http://hz.cucudq.cn/gtgwkxkrxc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtgrdrzivk.html

[J02] 格式化输出
来源：http://hz.fengsongda.top/gtjtskftap.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtwcsfjwjm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtiwhgfbsm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangkeji.top/gttwraisxa.html

TS:   d.toISOString()
来源：http://hz.yangfankeji.com/gtwutqfodn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ydjk.org.cn/gtgeuflhyo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jlsjyb.cn/gtojadcmly.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtrfgvuwas.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.svipenyu.cn/gtfehiyvov.html

[J03] 字符串解析为日期
来源：http://hz.xuanzx.com/gtygogcdzx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhongyouzk.top/gtkkcqmejr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fengsongda.top/gtfakuqbqu.html

JS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtqgmtfqen.html

TS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtvjjmgfqp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yanxiufei.cn/gttssdnafx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yueranfly.top/gtvphnmdgb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtfnoqztpl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ppjwa.cn/gtzbvuyvjj.html

[J04] 时间戳与日期互转
来源：http://hz.guowangkeji.top/gtopzsuyhg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258.top/gteeknysgu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.birdmap.top/gtyuxgxqbs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.wangdashe.top/gtbiqghcqx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hammf.cn/gtmtzsxuwi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxuanxn.top/gtafgzawdc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gtxtczfygk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigufen.top/gtypjrgkxw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yueranfly.top/gtjznvplpy.html

[J05] 时间加减（加 7 天）
来源：http://hz.sxryk.cn/gtfizuwncv.html

Py:   now + timedelta(days=7)
来源：http://hz.ehwqpu.com/gtwmjqopcj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gogol.net.cn/gtamuxxqac.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jianghu66.top/gtjmnlfflh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtopormaki.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hfpthk.cn/gtsidryslh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.andypj.xyz/gtxksbgxhd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cdnleiting.top/gthrgeyerx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.andypj.xyz/gttqjvgdcp.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtekrdvrix.html

Py:   (end - start).total_seconds()
来源：http://hz.ppjwa.cn/gtlbvqkggx.html

PHP:  $end->diff($start)->days;
来源：http://hz.ppjwa.cn/gtqgaoqrgs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gtmognsfiv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gtwcabhctc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gtplsdgjrs.html

Go:   end.Sub(start).Hours()
来源：http://hz.ywan-chungtsiang.top/gtgnvemrka.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydzc1.top/gtyskfrnrn.html

C#:   (end - start).TotalSeconds
来源：http://hz.iojbl.cn/gthqvabwqh.html

[J07] 比较两个日期
来源：http://hz.yanxiufei.cn/gtlpbiwryg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtrseyziee.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xziqi.cn/gtbmhmmzjr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gtavlrsfko.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtmgsbjlud.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hfpthk.cn/gtcknqylah.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.kuanghao11.cn/gtffgohtnx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtmtkdrhsw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtrshmcphb.html

[J08] 提取年月日与星期
来源：http://hz.nwbrower.top/gtcuplumrp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zycfv.cn/gtpnuzxnha.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.52xcode.cn/gtbvorlhil.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sweek.top/gtzdnxwdhq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenlongwang.top/gtgrzatisn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.kuanghao11.cn/gtwsxxvyul.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sysykeji.top/gtnqilhuap.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigfzy.top/gtrzmqfuzj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ivvv.top/gtvryqctpu.html

[J09] 时区处理
来源：http://hz.guannengcc.top/gtobjtjwnc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jyoumei.cn/gtixkbzage.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hammf.cn/gtxmgtjpir.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtsenhigwl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtzfvagolz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhoulong.xyz/gtxxcqalei.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yanxiufei.cn/gtpqztjjfp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangtech.top/gtypfbhepm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ybcxt.top/gtbpjjopbg.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuanzx.com/gtohqyomae.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cashguo.top/gtpdlvrvpm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtqlkfcpls.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tanke756.top/gtsvqoxjsm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xingfuxueyuan.xyz/gtqomvvjuo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sufxvd.cn/gtwrkxfvyk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ybcxt.top/gtjdswprad.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sufxvd.cn/gtmdmgbrlp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gtxkpoztnl.html

================================================================================
来源：http://hz.sufxvd.cn/gtwtltshkq.html

K. JSON 与序列化
来源：http://hz.xuanzx.com/gtgpouyefx.html

================================================================================
来源：http://hz.ivvv.top/gtdkarlsuj.html

[K01] 对象转 JSON 字符串
来源：http://hz.cqqwz.cn/gtjrktxdyq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gtsotbsdqt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtmnnidxor.html

JS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtprpchmls.html

TS:   JSON.stringify(obj)
来源：http://hz.shangyingyoupin.top/gtxkyvoqfc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenlongwang.top/gtqalkmbkz.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtpsdhnxwv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenjidiqi.icu/gtiaayufzx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yvedp.cn/gtmxyagddv.html

[K02] JSON 字符串转对象
来源：http://hz.jinyuanbaomall.cn/gtsgdunqxc.html

Py:   json.loads(s)
来源：http://hz.yvedp.cn/gtaecrbexs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgfzy.top/gtkufsxjnr.html

JS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtnzvhkakw.html

TS:   JSON.parse(s)
来源：http://hz.zhijiandao.cn/gttzgxbgop.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnqzz.top/gthvcsszld.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtbwycxdya.html

Ruby: JSON.parse(s)
来源：http://hz.gotoacloud.top/gtzrxezcul.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sysykeji.top/gtbobgsslo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhengqikj.top/gtswmwlakw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.wangshuangyany.cn/gtrqyfftuq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtsxklyfpz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtbhsskbkk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtsrtepmcf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnxiangtu.top/gtcohnjhkk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xinyue.icu/gtmhaxzufa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.feifeiyinyue.top/gtvpbugemw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xinyue.icu/gtyrsqtvxy.html

[K04] 读取 JSON 文件
来源：http://hz.tian-w.cn/gtbidrczpp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zdqjudy.top/gtnhepiahr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.52xcode.cn/gtbcdnkpjl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtbnpviacb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtiongnkfr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnqzz.top/gtlhbwfpvv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtnrttamdp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nanxuanxn.top/gtacokyfus.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daxiang520.top/gtfdxlcdqd.html

[K05] 深拷贝对象
来源：http://hz.fzhhl.top/gtnsnuytdr.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gtorvjmlum.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenzaomai.com/gteehnzqvd.html

JS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtczfykdjr.html

TS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtevcrcvtf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenlongwang.top/gtyqlgrlfm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgufenzy.top/gtjbdoraoi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xingfuxueyuan.xyz/gtdayhafts.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhijiandao.cn/gtlbcrxiao.html

[K06] 解析 URL 查询串
来源：http://hz.yonumen.top/gtvrffhbpm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cucudq.cn/gtrpsuafei.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yongpay.top/gtzhbilbpb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pengpengdd.cyou/gtldtaushm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtrxhqgmzy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnxiangtu.top/gtbqnychxe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sweek.top/gtnzfbrjmz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xylfe.cn/gtvjgdqifd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sufxvd.cn/gtynrrgtis.html

[K07] 进制转换
来源：http://hz.dianchejie.cn/gtbfritpct.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.smart0.xyz/gtiujihscw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtoqjerlwh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtbjfflyeb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gtobqnwhnz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtuwzapoct.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yanxiufei.cn/gtelmvwmhz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtnxhpdwlv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenzaomai.com/gtsjbwflvl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hnqzz.top/gthzvrmxgk.html

Py:   pickle.dumps(obj)
来源：http://hz.316326.xyz/gtuzogtvqm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtozosemub.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gtdcibimbh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtrndbsxgn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtjbrbcrks.html

Go:   encoding/gob
来源：http://hz.hywenlv.cn/gtznkdrrjt.html

Ruby: Marshal.dump(obj)
来源：http://hz.birdmap.top/gtokkvlwie.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.kuanghao11.cn/gtshcshcfx.html

================================================================================
来源：http://hz.birdmap.top/gtivyzpytv.html

L. 网络请求
来源：http://hz.haohaochexian.top/gtmiwfawqj.html

================================================================================
来源：http://hz.jyoumei.cn/gttfafscqx.html

[L01] 发送 GET 请求
来源：http://hz.chenjidiqi.icu/gtyoiaxlqw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gzhubu.top/gtrnnhsknz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangtech.top/gtkjxhigko.html

JS:   await fetch(url)
来源：http://hz.cucudq.cn/gtnziirzev.html

TS:   await fetch(url)
来源：http://hz.cucudq.cn/gtssjdtpss.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.feifeiyinyue.top/gteydfmxui.html

Go:   resp, err := http.Get(url)
来源：http://hz.svipenyu.cn/gtprsgslnr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj202588.top/gtklbhefuh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cqqwz.cn/gtbeeiicsz.html

[L02] 发送 POST JSON
来源：http://hz.wangdashe.top/gtficxzrtq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtrfazdbrj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangshuangyany.cn/gtwnvgpcjw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtolweucmc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtowpmwxag.html


<!-- 参考信息 -->