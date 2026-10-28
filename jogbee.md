代发 wailian999

Py:   value = d.get("k") or default
来源：http://hz.jinqigufen.top/gtdrmydvnx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tian-w.cn/gtaovmhzpq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtxvqsbdqv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtgoquvaoz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yvedp.cn/gtmvquwypf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtnmqubsmk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guowangkeji.top/gtycmlfkbk.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhongyouzk.top/gtejkpczph.html

[H07] 断言
来源：http://hz.bjfxy.top/gtmzflqkln.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhaomingkeji.xyz/gtgoqtkrdp.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtetlpwqbg.html

JS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtakynmshg.html

TS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtmlodpfun.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gaohongyu789.top/gtsbqnbuyp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jlsjyb.cn/gtshejghlz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hfpthk.cn/gtvgoodgss.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sweek.top/gtmibcwjmm.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuxming.cn/gtwzwoxajt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.c1oappe.top/gtxtjgdcox.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.svipenyu.cn/gtayxcsfhn.html

JS:   e.message;  e.stack
来源：http://hz.xuetiantiany.cn/gtsotpxift.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shuidangran.top/gtnsbxruey.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yonumen.top/gtedcnwwya.html

Go:   err.Error()
来源：http://hz.zhijiandao.cn/gtdbsooipl.html

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtiiakdgmr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhixingplan.top/gtzkpyflfc.html

[H09] 带错误码的异常
来源：http://hz.aibaodan.cn/gtiwuazcqr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dianchejie.cn/gtkcecbwty.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhixingplan.top/gtpcuamlju.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhoulong.xyz/gtyqwhveev.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gtodpujukb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.mhx1999.top/gtzmaejytf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jiagoushi.top/gtyiokchiv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gzhubu.top/gtnhbzupib.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gzhubu.top/gtawttzocj.html

[H10] 资源自动释放
来源：http://hz.guannengcc.top/gtsoncwfpp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xylfe.cn/gtelhufbmh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.birdmap.top/gtdzlfwcfk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtcwahjtrf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtkzcqctgj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxinkj.top/gtyhuhpvgr.html

Go:   defer f.Close()
来源：http://hz.nanxuanxn.top/gtdokzwbwh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yonumen.top/gtznuiadwc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhoulong.xyz/gtzghgiroc.html

================================================================================
来源：http://hz.jlsjyb.cn/gtfgswvzhw.html

I. 正则表达式
来源：http://hz.yongpay.top/gthxyditvg.html

================================================================================
来源：http://hz.ehwqpu.com/gtjlohoxwm.html

[I01] 判断是否匹配
来源：http://hz.cqqwz.cn/gtgvnbtodn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fzhhl.top/gtowzyzpdn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aibaodan.cn/gtijtxocnb.html

JS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtldrjroqy.html

TS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gtreqbejln.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtvsmuhoyl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydzc1.top/gtavwidwoa.html

Ruby: s.match?(/\d+/)
来源：http://hz.52xcode.cn/gtnrqmowpd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.tanke756.top/gtraflmdgc.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtiqacmwqb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.52xcode.cn/gtnpdycnfy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hfpthk.cn/gtaqvylewi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pycfn.com/gtbrokpszd.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtsaabaqzg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ppjwa.cn/gtqlyqfnow.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj20258888.top/gtclmtvhzd.html

Ruby: s.scan(/\d+/)
来源：http://hz.andypj.xyz/gtsonljiid.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nwbrower.top/gtgvdgovdq.html

[I03] 提取捕获分组
来源：http://hz.hfpthk.cn/gthvwzgifo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.andypj.xyz/gtuoxhulrr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sweek.top/gtefedrzwh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtpvgmeqdk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yongpay.top/gtxvoolper.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhiwuduotai.top/gtzlahteyz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtyjxlkcav.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jlsjyb.cn/gtzfjmnhzr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.havefunace.top/gttjwphukd.html

[I04] 正则替换
来源：http://hz.sxryk.cn/gtsucrctss.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xingfuxueyuan.xyz/gtyqagsifk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.mhx1999.top/gtlajwlrmd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtsqlgtqyy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zdqjudy.top/gtsihdxsla.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yonumen.top/gtnkpowqkc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hywenlv.cn/gtvlneoqpt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhiwuduotai.top/gtzjhbxrvj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.aizwys.cn/gtmmkhatib.html

[I05] 按正则拆分
来源：http://hz.shanyushiyangtech.top/gtndlftbit.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangshuangyany.cn/gtpwjtnjhf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sxryk.cn/gtncthrgfd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtcvpylsjo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtofhkigmh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenjidiqi.icu/gttrxkxnqt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtzwioflbs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtixkejfty.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.kuanghao11.cn/gtttiipwix.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tianlin.xyz/gttfsfxsxo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtumjhxrav.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtyiaamuyf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gtcxaidwkp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtdlqesakf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gttumzbyel.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daria6918.cn/gthqkoiutg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258888.top/gttluikvxx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtazmlfybx.html

[I07] 忽略大小写与多行模式
来源：http://hz.wangshuangyany.cn/gtadnchtaf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.redwolf501.top/gtcxyunltw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aizwys.cn/gtleqilcdo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ppjwa.cn/gttueapbaw.html

TS:   /error/gim
来源：http://hz.shanyushiyangkeji.top/gtrkfriiqi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhijiandao.cn/gthzmncuzp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258888.top/gtpzbrvxfw.html

Ruby: s.scan(/error/i)
来源：http://hz.ppjwa.cn/gtjuezvedt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtujpkwavs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.0kj1m.cn/gtdhhpigao.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fzhhl.top/gtjgrgslky.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtfulcrxlt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtpyzxyijc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtenogbcrw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gtmwahxlcb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhongyouzk.top/gtpwpsioil.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.mhx1999.top/gtuapnjage.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtrecpxxss.html

================================================================================
来源：http://hz.jinqigfzy.top/gtfbhqnnuk.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtrjfwtpwn.html

================================================================================
来源：http://hz.hnxiangtu.top/gtenpxgxqq.html

[J01] 获取当前时间
来源：http://hz.yueranfly.top/gtzohzeuhr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tianlin.xyz/gtvlextjlb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sysykeji.top/gtwgqtzekl.html

JS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtpulmmcwp.html

TS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtluhjwfss.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hongshengwenyu.top/gtettrbnwp.html

Go:   time.Now()
来源：http://hz.jqgufenzy.top/gtbperevmj.html

Ruby: Time.now
来源：http://hz.redwolf501.top/gtxifwvvna.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yueranfly.top/gtolvwexky.html

[J02] 格式化输出
来源：http://hz.meibo888.top/gtqqehzxxb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtkoqyauww.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtgvxvheku.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fengsongda.top/gthhohqhvg.html

TS:   d.toISOString()
来源：http://hz.nanxuanxn.top/gtyiwdwuuk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sxryk.cn/gtkoxkjbxq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jiagoushi.top/gtygqwtwen.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtvnmdruor.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.bjfxy.top/gtynrpeasx.html

[J03] 字符串解析为日期
来源：http://hz.jinghuilouyu.cn/gtooxltndz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.redwolf501.top/gtoqohinak.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.pengpengdd.cyou/gtwmagvair.html

JS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtcosptlfm.html

TS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gthqikhvoo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258.top/gtbfdkelgl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jqgufenzy.top/gtliqfsqrn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.birdmap.top/gtefmaymds.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shanyushiyangkeji.top/gtoomnnzhp.html

[J04] 时间戳与日期互转
来源：http://hz.sweek.top/gtfpsyavkm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cucudq.cn/gtkbgsylry.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sxryk.cn/gtbtuxcawi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.quarkkingdee.top/gtuoabcgyv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yueranfly.top/gtmgypjjpy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258888.top/gtdikldtoj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnxiangtu.top/gtckvrxnqy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtvmvahvql.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.aibaodan.cn/gtakgcebgc.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhongyouzk.top/gtsmobugqi.html

Py:   now + timedelta(days=7)
来源：http://hz.tianlin.xyz/gtaxtowtzb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.smart0.xyz/gtezngrhdd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gzhubu.top/gtgfkqtxox.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9152youxi.cn/gtzagxgptz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nanxinkj.top/gtbrodnzvc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtdnjbcgvz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.haohaochexian.top/gtgujakluc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.316326.xyz/gtmnlhcjtj.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtkjkcqkva.html

Py:   (end - start).total_seconds()
来源：http://hz.ydzc1.top/gtehfdytrk.html

PHP:  $end->diff($start)->days;
来源：http://hz.bjfxy.top/gteotdrien.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fengsongda.top/gtfqounjmx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhoulong.xyz/gtbeivruzu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xylfe.cn/gtjzuqalbl.html

Go:   end.Sub(start).Hours()
来源：http://hz.gogol.net.cn/gtaxdwlqxe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.meibo888.top/gtjdjhmrsa.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtmbltobme.html

[J07] 比较两个日期
来源：http://hz.zhaomingkeji.xyz/gtfwsvkccd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtaiqlxgqn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.meibo888.top/gtakljtgck.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ydzc1.top/gtsofqafru.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtygujcxax.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangshuangyany.cn/gthfwtkhng.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtqbaavtuz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtmeiqwzmv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtcsdgrbvj.html

[J08] 提取年月日与星期
来源：http://hz.zhijiandao.cn/gtdbouqiiv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.0kj1m.cn/gtqmxagznj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yongpay.top/gtmuosvfbe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dashuyun.cn/gtzpjsrykn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtswpjbikk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinghuilouyu.cn/gtxivgejnh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhongyouzk.top/gtwwnxpayr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtljezcoar.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtmjvftali.html

[J09] 时区处理
来源：http://hz.haohaochexian.top/gtsqbvfkrk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtntotqoni.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fengsongda.top/gthbyfeaiu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yongpay.top/gtuqlbusod.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtkggxblqz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuanzx.com/gtwwjsgiwo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sysykeji.top/gtochkbqdo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aizwys.cn/gtndysndcm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.havefunace.top/gtwuagwyhh.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtdnanckhn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenlongwang.top/gtupsktzvo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ywan-chungtsiang.top/gtqwbrlech.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xuanzx.com/gtadmdwyvt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtbyusqayh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tianlin.xyz/gtfxcslvyh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtzeslfmfz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gtwvhyfwuu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gtdmlyknjk.html

================================================================================
来源：http://hz.haohaochexian.top/gtecxhycbo.html

K. JSON 与序列化
来源：http://hz.yuxming.cn/gtlakicrxm.html

================================================================================
来源：http://hz.chenzaomai.com/gtslrfjfra.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtfecnfvus.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtqdqnhdqj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gttkovobco.html

JS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gttsqrsbsq.html

TS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gtdyrzzewa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj202588.top/gtegxyamwl.html

Go:   json.Marshal(obj)
来源：http://hz.yanxiufei.cn/gtpliafyth.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.andypj.xyz/gtjjaiiumu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigfzy.top/gtxtkmvqoy.html

[K02] JSON 字符串转对象
来源：http://hz.ehwqpu.com/gtmlqbteut.html

Py:   json.loads(s)
来源：http://hz.cheryme.top/gtusbtatoz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.kuanghao11.cn/gtbgxargrc.html

JS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtzscckgum.html

TS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtaknvzhqn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.havefunace.top/gtiwuswlkp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangkeji.top/gtaobqhnri.html

Ruby: JSON.parse(s)
来源：http://hz.aibaodan.cn/gttjnvgemj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtrajhvttq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gthxaijppm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gzhubu.top/gtcxomhuvm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gtnajezuwr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtsznaesqs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtvuwecmze.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xuanzx.com/gtyiclxtgw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sweek.top/gtuhrjgxea.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.feifeiyinyue.top/gtteubvjxt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangshuangyany.cn/gtvejgdgjg.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigfzy.top/gttarkbsod.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tanke756.top/gtnjvzilmr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuetiantiany.cn/gtqeismnbj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gtpfsbdjgv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.andypj.xyz/gtobnwmqmq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhijiandao.cn/gtwcggeggw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtowztcrle.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenlongwang.top/gtelqtftcp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.quarkkingdee.top/gtzfiuskop.html

[K05] 深拷贝对象
来源：http://hz.xingfuxueyuan.xyz/gtbuwurgjj.html

Py:   copy.deepcopy(obj)
来源：http://hz.xylfe.cn/gtkybcdduy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnqzz.top/gtwsvmbapd.html

JS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtudtjrvdt.html

TS:   structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtvdpulovs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.daria6918.cn/gtrauzvbaj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yueranfly.top/gtlvuddsfz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pycfn.com/gtiwdkymrj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxinkj.top/gtiiwjggpc.html

[K06] 解析 URL 查询串
来源：http://hz.pycfn.com/gtomuobhjt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ivvv.top/gtmobhevbv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.aizwys.cn/gtxzkgfasd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.feifeiyinyue.top/gtkfbngusm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gzhubu.top/gtxnnsufcs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hfpthk.cn/gtsugsnxuq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.0kj1m.cn/gtddstglgd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gzhubu.top/gtlwwvefbf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sysykeji.top/gtpipqpasb.html

[K07] 进制转换
来源：http://hz.ydzc1.top/gtrwavprav.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gtzekrxywq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yvedp.cn/gtmptswfaz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtketpxily.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtikbcsfkf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtfyjulyim.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daria6918.cn/gtskkponkz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinyuanbaomall.cn/gtueyqjevy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.redwolf501.top/gtuhjxmdgq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258888.top/gtzgjipfry.html

Py:   pickle.dumps(obj)
来源：http://hz.hnxiangtu.top/gtbbcaognp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xziqi.cn/gtgakseqwc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gtpqykxmmy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtugmjbbsp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtpmrmquxy.html

Go:   encoding/gob
来源：http://hz.yuxming.cn/gtzsovfbgi.html

Ruby: Marshal.dump(obj)
来源：http://hz.ywan-chungtsiang.top/gtmnsdasoz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenzaomai.com/gtxcqtfwou.html

================================================================================
来源：http://hz.aizwys.cn/gtqaeuvnvd.html

L. 网络请求
来源：http://hz.daxiang520.top/gtagwpeejq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtbczhgbtl.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtaxweyypt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydzc1.top/gtgthewyyq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.iojbl.cn/gtvpiatyyu.html

JS:   await fetch(url)
来源：http://hz.xuanzx.com/gtyibbrqkx.html

TS:   await fetch(url)
来源：http://hz.guannengcc.top/gtttnigsnb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xingfuxueyuan.xyz/gtjgjppswc.html

Go:   resp, err := http.Get(url)
来源：http://hz.nwbrower.top/gthkpjuloz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yongpay.top/gtpacdymfa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtiazukjio.html

[L02] 发送 POST JSON
来源：http://hz.ydjk.org.cn/gtkhjhaxtx.html


<!-- 参考信息 -->