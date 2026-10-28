代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxuanxn.top/gtkjxweevt.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhijiandao.cn/gtdxigxkdt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigfzy.top/gtgxbwzwor.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sxryk.cn/gtyqclzmaj.html

Py:   value = d.get("k") or default
来源：http://hz.haohaochexian.top/gtgrfhohqd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.vqdsnc.cn/gtcrojaqpb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtqvstinap.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gotoacloud.top/gtwwucnany.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhijiandao.cn/gtjuzshghg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ybcxt.top/gtqfhlsuyf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ydjk.org.cn/gtsivbwkfx.html

C#:   obj?.A?.B ?? default
来源：http://hz.ydjk.org.cn/gtseqslkui.html

[H07] 断言
来源：http://hz.smart0.xyz/gtkskwlaip.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hfpthk.cn/gtwgtocmqv.html

PHP:  assert($x > 0);
来源：http://hz.wangshuangyany.cn/gtduwmmfnv.html

JS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtnxthhdik.html

TS:   console.assert(x > 0);
来源：http://hz.yonumen.top/gtkfmdkvkl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shzxlz.cn/gtcckivprc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenjidiqi.icu/gtrxihlpqs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gtzmsdhvmd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xuanzx.com/gtycasgpad.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258888.top/gtwwehqpyx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgufenzy.top/gtcpuetzth.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cqqwz.cn/gtxsdddhis.html

JS:   e.message;  e.stack
来源：http://hz.xziqi.cn/gtoxphirsl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sweek.top/gttargcagb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenjidiqi.icu/gtbzxenpgk.html

Go:   err.Error()
来源：http://hz.jinqigfzy.top/gtjgacklxa.html

Ruby: e.message;  e.backtrace
来源：http://hz.shuidangran.top/gtxfljkdjy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.316326.xyz/gtkfzansjp.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtqtwshimw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sweek.top/gtexosuvki.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cqqwz.cn/gtrsadamxf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xylfe.cn/gtyqvodaro.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ehwqpu.com/gtgoxrkcks.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xziqi.cn/gtsofdxxbj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.andypj.xyz/gtleojyeme.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fengsongda.top/gtdniptqfm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.guowangkeji.top/gtihhgwwxx.html

[H10] 资源自动释放
来源：http://hz.xuetiantiany.cn/gtawhlfufs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenzaomai.com/gtiktdxgcx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gogol.net.cn/gtkrefnnwb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtprojcqpt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtrsimneku.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydjk.org.cn/gtfclnglet.html

Go:   defer f.Close()
来源：http://hz.xuanzx.com/gtizxxtuik.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxinkj.top/gtrcdprbgb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yanxiufei.cn/gtgycjcvlm.html

================================================================================
来源：http://hz.chenjidiqi.icu/gttcdrffoh.html

I. 正则表达式
来源：http://hz.dianchejie.cn/gtvryptbzj.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gteynathnc.html

[I01] 判断是否匹配
来源：http://hz.yj202588.top/gthyjhcxwu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yanxiufei.cn/gtjrdydgjl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cqqwz.cn/gtlrzlrvxc.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtjvgtvtes.html

TS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtqiqenhum.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.havefunace.top/gthsgoozow.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shangyingyoupin.top/gtcteawclk.html

Ruby: s.match?(/\d+/)
来源：http://hz.jianghu66.top/gtdawxvbxb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydzc1.top/gtwsntjooe.html

[I02] 提取所有匹配
来源：http://hz.ydjk.org.cn/gtjphovovo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shuidangran.top/gteywkcdjf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gtrysujsky.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtwyaaaafd.html

TS:   s.match(/\d+/g)
来源：http://hz.jlsjyb.cn/gtzcqzqqhl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.redwolf501.top/gtljehcolv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.havefunace.top/gtthsvhplv.html

Ruby: s.scan(/\d+/)
来源：http://hz.haohaochexian.top/gtpaxtvazg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gtjrwypecl.html

[I03] 提取捕获分组
来源：http://hz.ybcxt.top/gthuraluaz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jiagoushi.top/gtpktttbdy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj202588.top/gtkwsxehzp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ivvv.top/gtscoxhxfn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gteergwuah.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sysykeji.top/gtvjvkvtev.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.haohaochexian.top/gtiqiqaxtl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sweek.top/gtcirhlvsd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenjidiqi.icu/gtpgtdduiq.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gthksnqmbw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.snrcjt.cn/gtvurmybuv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.kuanghao11.cn/gtfyazkmns.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtiekldekj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtqzpwwzpx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yuxming.cn/gtbtzjachl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxinkj.top/gtkptlaazc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hywenlv.cn/gtbvprjqaa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydzc1.top/gteqmcddbe.html

[I05] 按正则拆分
来源：http://hz.yj202588.top/gthwqyzzay.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhengqikj.top/gtnpgsasvu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.316326.xyz/gtatwgzfte.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtjrwvcrnb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtrmnhcwnj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.bjfxy.top/gtlcgadpdr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtgapwbviq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtavbqbqjr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shanyushiyangtech.top/gtxqzsovjb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gzhubu.top/gtqoaiwvwx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtybvmamta.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jqgufenzy.top/gtjieanwcs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtuoxkpsje.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtusfklyhv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ppjwa.cn/gtbaclkbfs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xziqi.cn/gtjovhasgr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xingfuxueyuan.xyz/gthwmkmtyx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtuhjgnpjc.html

[I07] 忽略大小写与多行模式
来源：http://hz.sysykeji.top/gtlacwzflr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.andypj.xyz/gtkgvihacn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gtdsljankn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.birdmap.top/gtvusnoeno.html

TS:   /error/gim
来源：http://hz.nwbrower.top/gtcxgdqwot.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gthpkrysle.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gzhubu.top/gtqzcfaofq.html

Ruby: s.scan(/error/i)
来源：http://hz.hnqzz.top/gtzinitbke.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cdnleiting.top/gtyenozmfu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtjachxiss.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pengpengdd.cyou/gtsbcuimvg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.9152youxi.cn/gthpzixnhc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtmtnipccd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gtkxfjjpvc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydzc1.top/gtqhlhevyg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cheryme.top/gtlawergdf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.0kj1m.cn/gtcnaolbkw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.havefunace.top/gtveiybjdg.html

================================================================================
来源：http://hz.bjfxy.top/gtmfjlqujm.html

J. 日期与时间
来源：http://hz.zhengqikj.top/gtuuwlyooq.html

================================================================================
来源：http://hz.hywenlv.cn/gtyaxpubny.html

[J01] 获取当前时间
来源：http://hz.yangfankeji.com/gtuzfcbugv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ivvv.top/gtpnwumjbv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtukmapvum.html

JS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtiqihucyr.html

TS:   new Date();  Date.now()
来源：http://hz.jqgufenzy.top/gtbvictbda.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.meibo888.top/gtjeazsats.html

Go:   time.Now()
来源：http://hz.andypj.xyz/gtomjkmcmj.html

Ruby: Time.now
来源：http://hz.andypj.xyz/gtosmgvznm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yueranfly.top/gtalhghlfw.html

[J02] 格式化输出
来源：http://hz.feifeiyinyue.top/gttajopnpa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gtjbqhsghr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sysykeji.top/gtzyqaylzc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258888.top/gttnjprxkt.html

TS:   d.toISOString()
来源：http://hz.jianghu66.top/gtsbtwoova.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.kuanghao11.cn/gtxasyynmb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhengqikj.top/gtvqxxkqqz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtbalibizj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sweek.top/gtswzutuve.html

[J03] 字符串解析为日期
来源：http://hz.xinyue.icu/gtykcpzgpx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tanke756.top/gtxdebivnq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.iojbl.cn/gtiepxkyhj.html

JS:   new Date("2024-01-02")
来源：http://hz.mhx1999.top/gtfjhqaqwq.html

TS:   new Date("2024-01-02")
来源：http://hz.shzxlz.cn/gtbvrjlfzp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.mhx1999.top/gthlspaoem.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigufen.top/gtktjnrzhj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtjjmrbber.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.daxiang520.top/gtfiiedgpk.html

[J04] 时间戳与日期互转
来源：http://hz.gaohongyu789.top/gtsvhjfhxn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtspibpend.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fzhhl.top/gtuhidvzwb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xingfuxueyuan.xyz/gtdnbibuzs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gtaubnwlrq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhiwuduotai.top/gtoqllwcso.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgfzy.top/gtvufdbkaz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ybcxt.top/gtekbefxoy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tian-w.cn/gtxircwkhu.html

[J05] 时间加减（加 7 天）
来源：http://hz.yuanzhike.top/gtlyruhjgm.html

Py:   now + timedelta(days=7)
来源：http://hz.jiagoushi.top/gtvrezdoip.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.haohaochexian.top/gtdjhpyiij.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258.top/gttrjeypii.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtclxtzcgl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhixingplan.top/gtkfnvhuqt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yangfankeji.com/gtjxcdnbso.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pengpengdd.cyou/gtrdpxdsom.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.bjfxy.top/gtqjcynsen.html

[J06] 计算两时间之差
来源：http://hz.yangfankeji.com/gtclzcxlmq.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtjsxbmagy.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtmfsxchxf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtylzcfvoc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gtitepwxhc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gtjxjrbnpd.html

Go:   end.Sub(start).Hours()
来源：http://hz.dashuyun.cn/gtyniiopoa.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tianlin.xyz/gtyjhxmzpq.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtqsgdmzme.html

[J07] 比较两个日期
来源：http://hz.tian-w.cn/gtjwpgcshw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtwjrxritw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenlongwang.top/gtywcjexyt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gtvaowtwlw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtarpqrgqz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenlongwang.top/gtsitqitpd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.smart0.xyz/gtykfxvntc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtzlnytttu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtnurtagcm.html

[J08] 提取年月日与星期
来源：http://hz.andypj.xyz/gtfahasvtu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gogol.net.cn/gtdnkmdnbe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sxryk.cn/gtnmxwfktm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.0kj1m.cn/gtnformelt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tanke756.top/gteveztusw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.316326.xyz/gtjiidqjru.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gtttxhlxzj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gtlgeulxiu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ybcxt.top/gtanfyqebg.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtezhkgvii.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhengqikj.top/gtyugcyapb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.daria6918.cn/gtzzfhmkva.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gtjaieihdu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gtkjupfqqu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gtipknstjd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.c1oappe.top/gtmatjqrmo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuanzhike.top/gthustyfrm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydzc1.top/gtcgksxasf.html

[J10] 取今天 / 本月第一天
来源：http://hz.hfpthk.cn/gtvsywpsmp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yangfankeji.com/gtwbjsbshj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnxiangtu.top/gtigjfcfme.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.daxiang520.top/gtnazvxjqe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jqgfzy.top/gtemimhoxj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gtuuqnmlvx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dashuyun.cn/gtfjjnojol.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.feifeiyinyue.top/gtsghpzkhg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydjk.org.cn/gtmvqmxhli.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtftsytvbm.html

K. JSON 与序列化
来源：http://hz.zhengqikj.top/gtxkitvktz.html

================================================================================
来源：http://hz.jqgfzy.top/gtorjxdwci.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhoulong.xyz/gtfxqhsxsg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtjfedfpml.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtgyoisbgm.html

JS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtjmiojjcp.html

TS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtbugdwocb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yonumen.top/gtyvtbwyzo.html

Go:   json.Marshal(obj)
来源：http://hz.feifeiyinyue.top/gtmriwfbwg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhaomingkeji.xyz/gthhmtyeiv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.birdmap.top/gtshbybnzb.html

[K02] JSON 字符串转对象
来源：http://hz.guowangkeji.top/gtlwbpkzhj.html

Py:   json.loads(s)
来源：http://hz.smart0.xyz/gtddemlyir.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daxiang520.top/gtjkbeegla.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtijzlnqik.html

TS:   JSON.parse(s)
来源：http://hz.redwolf501.top/gtxrvdmnyq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.meibo888.top/gtwmlkrymc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gttqaucnpb.html

Ruby: JSON.parse(s)
来源：http://hz.9152youxi.cn/gtapfzples.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhixingplan.top/gtnklcaive.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fzhhl.top/gtqthgqlri.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtzntkmyhq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtrrffyetr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtlosfwuvb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gttkyxkygw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sufxvd.cn/gtguigdjpv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhengqikj.top/gtftjdsxul.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ywan-chungtsiang.top/gtabeocwbj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhixingplan.top/gtecqziqqj.html

[K04] 读取 JSON 文件
来源：http://hz.ydjk.org.cn/gttfeqenot.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jiagoushi.top/gtcpevlgss.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jianghu66.top/gthttfijcc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gtmdhnpswz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtukotaery.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gthvemuebe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gttknwemxc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.316326.xyz/gtyhkvwucf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gotoacloud.top/gtbgwxwjcg.html

[K05] 深拷贝对象
来源：http://hz.hammf.cn/gtuzvemhhe.html

Py:   copy.deepcopy(obj)
来源：http://hz.yvedp.cn/gtrhsalnig.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gtzbtgvbyt.html

JS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtaeotyklt.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtbxlkgbof.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.iojbl.cn/gtjeelbypc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhengqikj.top/gtlerhvefw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sysykeji.top/gtyulaqfkt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.svipenyu.cn/gtgvcbojue.html

[K06] 解析 URL 查询串
来源：http://hz.zhixingplan.top/gtjuyxbcul.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.birdmap.top/gtojlobybl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigfzy.top/gtxlyuwjbo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtizhbjzxb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtbijlwpep.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhongyouzk.top/gthzsfeske.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhengqikj.top/gtdbjgovli.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.snrcjt.cn/gttiejhcsq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtqiqrbxbv.html

[K07] 进制转换
来源：http://hz.daria6918.cn/gtaeywzynp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.guowangkeji.top/gtsiarznwu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cdnleiting.top/gtnunuwogg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtatwponwi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtcbnaieyp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtietfcikg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hywenlv.cn/gtzkdtnqxd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.haohaochexian.top/gtfvzelcnw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gttlsijjmp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangshuangyany.cn/gtdzktatqb.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258888.top/gtokmuryxq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ydzc1.top/gtnhdpcoya.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtqqdlqbkw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtfvfjuenf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jianghu66.top/gtpbwsyyqm.html

Go:   encoding/gob
来源：http://hz.jyoumei.cn/gtqmrgntxl.html

Ruby: Marshal.dump(obj)
来源：http://hz.vqdsnc.cn/gtaddzpquo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shzxlz.cn/gtneptbpwj.html

================================================================================
来源：http://hz.c1oappe.top/gtcwuhbwnu.html

L. 网络请求
来源：http://hz.yuanzhike.top/gtbzhwkusg.html

================================================================================
来源：http://hz.nwbrower.top/gtrwjrzugm.html

[L01] 发送 GET 请求
来源：http://hz.sweek.top/gtqzwktxyi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aibaodan.cn/gtzfckvyzx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258888.top/gtaegpjwgq.html

JS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtgqgxzncu.html

TS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtpcsrnuqt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.quarkkingdee.top/gtkuiadbvh.html


<!-- 参考信息 -->