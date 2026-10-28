代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.feifeiyinyue.top/gtrjmzfgqi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xylfe.cn/gtfkwlzfmy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtcvgnhtil.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ydjk.org.cn/gtsoqftvas.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhixingplan.top/gtwjircapc.html

Ruby: rescue ArgumentError => e
来源：http://hz.sysykeji.top/gtgqnnpwiu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhiwuduotai.top/gtitylliis.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jiagoushi.top/gtksfcylte.html

Py:   value = d.get("k") or default
来源：http://hz.ivvv.top/gttczdhtqr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yueranfly.top/gttncdaflg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.9152youxi.cn/gtfbmbvzwf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtaoozobth.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.svipenyu.cn/gtqbfyigeh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daria6918.cn/gtuoodjfsw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtahnfilky.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxuanxn.top/gthkweblys.html

[H07] 断言
来源：http://hz.shanyushiyangtech.top/gtzpqrxlrq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.9152youxi.cn/gtjgxpbjxz.html

PHP:  assert($x > 0);
来源：http://hz.jqgfzy.top/gtgoslvyct.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtkmkurkzh.html

TS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gtjncffvgh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zycfv.cn/gthhqvxqsh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangkeji.top/gtvbzuovks.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinghuilouyu.cn/gtxokbsrgd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jiagoushi.top/gtlilvlljl.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258.top/gtmiwqwhky.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuetiantiany.cn/gtxtwqpjoh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.snrcjt.cn/gtasxrxnqn.html

JS:   e.message;  e.stack
来源：http://hz.gaohongyu789.top/gtmxuquwev.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj202588.top/gtyhmlrxpv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yj20258.top/gttucijehv.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtidqnjnel.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhengqikj.top/gtfdsyoaii.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cashguo.top/gttxskzzzt.html

[H09] 带错误码的异常
来源：http://hz.pengpengdd.cyou/gtpobwssue.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.316326.xyz/gtbbuqrmhh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yanxiufei.cn/gtcldcdmkf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenjidiqi.icu/gtsionohqi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tianlin.xyz/gttfftwprs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinyuanbaomall.cn/gtbxtqgcfl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.havefunace.top/gttkmqtrjo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sweek.top/gtqajeybkh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.haohaochexian.top/gtsbplqswa.html

[H10] 资源自动释放
来源：http://hz.zhijiandao.cn/gtrxwmofxy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gzhubu.top/gtqmfigpew.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tanke756.top/gtzsehvqvh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gthlftpmqh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtstcurequ.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ppjwa.cn/gtmpxnbulz.html

Go:   defer f.Close()
来源：http://hz.9152youxi.cn/gtwcoyzszw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xingfuxueyuan.xyz/gtxfedrxve.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gaohongyu789.top/gtblyhzdel.html

================================================================================
来源：http://hz.smart0.xyz/gtrwmdcizh.html

I. 正则表达式
来源：http://hz.shanyushiyangtech.top/gtyvedwazv.html

================================================================================
来源：http://hz.mhx1999.top/gtnzhlylyr.html

[I01] 判断是否匹配
来源：http://hz.chenzaomai.com/gtyjyeowyt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xinyue.icu/gtcobuzblc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtrqznaefm.html

JS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gtrjqjazxt.html

TS:   /\d+/.test(s)
来源：http://hz.tian-w.cn/gtfsxonkpn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.vqdsnc.cn/gteyohfdqa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuanzhike.top/gteqqomlcf.html

Ruby: s.match?(/\d+/)
来源：http://hz.gotoacloud.top/gtkiskkmbg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenzaomai.com/gtjeziocgw.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gtvtlpkzov.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daria6918.cn/gtryspimum.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nwbrower.top/gtwquliveo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cheryme.top/gtwfgazntk.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgfzy.top/gtwokhtibs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangkeji.top/gtqrukubev.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xylfe.cn/gtemudltxs.html

Ruby: s.scan(/\d+/)
来源：http://hz.tanke756.top/gtdlbrokjm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zycfv.cn/gthtsmquad.html

[I03] 提取捕获分组
来源：http://hz.shangyingyoupin.top/gtodhmiqtv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fzhhl.top/gtfngruixl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jlsjyb.cn/gtkdscemyy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ppjwa.cn/gtwiivaiyg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ehwqpu.com/gtqdxlqbji.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tianlin.xyz/gtnfpggqjr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.52xcode.cn/gtwvfyyigt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.snrcjt.cn/gtxfhimxam.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shangyingyoupin.top/gtxczblvbe.html

[I04] 正则替换
来源：http://hz.chenzaomai.com/gtuzkhxqtg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hnxiangtu.top/gthisdfeyf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtcusfqetu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtavowwble.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtwhsokqyn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ehwqpu.com/gtlamcvoat.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydzc1.top/gtfxxmdgvl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zdqjudy.top/gteocrlrym.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.iojbl.cn/gtkwwxlxrb.html

[I05] 按正则拆分
来源：http://hz.cheryme.top/gtyisqatzg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.iojbl.cn/gtgxqzyzme.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuetiantiany.cn/gtodrdaume.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtpkyecnpg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtopzuzhbx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aizwys.cn/gtwchimakm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhixingplan.top/gtatrycqlg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtesogaigf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinghuilouyu.cn/gtmwkctfat.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sysykeji.top/gtigrhpszg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cheryme.top/gtayyqjrdn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yanxiufei.cn/gtdjmkvydx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gttvbfghub.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gtjscfkxpu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtmsonkpdm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ppjwa.cn/gtdqrzabns.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenzaomai.com/gttjgjybpf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shangyingyoupin.top/gtlnozznsn.html

[I07] 忽略大小写与多行模式
来源：http://hz.vqdsnc.cn/gtybgduond.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhixingplan.top/gtjpcjchhj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhijiandao.cn/gtzjvqtird.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tanke756.top/gtafmrnkcb.html

TS:   /error/gim
来源：http://hz.smart0.xyz/gtjechsoop.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jqgfzy.top/gtvxufkbyi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yonumen.top/gtidfwxnmb.html

Ruby: s.scan(/error/i)
来源：http://hz.shzxlz.cn/gtmenqyedk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gttxyugkcy.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yonumen.top/gtzxqqdsxv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuetiantiany.cn/gtsoqmwvfb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jyoumei.cn/gtuyerisze.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtjelfalwh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.quarkkingdee.top/gtabvpcbow.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigfzy.top/gtlbctfrsq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hywenlv.cn/gtkxbngzdt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cashguo.top/gtctbqmkwt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258888.top/gtjqwdenaf.html

================================================================================
来源：http://hz.smart0.xyz/gtigojsntx.html

J. 日期与时间
来源：http://hz.fzhhl.top/gtatiklgdy.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtumnlfxmi.html

[J01] 获取当前时间
来源：http://hz.sxryk.cn/gtpetdgbtz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhongyouzk.top/gtjkeundmv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtrqjeouze.html

JS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtlghrkcju.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtqyuzsvks.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tian-w.cn/gtdrzxrfgo.html

Go:   time.Now()
来源：http://hz.ywan-chungtsiang.top/gtqlzgxqrz.html

Ruby: Time.now
来源：http://hz.daria6918.cn/gtneetrubb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dashuyun.cn/gtzaboxgce.html

[J02] 格式化输出
来源：http://hz.daxiang520.top/gtpgkqbdpb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtirifovpw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtamhihnmp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuetiantiany.cn/gtyjpsdmcj.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtvfnzxcvu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xingfuxueyuan.xyz/gtpijxwgxi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gtxpsmgeml.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtnqlycgtv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnqzz.top/gtciasnxya.html

[J03] 字符串解析为日期
来源：http://hz.yj20258.top/gtchisdymg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.316326.xyz/gtfodwjdan.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gtndovulcf.html

JS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gtjaqfgtpr.html

TS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtahwgnvbf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtedqjcvqz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.svipenyu.cn/gtolatnfcc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuxming.cn/gtzbuevqaq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtusbkqoqv.html

[J04] 时间戳与日期互转
来源：http://hz.jqgufenzy.top/gtvsxqimnf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.quarkkingdee.top/gtuxqhjppb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gzhubu.top/gtgxqzlcmu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hongshengwenyu.top/gtafmpirpa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gtrbjdlwuw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cdnleiting.top/gtekoyroym.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fengsongda.top/gtmfbpkfny.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.redwolf501.top/gtvikcqkgq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgufenzy.top/gtbpgdjiul.html

[J05] 时间加减（加 7 天）
来源：http://hz.gzhubu.top/gtarltmykn.html

Py:   now + timedelta(days=7)
来源：http://hz.feifeiyinyue.top/gtuyzfrhqj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.9152youxi.cn/gtoukwtiau.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtfyuzwvff.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtyoeispet.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hywenlv.cn/gtbimqmble.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cheryme.top/gtyxwwkeue.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtkgkpjpdd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhongyouzk.top/gtyyfkxwea.html

[J06] 计算两时间之差
来源：http://hz.zhoulong.xyz/gtlollqnvl.html

Py:   (end - start).total_seconds()
来源：http://hz.guannengcc.top/gtegvinaxn.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuetiantiany.cn/gtuhtbcnmn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xylfe.cn/gtisuvuulb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yueranfly.top/gtcylgmizz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xylfe.cn/gtymywfdkw.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj20258.top/gtbqzkbbig.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtifybyxum.html

C#:   (end - start).TotalSeconds
来源：http://hz.yonumen.top/gtkxkftroy.html

[J07] 比较两个日期
来源：http://hz.jqgufenzy.top/gtaqkrfbis.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtsfjfmxox.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tanke756.top/gtccjrvnar.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtiuiflwiq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtxiwrmwnm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.feifeiyinyue.top/gtwnzqysic.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.iojbl.cn/gttqqaaodc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtjgxzuszb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtsdqpzabp.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangtech.top/gtjqcrrurn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shzxlz.cn/gthnehqgem.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tianlin.xyz/gtncabtedy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.svipenyu.cn/gtiiyselpn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhaomingkeji.xyz/gtkqlumbtc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.snrcjt.cn/gtevwwrowl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gtykiijfow.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtynggobyb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shzxlz.cn/gtghgaqtqi.html

[J09] 时区处理
来源：http://hz.shzxlz.cn/gtrnedkxfr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aizwys.cn/gtcgwtootu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangshuangyany.cn/gtthrfojvw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtknvqdrmq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtavhmchmq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yonumen.top/gtltynlabv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yueranfly.top/gtafulfbuv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxuanxn.top/gtuydrkvai.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dashuyun.cn/gtfevcqvgp.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuanzx.com/gtdagvbtct.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gogol.net.cn/gttmlskhqr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.svipenyu.cn/gtqrdwfnyf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hysaishi.cn/gtnssededs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xylfe.cn/gtziqlabnd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gtcydoqkax.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigfzy.top/gtvtonwmqk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ybcxt.top/gtpjrdmzjr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gtnjmdksnb.html

================================================================================
来源：http://hz.gotoacloud.top/gtmrqngszu.html

K. JSON 与序列化
来源：http://hz.yanxiufei.cn/gtbftjfsxb.html

================================================================================
来源：http://hz.sysykeji.top/gtmsvhsecq.html

[K01] 对象转 JSON 字符串
来源：http://hz.tianlin.xyz/gtlsrnomqd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtgfcofowj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtsmhfcmfn.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtuggqnkdo.html

TS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gtngvkcmqk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sxryk.cn/gtfiuwtbqz.html

Go:   json.Marshal(obj)
来源：http://hz.gzhubu.top/gttcrdlrqr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gtrxohkncf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cucudq.cn/gtxxlsneuq.html

[K02] JSON 字符串转对象
来源：http://hz.cdnleiting.top/gtucqrflom.html

Py:   json.loads(s)
来源：http://hz.cashguo.top/gtfewoyyjh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jlsjyb.cn/gtfroymfmg.html

JS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtsqshdkmm.html

TS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtmhnozirs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sysykeji.top/gtbiomjslt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtfeebkaah.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gttimlimxa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shzxlz.cn/gtmvebosyr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhongyouzk.top/gtvvvzjwhl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtvsqywoep.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtkkisawad.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtzonabfll.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtfcqitlqr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fengsongda.top/gtpgwugjde.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.haohaochexian.top/gtkdmrwixf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtaxsyzamx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dashuyun.cn/gttgpsatbz.html

[K04] 读取 JSON 文件
来源：http://hz.nanxuanxn.top/gtqrwmauqo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hammf.cn/gtzulghbdm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangdashe.top/gtscovjxwy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gtbmdeabsb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtqqkeaukj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gttljhiekw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gtuvihvpps.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gtressoucb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.52xcode.cn/gtkngenqcg.html

[K05] 深拷贝对象
来源：http://hz.wangdashe.top/gttthytkks.html

Py:   copy.deepcopy(obj)
来源：http://hz.jqgufenzy.top/gtrgeyfsvs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydjk.org.cn/gtibcppwdr.html

JS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtmnywkkgi.html

TS:   structuredClone(obj)
来源：http://hz.nanxinkj.top/gthmbkxhxu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xziqi.cn/gtrlnkgtpv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cqqwz.cn/gtqbtmymzx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenjidiqi.icu/gtnqmgtvpp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yueranfly.top/gtrlskmrrl.html

[K06] 解析 URL 查询串
来源：http://hz.sxryk.cn/gtbrhwweod.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydjk.org.cn/gtaqrslnir.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zycfv.cn/gtdlynsdyd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtqdnirhzn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtdpuntcfz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ppjwa.cn/gtvwvxwqbk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtcfiwined.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtnbxrxojk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuanzx.com/gtqogoquag.html

[K07] 进制转换
来源：http://hz.jlsjyb.cn/gtjcutraxo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtmjrxnwnv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.svipenyu.cn/gtnpybdxab.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtnrwdjfsy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yongpay.top/gtbwljvzlh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtrsfmewiu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.havefunace.top/gttbdghtdg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.bjfxy.top/gtcuzjnfjc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nwbrower.top/gthgymtnyk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenlongwang.top/gtlyksapsz.html

Py:   pickle.dumps(obj)
来源：http://hz.cucudq.cn/gtxaqnodby.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigufen.top/gtvyexnclx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cdnleiting.top/gtbithhhno.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.vqdsnc.cn/gtxjdmojsq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gtbhhacaqm.html

Go:   encoding/gob
来源：http://hz.jinghuilouyu.cn/gtltxwtljx.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtzmbeoqva.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gtrkiryeda.html

================================================================================
来源：http://hz.c1oappe.top/gttsobkfnd.html

L. 网络请求
来源：http://hz.jinyuanbaomall.cn/gtzlkgsezz.html

================================================================================
来源：http://hz.jianghu66.top/gtgefcrgnw.html

[L01] 发送 GET 请求
来源：http://hz.52xcode.cn/gtzookhsaw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnxiangtu.top/gthqdrxtpy.html


<!-- 参考信息 -->