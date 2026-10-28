代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yuanzhike.top/gtdormtfrx.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtcuijdzgv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sweek.top/gtitsrsspu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuetiantiany.cn/gtcbzqoqfw.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258888.top/gtfombisgl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtiabocuco.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cashguo.top/gttrwrqpei.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangshuangyany.cn/gtkxpxbgvg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nanxuanxn.top/gtlzsekhmp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxuanxn.top/gtoixpvsgj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuanzhike.top/gtofbnmwys.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtrdjdoxfz.html

[H07] 断言
来源：http://hz.wangdashe.top/gtwqptcyqt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dashuyun.cn/gtbtfxmpds.html

PHP:  assert($x > 0);
来源：http://hz.guannengcc.top/gtzohvkzrk.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gttuhlyooq.html

TS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtdlptship.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fengsongda.top/gtjekzhgbg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xylfe.cn/gtppxtdwyf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shangyingyoupin.top/gthucuifup.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtymjnoemj.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenlongwang.top/gtjsixngjx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nanxuanxn.top/gtrrysdkzg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhixingplan.top/gtbvlwqrlg.html

JS:   e.message;  e.stack
来源：http://hz.ehwqpu.com/gtdpgyerem.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258888.top/gtpepgrmim.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shuidangran.top/gtcxhfhpxh.html

Go:   err.Error()
来源：http://hz.zhengqikj.top/gtpkhwywws.html

Ruby: e.message;  e.backtrace
来源：http://hz.sxryk.cn/gtztktjpaf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.snrcjt.cn/gtahvbgnxp.html

[H09] 带错误码的异常
来源：http://hz.zhaomingkeji.xyz/gtimoqqbgn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.haohaochexian.top/gtcslsltyh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxinkj.top/gtsstypymn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jyoumei.cn/gtaxkrghow.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zdqjudy.top/gtjngcfieb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.vqdsnc.cn/gtxlgbxstd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gtlsbpkesm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tianlin.xyz/gtkmtvkdwj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tianlin.xyz/gtyvymwigf.html

[H10] 资源自动释放
来源：http://hz.shangyingyoupin.top/gtvypunxqr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guowangkeji.top/gtiyjcjprl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xylfe.cn/gtwsshyzxp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtsmrmgfnq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhongyouzk.top/gtwpcjhgrm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhongyouzk.top/gthtnwtets.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangtech.top/gtvjpiuhpo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.quarkkingdee.top/gtzdpirwmc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.9152youxi.cn/gtwaggkkff.html

================================================================================
来源：http://hz.9152youxi.cn/gtgyifkrqs.html

I. 正则表达式
来源：http://hz.fengsongda.top/gtrzdmqnuv.html

================================================================================
来源：http://hz.ehwqpu.com/gtnlxhcxcp.html

[I01] 判断是否匹配
来源：http://hz.hnqzz.top/gtjzaqbutt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydzc1.top/gtdrqvvacx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cashguo.top/gtuwanwnex.html

JS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtixioznej.html

TS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtaqgebhef.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pycfn.com/gtbkjuwogf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yonumen.top/gtiredlbei.html

Ruby: s.match?(/\d+/)
来源：http://hz.mhx1999.top/gtwhhbkstj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yangfankeji.com/gttbneqzfu.html

[I02] 提取所有匹配
来源：http://hz.aibaodan.cn/gtljtxohwo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtjuivccpw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cqqwz.cn/gtgcoexyoz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yanxiufei.cn/gtrndiutli.html

TS:   s.match(/\d+/g)
来源：http://hz.daxiang520.top/gtijrntywi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pengpengdd.cyou/gtqqcahbyp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ybcxt.top/gtgycfsyvp.html

Ruby: s.scan(/\d+/)
来源：http://hz.gaohongyu789.top/gtjudzngij.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.iojbl.cn/gtpfartsfd.html

[I03] 提取捕获分组
来源：http://hz.sysykeji.top/gthgmfjltc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuxming.cn/gtutdpjaxt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yangfankeji.com/gtpilaurru.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangdashe.top/gtfuoidmux.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jlsjyb.cn/gtspdmjwjh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinghuilouyu.cn/gtjyqoqswu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gtgttkibyc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tian-w.cn/gtktpfofem.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gotoacloud.top/gtqvwmypdo.html

[I04] 正则替换
来源：http://hz.yongpay.top/gttytdrwki.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gtapykfyij.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtubwnlfmx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gthhcqwjxb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gthxzvyroc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shzxlz.cn/gtzaiokbpl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhengqikj.top/gtjckaltsn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuxming.cn/gtdtxijwkp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cucudq.cn/gtgjwxkeii.html

[I05] 按正则拆分
来源：http://hz.jyoumei.cn/gterazhesv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangshuangyany.cn/gtwfzkhmdg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gtbrbnbwox.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtkfjslkzo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtytoozasm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gzhubu.top/gtkarufopa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cheryme.top/gtnwqiajni.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtxwnasykm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yvedp.cn/gtydghwtep.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cdnleiting.top/gtuotvrpiu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtqkspmpqf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dashuyun.cn/gtndgxjqjy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtgezqkspz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtokxwvyjh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guowangkeji.top/gtrvzcordl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ehwqpu.com/gtzrnpjlqz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenjidiqi.icu/gtznvmanlc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dashuyun.cn/gtvksnecgt.html

[I07] 忽略大小写与多行模式
来源：http://hz.aizwys.cn/gtapkqdjro.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yonumen.top/gtfosbuizl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tianlin.xyz/gtbtxttdyi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.52xcode.cn/gtcgsbfvhj.html

TS:   /error/gim
来源：http://hz.0kj1m.cn/gtyrdjsvip.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jlsjyb.cn/gtadnpxdpp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.vqdsnc.cn/gtdfxmjiok.html

Ruby: s.scan(/error/i)
来源：http://hz.wangshuangyany.cn/gteworclph.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gzhubu.top/gtjvantvgz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nwbrower.top/gthjyihnpo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yvedp.cn/gtmgfsktxx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gzhubu.top/gtdeevqodn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.vqdsnc.cn/gtzzetexfh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtidbaezub.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.svipenyu.cn/gtzvkpmsoo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tian-w.cn/gtbwqfxujk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigufen.top/gtnohbguni.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtpxeyiuig.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrckmhoju.html

J. 日期与时间
来源：http://hz.snrcjt.cn/gthghmfwqq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthjcbdvie.html

[J01] 获取当前时间
来源：http://hz.chenjidiqi.icu/gtrkhlvjbw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtwgpahxnh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtdttmguim.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtdsuwezsn.html

TS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtgisiuaes.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hywenlv.cn/gtmzusqcrf.html

Go:   time.Now()
来源：http://hz.iojbl.cn/gtxpxpmxod.html

Ruby: Time.now
来源：http://hz.shanyushiyangtech.top/gtbthudmfe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dianchejie.cn/gtkwkbduwn.html

[J02] 格式化输出
来源：http://hz.daria6918.cn/gtlhznizlr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.haohaochexian.top/gtepzmmpuz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtmdxfumme.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yonumen.top/gtoyhmiams.html

TS:   d.toISOString()
来源：http://hz.dashuyun.cn/gtopetpmbt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gtnbiplruv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guannengcc.top/gtjzrreggp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtdadgpado.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jyoumei.cn/gthkbjjail.html

[J03] 字符串解析为日期
来源：http://hz.shangyingyoupin.top/gthfmyfrbv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.andypj.xyz/gtvoaqhcdn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sufxvd.cn/gtoaiakncl.html

JS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gtyfycxbff.html

TS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtrtdlledw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.quarkkingdee.top/gtmgcnzwoc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hongshengwenyu.top/gtqbyvjzao.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtkndhjpce.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sweek.top/gtbhkuplkp.html

[J04] 时间戳与日期互转
来源：http://hz.jyoumei.cn/gtztwdhjqr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ivvv.top/gtuequloxc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zdqjudy.top/gtnrxgwuig.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258.top/gtpekmrcio.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.c1oappe.top/gtnlhiyutq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.snrcjt.cn/gtkbdhbnfr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jianghu66.top/gtmxcizbqp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydjk.org.cn/gtlodliuzp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnxiangtu.top/gtlrsvrmty.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangtech.top/gtgijzgiim.html

Py:   now + timedelta(days=7)
来源：http://hz.hammf.cn/gtnichknvd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtcizzxbzq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtcfyxezdy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtxqcaumkx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ivvv.top/gtzbasxzff.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hongshengwenyu.top/gtkjpqrbgo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuanzhike.top/gtaycsjftq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nwbrower.top/gtielnhgqg.html

[J06] 计算两时间之差
来源：http://hz.jyoumei.cn/gtfefzhcbs.html

Py:   (end - start).total_seconds()
来源：http://hz.havefunace.top/gtdmsmxvse.html

PHP:  $end->diff($start)->days;
来源：http://hz.bjfxy.top/gtiityryfr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangshuangyany.cn/gthujstolz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.birdmap.top/gtlxjnikqd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuanzx.com/gtggutlxem.html

Go:   end.Sub(start).Hours()
来源：http://hz.cdnleiting.top/gtscgfyekq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.meibo888.top/gtnbfrsovn.html

C#:   (end - start).TotalSeconds
来源：http://hz.xylfe.cn/gtznygwmsk.html

[J07] 比较两个日期
来源：http://hz.jinghuilouyu.cn/gtvspqxfnp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gttwglprfx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinyuanbaomall.cn/gtzdtsaine.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtbvrxqjhn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtiebiiauv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnxiangtu.top/gtbgvuaxci.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.redwolf501.top/gtyoxqlfrj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtsozpsmzd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gtrddirrad.html

[J08] 提取年月日与星期
来源：http://hz.yj202588.top/gtddqqhdml.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aizwys.cn/gtufawbtuy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shzxlz.cn/gtovtlmyzi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenzaomai.com/gtgonilryd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yvedp.cn/gtiutbbcnw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gtayqbaxcg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pycfn.com/gtjhqpotzg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gzhubu.top/gtezqqrrlr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ywan-chungtsiang.top/gtyyodwjcz.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtpsrkpprk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cashguo.top/gtjlenlplw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigfzy.top/gtyxpewgxs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtkaveflvn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtvffzhohq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shangyingyoupin.top/gtjkkuqimp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gtuchibbto.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guowangkeji.top/gtrievvthg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cqqwz.cn/gttxtrqyeq.html

[J10] 取今天 / 本月第一天
来源：http://hz.sysykeji.top/gtueftzkte.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cashguo.top/gtsqcltjiw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tian-w.cn/gtqglaruuc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hongshengwenyu.top/gttunwdicc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtgkqslezo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenjidiqi.icu/gtiachhrbs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sysykeji.top/gtpelmtqbz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinyuanbaomall.cn/gtkynjnxcm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.birdmap.top/gtzbdijmjc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtncfleust.html

K. JSON 与序列化
来源：http://hz.gogol.net.cn/gtksyudgss.html

================================================================================
来源：http://hz.cucudq.cn/gtkiyuukdp.html

[K01] 对象转 JSON 字符串
来源：http://hz.yuanzhike.top/gtsxsvqkre.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtvbwohcza.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtfevfkhtk.html

JS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gttbmkhymf.html

TS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtnzlnnvli.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.0kj1m.cn/gtyzzglyfw.html

Go:   json.Marshal(obj)
来源：http://hz.jqgfzy.top/gtadvlmabj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.9152youxi.cn/gtwkavboaw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhongyouzk.top/gtwgzkoulo.html

[K02] JSON 字符串转对象
来源：http://hz.yuxming.cn/gthcqifcvn.html

Py:   json.loads(s)
来源：http://hz.zhaomingkeji.xyz/gtwrxsrhao.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenlongwang.top/gtnwjoqldt.html

JS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtvikubxwb.html

TS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gtfxjexpql.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtduhlcqfc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydjk.org.cn/gtrezloyom.html

Ruby: JSON.parse(s)
来源：http://hz.cashguo.top/gtpwcohxdb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenlongwang.top/gthohygyap.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aizwys.cn/gtgwpuxykx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtnpchkytq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtesuptivz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtvqdxkucg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.vqdsnc.cn/gtzkabqqrn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xinyue.icu/gtyvxrcaao.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cashguo.top/gtlpfqmtph.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dianchejie.cn/gtoubziadm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fengsongda.top/gthprmtlbr.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtuiujcpcr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtrmrkruse.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xylfe.cn/gtbjaglvua.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydzc1.top/gtplwmzdku.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gtiilmgncs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuxming.cn/gtvezcfexb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtotlkouoh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.iojbl.cn/gtdbbnoobm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.316326.xyz/gtplhfyndd.html

[K05] 深拷贝对象
来源：http://hz.jyoumei.cn/gthauqspvw.html

Py:   copy.deepcopy(obj)
来源：http://hz.snrcjt.cn/gtyvwtqqom.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigfzy.top/gtniltpmwj.html

JS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gtpusrvdfu.html

TS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtgrjsngtj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.daxiang520.top/gtqvyeooky.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hywenlv.cn/gtxbtdloel.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cucudq.cn/gtumqrhivb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydzc1.top/gtcciqkxpm.html

[K06] 解析 URL 查询串
来源：http://hz.xylfe.cn/gtytdqljbo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pengpengdd.cyou/gtjwdnxsbi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtdtqpsomj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.0kj1m.cn/gtvnwavdgy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gtungtkkoh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenjidiqi.icu/gtcykmjstr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aibaodan.cn/gtnnevglhg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenzaomai.com/gthuymzdju.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigufen.top/gttlzqgcca.html

[K07] 进制转换
来源：http://hz.yangfankeji.com/gtrvskqcwr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.svipenyu.cn/gttwdrmilc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shuidangran.top/gtitbmcmjl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gtqgbmvkba.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtpohkujsn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.birdmap.top/gtucbbozwy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtlbqgbpdp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.bjfxy.top/gtjxrzcspq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pycfn.com/gtwbjotbqi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.meibo888.top/gtwjsbxqog.html

Py:   pickle.dumps(obj)
来源：http://hz.chenzaomai.com/gtyjkvywll.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj202588.top/gtlyzwvoau.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cqqwz.cn/gtwfpfqune.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hysaishi.cn/gtlesaukpx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.snrcjt.cn/gtydnlmvkl.html

Go:   encoding/gob
来源：http://hz.ywan-chungtsiang.top/gtuvbgungj.html

Ruby: Marshal.dump(obj)
来源：http://hz.pycfn.com/gtdwcvcyvi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhongyouzk.top/gtxboyvaof.html

================================================================================
来源：http://hz.dianchejie.cn/gtvsqkmpqz.html

L. 网络请求
来源：http://hz.sysykeji.top/gtqfaaapgd.html

================================================================================
来源：http://hz.havefunace.top/gtfycicsyx.html

[L01] 发送 GET 请求
来源：http://hz.gzhubu.top/gtpqcwocfh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yanxiufei.cn/gtcvfltobw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nanxuanxn.top/gtjfzztdnq.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtycwywtdd.html

TS:   await fetch(url)
来源：http://hz.shuidangran.top/gtueutqczv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yueranfly.top/gtuadjwnqb.html


<!-- 参考信息 -->