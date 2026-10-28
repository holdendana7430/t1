代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenjidiqi.icu/gtbkzmqdrn.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuanzhike.top/gtxodjnvlg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hywenlv.cn/gtkqpgzbwe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.bjfxy.top/gtetyigsxb.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtnzmkseru.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.havefunace.top/gtiiphteqf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtgebkmzze.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gthiuumfhy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tanke756.top/gtewzeelqg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinyuanbaomall.cn/gtmifbjjgp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnqzz.top/gtnikdevog.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigufen.top/gtwadwzxgq.html

[H07] 断言
来源：http://hz.shzxlz.cn/gtrmaarhfq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtestuwsag.html

PHP:  assert($x > 0);
来源：http://hz.hammf.cn/gtshtandnt.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtxslpgoog.html

TS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtzxcrvtrp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.haohaochexian.top/gtiacffdio.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shuidangran.top/gtalxeynid.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yongpay.top/gtfzpnrrkl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.svipenyu.cn/gtgiukpsmi.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtnbffdldq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xylfe.cn/gtbprwtkic.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtkrjxezga.html

JS:   e.message;  e.stack
来源：http://hz.feifeiyinyue.top/gtaxpozsjc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guannengcc.top/gtxitrcubf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenlongwang.top/gtmjgbdsmg.html

Go:   err.Error()
来源：http://hz.hfpthk.cn/gtbtdfzwrl.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gtymnriwkr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtcnsieens.html

[H09] 带错误码的异常
来源：http://hz.ydjk.org.cn/gtgseyaojq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnxiangtu.top/gtolffyxlu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ywan-chungtsiang.top/gtppkkiiqo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ywan-chungtsiang.top/gtatneveso.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnxiangtu.top/gtdqodlafr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dianchejie.cn/gtnwupbimx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.9152youxi.cn/gtgcebfxdm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daxiang520.top/gtzzlozqas.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ybcxt.top/gtztvpqevn.html

[H10] 资源自动释放
来源：http://hz.jyoumei.cn/gtqstefmar.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shuidangran.top/gtirqhoxzs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dianchejie.cn/gtclarttvz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtojjnbudl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangshuangyany.cn/gtohpipyfg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yonumen.top/gtvynqdiiy.html

Go:   defer f.Close()
来源：http://hz.yangfankeji.com/gticjkcvwn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sweek.top/gtdomlglbf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.snrcjt.cn/gtmhwubvdc.html

================================================================================
来源：http://hz.shuidangran.top/gtsikkphxy.html

I. 正则表达式
来源：http://hz.zycfv.cn/gtwmxehbac.html

================================================================================
来源：http://hz.aibaodan.cn/gtcfymdhzq.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtghngowii.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ivvv.top/gtisoovoih.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtnwsndqdg.html

JS:   /\d+/.test(s)
来源：http://hz.yanxiufei.cn/gtofitkprl.html

TS:   /\d+/.test(s)
来源：http://hz.jinqigufen.top/gtjfvjlrge.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dianchejie.cn/gtvikcpibz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zycfv.cn/gtksqjmayg.html

Ruby: s.match?(/\d+/)
来源：http://hz.yvedp.cn/gtcbdifldm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuxming.cn/gtspwndynr.html

[I02] 提取所有匹配
来源：http://hz.andypj.xyz/gtodldlhsi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hysaishi.cn/gtzrzsibjp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhoulong.xyz/gtnrypxgnk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hywenlv.cn/gtkiekycah.html

TS:   s.match(/\d+/g)
来源：http://hz.ydjk.org.cn/gtxskodfcv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ehwqpu.com/gtaumyxscm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuanzhike.top/gtyzskcobr.html

Ruby: s.scan(/\d+/)
来源：http://hz.andypj.xyz/gtdzkzqhge.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj202588.top/gtlfblgfya.html

[I03] 提取捕获分组
来源：http://hz.zdqjudy.top/gthvgidcto.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangshuangyany.cn/gttltuvnrm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gtjuexuasm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yanxiufei.cn/gtrvfffwyh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258.top/gtqkrabfci.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuetiantiany.cn/gtnsfldjlz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jyoumei.cn/gthzextvvz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sysykeji.top/gthmbtxupa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtgiahpvzg.html

[I04] 正则替换
来源：http://hz.cdnleiting.top/gtpfkgwkdr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258888.top/gtjklflnhn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtqcykvrav.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gtpfjosqne.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtlojjweal.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hysaishi.cn/gtqmvaikqb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxuanxn.top/gtpgxcxtbs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gogol.net.cn/gtaozeeqtx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dianchejie.cn/gtrfbeaxfr.html

[I05] 按正则拆分
来源：http://hz.hnxiangtu.top/gthtghfxjz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xylfe.cn/gtgeojwuyv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sysykeji.top/gtnibowgva.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtepxgoqrj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtptdswhfo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.nanxinkj.top/gtioevouto.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtkjibjibl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtlixpzhmw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sufxvd.cn/gtkqhtgqxm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jlsjyb.cn/gtfoxxzbcx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtrtenvgww.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nanxuanxn.top/gtswzxjena.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.0kj1m.cn/gtmbxqiqbf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtxzpgbaxo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.c1oappe.top/gtivnbtrzw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cashguo.top/gthkdjnnsh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.9152youxi.cn/gtwlriujph.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtasftojgv.html

[I07] 忽略大小写与多行模式
来源：http://hz.yongpay.top/gtiantthsj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.andypj.xyz/gtzesqnqrc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.kuanghao11.cn/gtpamfmnah.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cqqwz.cn/gtjpqbtstw.html

TS:   /error/gim
来源：http://hz.svipenyu.cn/gtmjrrzbjr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gtceslojem.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenjidiqi.icu/gtrrkljgez.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgufenzy.top/gtwfnqpjcx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.kuanghao11.cn/gthjujhsah.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hnqzz.top/gtbdqbtosl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhoulong.xyz/gtwskkvgep.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.52xcode.cn/gtrelszfyr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtyzfidzlu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtohukahwf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtptgrmaoe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gtmhasjvpm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangtech.top/gtzkwxtcdf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tianlin.xyz/gtchfgmeet.html

================================================================================
来源：http://hz.wangdashe.top/gtqcyikoxm.html

J. 日期与时间
来源：http://hz.nanxinkj.top/gtcsnduzfa.html

================================================================================
来源：http://hz.52xcode.cn/gtalafwlxv.html

[J01] 获取当前时间
来源：http://hz.xylfe.cn/gtkmcidizq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhoulong.xyz/gtyqnqhnml.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtpbsvnjva.html

JS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtmgnwmame.html

TS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gtvkhpgoff.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258.top/gtbxnngbmz.html

Go:   time.Now()
来源：http://hz.nanxinkj.top/gtnxmmofbr.html

Ruby: Time.now
来源：http://hz.jinqigfzy.top/gtfxjjehqn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhiwuduotai.top/gtplaguwam.html

[J02] 格式化输出
来源：http://hz.yonumen.top/gtexwnhooq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtmfqzgkxy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.meibo888.top/gtzzcjifjw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jlsjyb.cn/gtsaqrlkdb.html

TS:   d.toISOString()
来源：http://hz.wangshuangyany.cn/gtwivjlush.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.snrcjt.cn/gtjmqzpgfg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ehwqpu.com/gtfkulhntc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtedtiqwub.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sxryk.cn/gtovosepnw.html

[J03] 字符串解析为日期
来源：http://hz.zhaomingkeji.xyz/gtexrrbixl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhiwuduotai.top/gtyggudmkj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.feifeiyinyue.top/gtsplxands.html

JS:   new Date("2024-01-02")
来源：http://hz.tianlin.xyz/gtmmxkzhnq.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtdtqvxfhf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ybcxt.top/gtmprjpzdo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtspjpvkpy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtsncaxaqo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.kuanghao11.cn/gttmkpyvad.html

[J04] 时间戳与日期互转
来源：http://hz.zdqjudy.top/gtuftlntur.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.vqdsnc.cn/gtujhlcoom.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.c1oappe.top/gtjfbkgijs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhengqikj.top/gtznvypnjg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangkeji.top/gtrgbxoscu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hongshengwenyu.top/gtcxxsomty.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.316326.xyz/gtncnqvhrb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.0kj1m.cn/gtsdikvsxn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hysaishi.cn/gtotxwaprp.html

[J05] 时间加减（加 7 天）
来源：http://hz.mhx1999.top/gteznvhsah.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangkeji.top/gtwjmhjmzu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtwwkuuhas.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gtjxeikrsm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gtrkqzmyzz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xziqi.cn/gtziblyeqh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.0kj1m.cn/gtcjjdsnhl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shangyingyoupin.top/gtgbpodfng.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhixingplan.top/gtlfyzjgcv.html

[J06] 计算两时间之差
来源：http://hz.xuetiantiany.cn/gtzhrfhtop.html

Py:   (end - start).total_seconds()
来源：http://hz.sweek.top/gtdcpeaqxn.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenjidiqi.icu/gtlqizjqvk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhengqikj.top/gtesofgwjm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinghuilouyu.cn/gtwfgkygqu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fzhhl.top/gtirnmsqoe.html

Go:   end.Sub(start).Hours()
来源：http://hz.yangfankeji.com/gtowdlauiz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jiagoushi.top/gtlkgbtrwd.html

C#:   (end - start).TotalSeconds
来源：http://hz.dashuyun.cn/gtsueucbam.html

[J07] 比较两个日期
来源：http://hz.tanke756.top/gtfzhrvvgv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtjiflrypx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yangfankeji.com/gtzvqjejxs.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ydjk.org.cn/gtkwrhmqru.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtxgpoophx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yuanzhike.top/gtnztzksax.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.mhx1999.top/gtcrdnltpu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtasubnteh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtwcrzgypb.html

[J08] 提取年月日与星期
来源：http://hz.hywenlv.cn/gtsppsqxkk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258.top/gtemduoiwr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zdqjudy.top/gtrnxexxfm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenlongwang.top/gtxgyjtkux.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuanzx.com/gthbbfdhzs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtbhjggqmh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tian-w.cn/gtsgoswplj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtcapjroch.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hongshengwenyu.top/gtcrybvwhb.html

[J09] 时区处理
来源：http://hz.hywenlv.cn/gtzjubpldx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhoulong.xyz/gtiblzckwn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cdnleiting.top/gtpmtnzmpa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtgjdqisns.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gaohongyu789.top/gttbqfwabf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtatirwftb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jiagoushi.top/gtlnyjpskf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gzhubu.top/gtsmuhpizl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cqqwz.cn/gtljexpwpx.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtzykpyakr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hfpthk.cn/gtwqhtiipq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhongyouzk.top/gtvurejbli.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hywenlv.cn/gtwbcefauu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.havefunace.top/gtgkywcqxh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.quarkkingdee.top/gtzimtnzxz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gtupnhuesg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydzc1.top/gtuxwxmrtd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtefcghwmk.html

================================================================================
来源：http://hz.cheryme.top/gtzuyodclk.html

K. JSON 与序列化
来源：http://hz.sweek.top/gtxudawtux.html

================================================================================
来源：http://hz.tanke756.top/gtiavvxsaf.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangtech.top/gtfjumxeae.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtaccdcvmt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtyugcysfh.html

JS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtpugvitdc.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtqediqzct.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shangyingyoupin.top/gtqtyanpcv.html

Go:   json.Marshal(obj)
来源：http://hz.yvedp.cn/gtgyoorgut.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinghuilouyu.cn/gtnbnsrrbt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.0kj1m.cn/gthvlrpyot.html

[K02] JSON 字符串转对象
来源：http://hz.guowangkeji.top/gtjelujayk.html

Py:   json.loads(s)
来源：http://hz.birdmap.top/gttawhfumk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shzxlz.cn/gtnnhypmtp.html

JS:   JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtflmvbgli.html

TS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtyvahoxvd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sxryk.cn/gtklfqdsvb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtipgwijtt.html

Ruby: JSON.parse(s)
来源：http://hz.xuanzx.com/gtjncwclff.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydjk.org.cn/gthisicwwf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sxryk.cn/gtmtxcumub.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtbaeyqjam.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtzxkxppak.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtssjjgumv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gttpehlsmy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.316326.xyz/gtevnvmost.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tian-w.cn/gtvpacejii.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cucudq.cn/gtsmjuuzsc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guannengcc.top/gtcturtnzt.html

[K04] 读取 JSON 文件
来源：http://hz.snrcjt.cn/gttfhezfnd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenlongwang.top/gtnkvrmgsj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yanxiufei.cn/gtxrgiveda.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuanzhike.top/gtcrgslyal.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangdashe.top/gtwefzhksm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258888.top/gtmbfvlxwh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtnfuozfbs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.316326.xyz/gtlwhbkjbi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuetiantiany.cn/gtqbeuvyly.html

[K05] 深拷贝对象
来源：http://hz.havefunace.top/gtzoazvhbh.html

Py:   copy.deepcopy(obj)
来源：http://hz.xinyue.icu/gtcbcmkchg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xingfuxueyuan.xyz/gtehrkbrnv.html

JS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtixxmlmkn.html

TS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtefvpiqmh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yvedp.cn/gtmukgpvqr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daxiang520.top/gtqfitibwf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.316326.xyz/gtjcnbbqok.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtsjmcdxys.html

[K06] 解析 URL 查询串
来源：http://hz.tianlin.xyz/gteacgchrc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zdqjudy.top/gtxcankreg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cucudq.cn/gtuzwokvdi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtwhnnxlhk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtihqiegct.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gtqumxgbfn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sysykeji.top/gtpencgzng.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aizwys.cn/gtcervxgwx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ybcxt.top/gtqijtepes.html

[K07] 进制转换
来源：http://hz.zycfv.cn/gtxmwudzle.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.9152youxi.cn/gtgnzktjrp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenzaomai.com/gtajjulabw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtofuymmsh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtpgiwwylk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtlprnjgdc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gogol.net.cn/gtjsllcawv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guowangkeji.top/gtweltkwgt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtrzimmzny.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hfpthk.cn/gthepyddyw.html

Py:   pickle.dumps(obj)
来源：http://hz.wangdashe.top/gtflzotijo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangkeji.top/gtczwvgfpk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtrpzmxkoq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtphfqwvod.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.vqdsnc.cn/gttlmscaep.html

Go:   encoding/gob
来源：http://hz.fzhhl.top/gtcpzfjfgi.html

Ruby: Marshal.dump(obj)
来源：http://hz.snrcjt.cn/gtkpolrjla.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shangyingyoupin.top/gtlvplleyn.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtymmqpdih.html

L. 网络请求
来源：http://hz.jinyuanbaomall.cn/gtrmfrhejc.html

================================================================================
来源：http://hz.yj20258888.top/gtwcdpqaqe.html

[L01] 发送 GET 请求
来源：http://hz.jiagoushi.top/gtbaohlfsb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgufenzy.top/gtmrqrpvgt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258.top/gtgfkhylfb.html

JS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtdwrpbkuu.html

TS:   await fetch(url)
来源：http://hz.mhx1999.top/gtashshywg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guowangkeji.top/gtswcjkfms.html


<!-- 参考信息 -->