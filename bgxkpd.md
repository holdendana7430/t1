代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pycfn.com/gtrtazrcxa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xylfe.cn/gtwvnisxcq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj202588.top/gtaufzejxt.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtkujrtxva.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gtcfpkpcch.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ybcxt.top/gtynokhaic.html

PHP:  assert($x > 0);
来源：http://hz.ydzc1.top/gtmolzwquv.html

JS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gtkmxbhses.html

TS:   console.assert(x > 0);
来源：http://hz.pycfn.com/gtvoqwdnhz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.redwolf501.top/gtbjfcpait.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnxiangtu.top/gtrmfopbyh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xziqi.cn/gtlpumzzjo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aibaodan.cn/gtgsycbyyl.html

[H08] 获取错误信息与堆栈
来源：http://hz.haohaochexian.top/gtrwjtmpsn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnxiangtu.top/gtqcbwtybv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shuidangran.top/gtiuvbaeki.html

JS:   e.message;  e.stack
来源：http://hz.zhongyouzk.top/gtkeigqfsi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.redwolf501.top/gtqtsbzcpq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.9152youxi.cn/gtjalgyfga.html

Go:   err.Error()
来源：http://hz.ydzc1.top/gtguankycb.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtptqdtlmh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shangyingyoupin.top/gtinrfztuc.html

[H09] 带错误码的异常
来源：http://hz.tianlin.xyz/gtnhdgpvqi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.feifeiyinyue.top/gtrkyckbnu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fengsongda.top/gtbonfkwpt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj202588.top/gtkukprchq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydjk.org.cn/gtkgzuxddw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cucudq.cn/gtuhiplnok.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yongpay.top/gtopsznojs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daria6918.cn/gtclyjwyzr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gzhubu.top/gtgaoyolln.html

[H10] 资源自动释放
来源：http://hz.zhoulong.xyz/gtmktinmiz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gtlsvelkvq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daxiang520.top/gtngevjwzb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gtwkruneen.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cqqwz.cn/gtsdclpmnc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ehwqpu.com/gtmufhvrva.html

Go:   defer f.Close()
来源：http://hz.zhongyouzk.top/gtsmosnlso.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtcplniytf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj20258888.top/gthkvwvbro.html

================================================================================
来源：http://hz.yueranfly.top/gtesuzznpb.html

I. 正则表达式
来源：http://hz.zycfv.cn/gtyvlaqcpl.html

================================================================================
来源：http://hz.shzxlz.cn/gtnpydbfgq.html

[I01] 判断是否匹配
来源：http://hz.fzhhl.top/gtvpaislbb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pycfn.com/gttsybpsat.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuanzhike.top/gtwppehnsx.html

JS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gtrciwuhew.html

TS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtjlpjdrsb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.vqdsnc.cn/gtldnyputd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fengsongda.top/gteavtoela.html

Ruby: s.match?(/\d+/)
来源：http://hz.guowangkeji.top/gtqjzywopk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gtqeryswmu.html

[I02] 提取所有匹配
来源：http://hz.guannengcc.top/gtkwamelgl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zycfv.cn/gtoqytvveh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.kuanghao11.cn/gtblikvspq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenzaomai.com/gtobfhjfsz.html

TS:   s.match(/\d+/g)
来源：http://hz.zdqjudy.top/gtotxortnq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenlongwang.top/gtikmgtpvt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.pengpengdd.cyou/gtmdxjninj.html

Ruby: s.scan(/\d+/)
来源：http://hz.ivvv.top/gtiorkuvyt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.pengpengdd.cyou/gtbrqdsqko.html

[I03] 提取捕获分组
来源：http://hz.redwolf501.top/gtimnknykh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.birdmap.top/gtyfvtnxxm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.havefunace.top/gtfkgwdedr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhixingplan.top/gteirenivw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gaohongyu789.top/gtuzyajpht.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuanzx.com/gtdgzaykir.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xuanzx.com/gtbugypitd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.birdmap.top/gtjwqexaro.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuanzx.com/gtogkuqkyr.html

[I04] 正则替换
来源：http://hz.shanyushiyangkeji.top/gteldcidew.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sysykeji.top/gtwdbehgha.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.kuanghao11.cn/gtemwpbuuv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtnlecsggh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtuevesvgc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gtuwluzmib.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.meibo888.top/gtdtjrndsy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenlongwang.top/gtmvnhozmh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daria6918.cn/gtgxltrulg.html

[I05] 按正则拆分
来源：http://hz.kuanghao11.cn/gtiwfkqfll.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuxming.cn/gtgyettksk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gaohongyu789.top/gthaelqrqp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtkvsqgyqx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtiiycejzw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangkeji.top/gtdxhdsypz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenzaomai.com/gtrldrdceh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtladodggl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aizwys.cn/gtofjgqtzg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nwbrower.top/gtajrqwwid.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gtckyegqgc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tianlin.xyz/gthswvvgod.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtxdmqycth.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtmgzuzkno.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.52xcode.cn/gtlxoluixn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yuxming.cn/gtiinpaxoj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gthvxucfxv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtthxnzjeg.html

[I07] 忽略大小写与多行模式
来源：http://hz.havefunace.top/gtyclkkhap.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtqdwaqwew.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.316326.xyz/gtkkctqwyl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.c1oappe.top/gtwikejpuq.html

TS:   /error/gim
来源：http://hz.ywan-chungtsiang.top/gtzmrplswk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yvedp.cn/gtsmfvwugr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.havefunace.top/gtxulpchde.html

Ruby: s.scan(/error/i)
来源：http://hz.redwolf501.top/gtlbwmcezb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.feifeiyinyue.top/gtquakqgmh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtoynqwpey.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.mhx1999.top/gtbcjkxmvp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hammf.cn/gtpkqelgov.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ehwqpu.com/gtyzxiwirc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtbsmwzazd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zdqjudy.top/gthqbjajet.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jyoumei.cn/gtljqshfqi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigfzy.top/gttwlfsldd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtkyoiptan.html

================================================================================
来源：http://hz.sweek.top/gtvoietmpy.html

J. 日期与时间
来源：http://hz.cheryme.top/gtdgiwbduc.html

================================================================================
来源：http://hz.birdmap.top/gtqxxlgjeo.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtnzluxeag.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtnapmanxj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtqztyfmwq.html

JS:   new Date();  Date.now()
来源：http://hz.jqgufenzy.top/gtfwaojlqs.html

TS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gtahrbzdpx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.mhx1999.top/gtvgckqtju.html

Go:   time.Now()
来源：http://hz.sxryk.cn/gtatcvjlwk.html

Ruby: Time.now
来源：http://hz.52xcode.cn/gtvqgjiahu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hongshengwenyu.top/gtuuwdlzfz.html

[J02] 格式化输出
来源：http://hz.birdmap.top/gtohewqqng.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gtieyrhuma.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtgyiiyezg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cashguo.top/gtujgtqywf.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gtiewezmxv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aibaodan.cn/gteyjclkam.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnqzz.top/gtmsdmkhvr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtacvslnji.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.c1oappe.top/gtvsbsmksd.html

[J03] 字符串解析为日期
来源：http://hz.yangfankeji.com/gtbrpdeaug.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gtkdecrgzx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydjk.org.cn/gtjevnaamk.html

JS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtdiquiciy.html

TS:   new Date("2024-01-02")
来源：http://hz.fengsongda.top/gtxizqocox.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gtwelfleik.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.0kj1m.cn/gtmvpwpkql.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtunrggznm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.dashuyun.cn/gtfdyvamvg.html

[J04] 时间戳与日期互转
来源：http://hz.chenlongwang.top/gtnnrdopkw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenjidiqi.icu/gtoqeedcon.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgfzy.top/gtbpryasxw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aizwys.cn/gtfpntobsf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigfzy.top/gtwanpksvj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.iojbl.cn/gtthkxrpuk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fzhhl.top/gtkzmnivjo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pycfn.com/gtpinrcggw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.0kj1m.cn/gtlhbsgunc.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgufenzy.top/gtkhimyevk.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangkeji.top/gthuuxinjz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hammf.cn/gthbemjzii.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtlzqkgagu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtciertgpu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenlongwang.top/gtufyzetyn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.meibo888.top/gtkqzqxrkp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gttsiqukvv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.meibo888.top/gtdnbhllyl.html

[J06] 计算两时间之差
来源：http://hz.fengsongda.top/gtrkrpgofe.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangtech.top/gtzccodnco.html

PHP:  $end->diff($start)->days;
来源：http://hz.xinyue.icu/gtpswzyozf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zdqjudy.top/gtqkyhmfuv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yanxiufei.cn/gtdypyhbnr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tianlin.xyz/gtqnveqndl.html

Go:   end.Sub(start).Hours()
来源：http://hz.yanxiufei.cn/gtybplamgx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gotoacloud.top/gtxmnqdxmf.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuxming.cn/gteksltdig.html

[J07] 比较两个日期
来源：http://hz.daxiang520.top/gtkwkgeehp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtmicdwyhf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj202588.top/gtrzrhibma.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gtlgmrfctv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gtqggvuctr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.birdmap.top/gtfnshzyut.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhiwuduotai.top/gtcmujnqcc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtakszxdqw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtuwvogvfu.html

[J08] 提取年月日与星期
来源：http://hz.9152youxi.cn/gtbecycgko.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hysaishi.cn/gteilzefbt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fzhhl.top/gtjhbhzbkh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gtnjndpufe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinyuanbaomall.cn/gtwnpabrcb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hongshengwenyu.top/gtvjhselev.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtqeldvznj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daxiang520.top/gtznsivmxn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gogol.net.cn/gttdsonlyb.html

[J09] 时区处理
来源：http://hz.xziqi.cn/gtnfcqzimq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tian-w.cn/gtilecptlg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.mhx1999.top/gtvzzsncmo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtfqvtweni.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtqefxoyzg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtegadiozl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.mhx1999.top/gtgsbjtdvc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ivvv.top/gtkompnvvs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aizwys.cn/gtfhfqhecc.html

[J10] 取今天 / 本月第一天
来源：http://hz.yanxiufei.cn/gtcxlupjqe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gthpsipscl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhaomingkeji.xyz/gtsfruksod.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sweek.top/gtrrmjphwb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxinkj.top/gtgerqlick.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhiwuduotai.top/gtcpuqixjn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ivvv.top/gtwdfxcxsh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hywenlv.cn/gtrqtgebcg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydzc1.top/gtufmcnqkj.html

================================================================================
来源：http://hz.nwbrower.top/gtwfbncqei.html

K. JSON 与序列化
来源：http://hz.shanyushiyangtech.top/gtavqnlxkz.html

================================================================================
来源：http://hz.tian-w.cn/gtswrboxvd.html

[K01] 对象转 JSON 字符串
来源：http://hz.fengsongda.top/gterptigek.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtzadxaduq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.havefunace.top/gtqluayxdj.html

JS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtiijlrbcp.html

TS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtqszfvxwd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sxryk.cn/gtxvpkaohk.html

Go:   json.Marshal(obj)
来源：http://hz.hfpthk.cn/gtgmdjshbk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.smart0.xyz/gtxemlksxj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.snrcjt.cn/gtuplnnsla.html

[K02] JSON 字符串转对象
来源：http://hz.yonumen.top/gtrpcpkwxa.html

Py:   json.loads(s)
来源：http://hz.316326.xyz/gtwjsbsfdm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ywan-chungtsiang.top/gtgmiukrbq.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gttznomajs.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtrlgkwqgj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sxryk.cn/gtbfnqqszt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtlbwvahdu.html

Ruby: JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtegnteedy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shangyingyoupin.top/gtiydhkxee.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenjidiqi.icu/gtlatwhxhc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xinyue.icu/gtdffcvdwf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gthzcbfolr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtttauuiyd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtflowynsf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sufxvd.cn/gtklnrfkil.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shuidangran.top/gteqolwtrm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tianlin.xyz/gtchnptgen.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fengsongda.top/gtzxvnekxj.html

[K04] 读取 JSON 文件
来源：http://hz.sysykeji.top/gtykpdazga.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.9152youxi.cn/gtfwkzplax.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigfzy.top/gtxfdipsaz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gturfstjbb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtnrckpzxa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtvshcdyrt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinyuanbaomall.cn/gthwhqikzt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yangfankeji.com/gtyvnwsgom.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cqqwz.cn/gtqsumofnx.html

[K05] 深拷贝对象
来源：http://hz.meibo888.top/gtytorukkc.html

Py:   copy.deepcopy(obj)
来源：http://hz.kuanghao11.cn/gtkxgulhze.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gtezcktfkc.html

JS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtwvvxgkru.html

TS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtqfepplak.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.meibo888.top/gtabluzhwi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.kuanghao11.cn/gtwncyftow.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258.top/gttbgwrmde.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ehwqpu.com/gtbtjlgkfw.html

[K06] 解析 URL 查询串
来源：http://hz.wangshuangyany.cn/gtmeixyybu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sufxvd.cn/gtqroxzxxk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shuidangran.top/gtxsfacloo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtvoidpfyo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtjjuusodg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gtznfwyyex.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtsunepsld.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dianchejie.cn/gtbuetopna.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nwbrower.top/gtoyycrrsj.html

[K07] 进制转换
来源：http://hz.chenjidiqi.icu/gtvtzaptfs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.52xcode.cn/gttkexjbpn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtvusynobz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtqlwhzliw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gturfgorzv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtgfzdmdic.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtqltvnkpy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.c1oappe.top/gtdmdrytuf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gaohongyu789.top/gtxxxyddja.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258.top/gtfyoibxil.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258888.top/gtbnefjxjj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.meibo888.top/gtjoqqgokh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtydpgteuj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gthltwdhnk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenjidiqi.icu/gtmaqqvkzv.html

Go:   encoding/gob
来源：http://hz.guowangkeji.top/gttgvmztds.html

Ruby: Marshal.dump(obj)
来源：http://hz.316326.xyz/gtijrcsfsb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtncjckjxs.html

================================================================================
来源：http://hz.xziqi.cn/gtwhgmhxpa.html

L. 网络请求
来源：http://hz.ivvv.top/gtzxfrgknb.html

================================================================================
来源：http://hz.hammf.cn/gtjrdqairl.html

[L01] 发送 GET 请求
来源：http://hz.shzxlz.cn/gtmdxgtzed.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.52xcode.cn/gtwiwfdaxz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.havefunace.top/gtwceefgot.html

JS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtwdpcxgst.html

TS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtbzkevkkt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xylfe.cn/gtygwszvlr.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtwggzhdkz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhoulong.xyz/gtwvhfnmfe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.0kj1m.cn/gtjnlhvkmf.html

[L02] 发送 POST JSON
来源：http://hz.jqgufenzy.top/gtwwngfrdw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gtlvbzssln.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtepzlouep.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gthulmovbi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtcojyncrn.html


<!-- 参考信息 -->