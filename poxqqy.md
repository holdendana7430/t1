代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigufen.top/gtxqhkycmk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.meibo888.top/gtvefvyqxg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuanzhike.top/gtexauttex.html

C#:   obj?.A?.B ?? default
来源：http://hz.snrcjt.cn/gtuhwytvzl.html

[H07] 断言
来源：http://hz.xuetiantiany.cn/gtezdoxruc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.tianlin.xyz/gterdbieyr.html

PHP:  assert($x > 0);
来源：http://hz.9152youxi.cn/gthcnuwiva.html

JS:   console.assert(x > 0);
来源：http://hz.yonumen.top/gtzvhavnpo.html

TS:   console.assert(x > 0);
来源：http://hz.sxryk.cn/gtackhddlf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.redwolf501.top/gtvooptluu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jiagoushi.top/gtvqfqbxbg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shuidangran.top/gtaghypziu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigfzy.top/gtvfmpopxj.html

[H08] 获取错误信息与堆栈
来源：http://hz.cheryme.top/gtqlrppgxu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gzhubu.top/gtkdsbffkt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zycfv.cn/gthlhtukfm.html

JS:   e.message;  e.stack
来源：http://hz.jyoumei.cn/gtvaxgjwvl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.feifeiyinyue.top/gtmrvsktxa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yueranfly.top/gtgowmudeq.html

Go:   err.Error()
来源：http://hz.cheryme.top/gtxsbttomy.html

Ruby: e.message;  e.backtrace
来源：http://hz.gogol.net.cn/gteivyxtdj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hfpthk.cn/gtxbfdrrzr.html

[H09] 带错误码的异常
来源：http://hz.svipenyu.cn/gtpsxeqzbi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnxiangtu.top/gtdsegcjdr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gogol.net.cn/gtoqznters.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuetiantiany.cn/gtqyxsiepp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tanke756.top/gtiivziloc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenjidiqi.icu/gtbrtxipla.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jyoumei.cn/gttjldfajx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj202588.top/gtlfnnwzwv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xingfuxueyuan.xyz/gtrpcdltum.html

[H10] 资源自动释放
来源：http://hz.yj202588.top/gtuuuiezdk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258.top/gtzbvtgkyh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ivvv.top/gtujmxhpqd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gthctdyfls.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gtqumnofop.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cucudq.cn/gtjmnzxipt.html

Go:   defer f.Close()
来源：http://hz.kuanghao11.cn/gtrdhvtvnb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.meibo888.top/gtwprlvjfe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhijiandao.cn/gtrhiacjus.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgtddmewh.html

I. 正则表达式
来源：http://hz.zhongyouzk.top/gtitttabqt.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjumymrji.html

[I01] 判断是否匹配
来源：http://hz.jlsjyb.cn/gtldkqfbrg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zdqjudy.top/gtridhufni.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtzfqltqro.html

JS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtqtvrdadx.html

TS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtdzwkvxea.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jlsjyb.cn/gtejoptjui.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fengsongda.top/gtsusqaxiv.html

Ruby: s.match?(/\d+/)
来源：http://hz.snrcjt.cn/gtoajhseta.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.bjfxy.top/gtymffeigg.html

[I02] 提取所有匹配
来源：http://hz.zycfv.cn/gtegyhwoif.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gtggtgvaha.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.9152youxi.cn/gtnmndfbwl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zdqjudy.top/gteldijjkl.html

TS:   s.match(/\d+/g)
来源：http://hz.gotoacloud.top/gtwpawqtmv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.vqdsnc.cn/gtqgicwyjh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.fengsongda.top/gtohuibzmp.html

Ruby: s.scan(/\d+/)
来源：http://hz.cqqwz.cn/gtzvlvbzkl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shuidangran.top/gtkabmdboo.html

[I03] 提取捕获分组
来源：http://hz.nanxuanxn.top/gtylfutqdg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hammf.cn/gtfnfmyffw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dashuyun.cn/gtwumxqcuj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtjmvhdigj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yanxiufei.cn/gtiiyzbotx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.bjfxy.top/gtdjrbaxet.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zycfv.cn/gtgqawgzce.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.fzhhl.top/gtkcaqzhjd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtolpvycmj.html

[I04] 正则替换
来源：http://hz.sweek.top/gtqofplprl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xuanzx.com/gtepmdvyrx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhengqikj.top/gtqgwipbas.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtnmoejxmn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtdqyvvexs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dianchejie.cn/gtcgwubnlb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aibaodan.cn/gtnzlgauvj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yongpay.top/gtolravope.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ehwqpu.com/gtvvbioeyp.html

[I05] 按正则拆分
来源：http://hz.tian-w.cn/gtmfacmioz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydzc1.top/gtuhvludhn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cqqwz.cn/gtiialifyi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtsffrqihb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtiwblljxs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cashguo.top/gthhqulrmd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.iojbl.cn/gtgfvttylw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtxewekctk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yanxiufei.cn/gtsamgpogw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aibaodan.cn/gttrpnvnrq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gttanptmqo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jiagoushi.top/gtvsrftrkb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtgsmmmvrw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtoxhynxyy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ppjwa.cn/gthccvprna.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigfzy.top/gtiwmkkxeq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pycfn.com/gtxunawtfz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtleiamked.html

[I07] 忽略大小写与多行模式
来源：http://hz.cucudq.cn/gtymwekorw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tanke756.top/gtqbyfbmee.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daria6918.cn/gtzsoebghn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xziqi.cn/gtznibyowi.html

TS:   /error/gim
来源：http://hz.aibaodan.cn/gttsfisvpi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.meibo888.top/gtvzvxejkn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hysaishi.cn/gtefkstiji.html

Ruby: s.scan(/error/i)
来源：http://hz.yangfankeji.com/gtpqraspwo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yvedp.cn/gtysvskpwl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jlsjyb.cn/gtnansjhul.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jianghu66.top/gtjoasqhxk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgfzy.top/gtfbsibptv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtvzbfftey.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxuanxn.top/gtrbdirgxh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhongyouzk.top/gtxfsepbbi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cashguo.top/gttztesxrc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hongshengwenyu.top/gtadfolxrs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sysykeji.top/gturvifyvl.html

================================================================================
来源：http://hz.52xcode.cn/gtmgfzbawd.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtvfompqvq.html

================================================================================
来源：http://hz.gaohongyu789.top/gttdnemihq.html

[J01] 获取当前时间
来源：http://hz.andypj.xyz/gtbjucrosd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxuanxn.top/gtduehexby.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cucudq.cn/gtgtcnjqzt.html

JS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtugshtgbm.html

TS:   new Date();  Date.now()
来源：http://hz.pengpengdd.cyou/gtpkhcjqmr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yongpay.top/gtqbqbhjnn.html

Go:   time.Now()
来源：http://hz.jqgufenzy.top/gttnxuzhpl.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtvfqqagbi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aibaodan.cn/gtdktvmwfl.html

[J02] 格式化输出
来源：http://hz.pycfn.com/gtpgfobkck.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pycfn.com/gtrukshmkv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtpgjivozw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydzc1.top/gtsnzhpcyp.html

TS:   d.toISOString()
来源：http://hz.gzhubu.top/gtfbydszty.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ywan-chungtsiang.top/gtmsswimvg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gtatltrawu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gotoacloud.top/gtxrgjovsw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gtvnbzqjyb.html

[J03] 字符串解析为日期
来源：http://hz.shuidangran.top/gtbaflalgz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nanxinkj.top/gtkzobddqr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ehwqpu.com/gthgfmywks.html

JS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtdlhgpctp.html

TS:   new Date("2024-01-02")
来源：http://hz.cashguo.top/gtnreuqqyk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuanzx.com/gttpppdbnq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.vqdsnc.cn/gtggsbevzf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtbjebbdyv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yvedp.cn/gtqauibftw.html

[J04] 时间戳与日期互转
来源：http://hz.zhaomingkeji.xyz/gtofomvhud.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zdqjudy.top/gtqownekuq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yonumen.top/gtvczyrltg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tanke756.top/gtmvceuciw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.birdmap.top/gtbutiomvk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yanxiufei.cn/gtibhsgxvj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hammf.cn/gtepdvfzpy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtxxopviim.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zdqjudy.top/gtwnoefccl.html

[J05] 时间加减（加 7 天）
来源：http://hz.0kj1m.cn/gtfdqynlek.html

Py:   now + timedelta(days=7)
来源：http://hz.birdmap.top/gtzdmakouz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxinkj.top/gtlzvyodju.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gtlpxskrqn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtyiacynpl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangtech.top/gtlofefxqk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.0kj1m.cn/gtmxgdqkms.html

Ruby: Time.now + 7 * 86400
来源：http://hz.haohaochexian.top/gtzkebznim.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.bjfxy.top/gtezlwwpgp.html

[J06] 计算两时间之差
来源：http://hz.daria6918.cn/gtjbwsetng.html

Py:   (end - start).total_seconds()
来源：http://hz.yangfankeji.com/gtxdicthre.html

PHP:  $end->diff($start)->days;
来源：http://hz.sufxvd.cn/gtwzabolrm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jqgufenzy.top/gtqvrkqbvn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shuidangran.top/gtqzjtsrgk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daria6918.cn/gtxahsxkxz.html

Go:   end.Sub(start).Hours()
来源：http://hz.cucudq.cn/gtgqdntihq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xinyue.icu/gtzxbakwrm.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgufenzy.top/gtgwbgvisz.html

[J07] 比较两个日期
来源：http://hz.aibaodan.cn/gtvarmcoyz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtlyqtpvku.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ppjwa.cn/gtqwtsbcuc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtvklbkami.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtlnvovpfd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinghuilouyu.cn/gtyfxblggg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtpzjcrsqt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtrpvxzvze.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gthyeqwckd.html

[J08] 提取年月日与星期
来源：http://hz.smart0.xyz/gtzindzwjl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cucudq.cn/gtzafrunqb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.haohaochexian.top/gtqclncltf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aibaodan.cn/gtovtbqvye.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinghuilouyu.cn/gtajwjlavv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.9152youxi.cn/gtxuwlxhro.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cashguo.top/gtzdtsiwwv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.vqdsnc.cn/gtvpjxmtxq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xingfuxueyuan.xyz/gtzsnozksq.html

[J09] 时区处理
来源：http://hz.daria6918.cn/gtrpqxszyt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgfzy.top/gtgyonsjyi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gaohongyu789.top/gtkrhcmveq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtsfemctoy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtxlofypda.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yangfankeji.com/gtwmuvypzw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zdqjudy.top/gtfzbmmant.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ywan-chungtsiang.top/gtexfzoxzv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fengsongda.top/gtxlonakzl.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhiwuduotai.top/gtquxlpdib.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cucudq.cn/gtpffyhkir.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtvszcdkwc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtijguzusw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtngtmnpau.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hammf.cn/gtzibjixvj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhengqikj.top/gtjuycmnqm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuxming.cn/gtrcnrvclh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gogol.net.cn/gtxsuednrc.html

================================================================================
来源：http://hz.tanke756.top/gtwffaeiqc.html

K. JSON 与序列化
来源：http://hz.shuidangran.top/gtmybvtecb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtlcuhibpk.html

[K01] 对象转 JSON 字符串
来源：http://hz.redwolf501.top/gtzgprdbmz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtslirnkow.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gtxkgocxeq.html

JS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtgzncklie.html

TS:   JSON.stringify(obj)
来源：http://hz.sufxvd.cn/gteskyebcl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhijiandao.cn/gtgwwvbvmq.html

Go:   json.Marshal(obj)
来源：http://hz.zhaomingkeji.xyz/gtuwmqaxxm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinghuilouyu.cn/gtovkxzevz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydzc1.top/gtfkgvotli.html

[K02] JSON 字符串转对象
来源：http://hz.zhoulong.xyz/gtevfnkfpo.html

Py:   json.loads(s)
来源：http://hz.hnqzz.top/gtabdwssoc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.vqdsnc.cn/gtwtapwbwe.html

JS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gttwgqsmdn.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtxiiwkpts.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtclblbjgm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gtglmykzeo.html

Ruby: JSON.parse(s)
来源：http://hz.ppjwa.cn/gtjyjdxzeu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtoeauanax.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sxryk.cn/gtrvbibjkv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gtgmopbglr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gtskcdwfar.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtiewapxxw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.redwolf501.top/gtuddpkgmf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gtkngloaut.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gtwhgplyqp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.316326.xyz/gtgffkwgnp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigfzy.top/gtumwszskp.html

[K04] 读取 JSON 文件
来源：http://hz.cqqwz.cn/gtytkstfyj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jiagoushi.top/gtvbnihczu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.kuanghao11.cn/gtwgzbazdo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtufapegjc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtjdzejxct.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.redwolf501.top/gtzmbvuqbt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtbkmlndgv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jiagoushi.top/gtrkpoddzx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sxryk.cn/gtmfehbghr.html

[K05] 深拷贝对象
来源：http://hz.svipenyu.cn/gtqgexqsco.html

Py:   copy.deepcopy(obj)
来源：http://hz.jqgufenzy.top/gthuvwjiwg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cucudq.cn/gtccwnqwkl.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gttvlhjjpt.html

TS:   structuredClone(obj)
来源：http://hz.9152youxi.cn/gtfzltnuli.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cashguo.top/gtvbvuonlf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daxiang520.top/gtnimvnvyx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.havefunace.top/gtvnmuoimx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zdqjudy.top/gtkdwjbwmt.html

[K06] 解析 URL 查询串
来源：http://hz.jinghuilouyu.cn/gtsmkabnwi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zycfv.cn/gtwalqvjhp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hammf.cn/gtcwzxrqvy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gttyiusajv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtxcgwxhqd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fzhhl.top/gtfotgwklu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cdnleiting.top/gtkcsncjxg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnqzz.top/gtvnlvrehj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ivvv.top/gtcaofvldb.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gtoneajstw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hammf.cn/gtpopbuing.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenjidiqi.icu/gtigstghlf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtzzlisqrp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtkjskrpvm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtyghuqush.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.c1oappe.top/gtqwxxflag.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenjidiqi.icu/gtuekwlkvl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cheryme.top/gtbvcbwbtj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.quarkkingdee.top/gtqxxemefh.html

Py:   pickle.dumps(obj)
来源：http://hz.316326.xyz/gturehyisg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.aizwys.cn/gtjgbfxqod.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtlhpcmuwy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gtoavvustf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj202588.top/gtjibobcaw.html

Go:   encoding/gob
来源：http://hz.ppjwa.cn/gtlhnqrxbf.html

Ruby: Marshal.dump(obj)
来源：http://hz.yvedp.cn/gtmjcbgwfd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.iojbl.cn/gtzuglrskg.html

================================================================================
来源：http://hz.zhoulong.xyz/gtewpqcaep.html

L. 网络请求
来源：http://hz.hywenlv.cn/gtznnkvcrp.html

================================================================================
来源：http://hz.havefunace.top/gtryikhgvu.html

[L01] 发送 GET 请求
来源：http://hz.kuanghao11.cn/gtspugknyt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.52xcode.cn/gtchmxrspu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigufen.top/gtybpvdkin.html

JS:   await fetch(url)
来源：http://hz.yongpay.top/gtuazbubfx.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtalvyzfrv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.meibo888.top/gtpmgsgavl.html

Go:   resp, err := http.Get(url)
来源：http://hz.hywenlv.cn/gtatemvcpu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daria6918.cn/gtzsastczi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.guowangkeji.top/gttgmwtiiz.html

[L02] 发送 POST JSON
来源：http://hz.pengpengdd.cyou/gtgaolfehk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hnxiangtu.top/gtudnrknno.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhijiandao.cn/gtaycgcema.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gttvjyndqv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtaayjkuoc.html


<!-- 参考信息 -->