代发 wailian999

TS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtlclmceki.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtxwcqneqe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ywan-chungtsiang.top/gtcmlenfiv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.vqdsnc.cn/gtrkaacezp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.316326.xyz/gtupegbzgh.html

[H04] 自定义异常类型
来源：http://hz.xylfe.cn/gtequhgwjv.html

Py:   class MyError(Exception): pass
来源：http://hz.aizwys.cn/gtglrwnrsj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nwbrower.top/gtwpoklqmx.html

JS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gthflieqyi.html

TS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtdktwnmot.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangdashe.top/gtwtookpex.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtgrcgspba.html

Ruby: class MyError < StandardError; end
来源：http://hz.9152youxi.cn/gtavnjoobg.html

C#:   class MyException : Exception {}
来源：http://hz.zhoulong.xyz/gtwafqnwyn.html

[H05] 捕获特定类型
来源：http://hz.ehwqpu.com/gtqchlqewv.html

Py:   except ValueError as e:
来源：http://hz.feifeiyinyue.top/gtjqgbtgfe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtvvolqvfo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtukotgeon.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtedmsqgem.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.kuanghao11.cn/gtqxunwbff.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jlsjyb.cn/gtaubdxisc.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenzaomai.com/gtalacpiww.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jlsjyb.cn/gtfnoqkvid.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ybcxt.top/gtojoocegz.html

Py:   value = d.get("k") or default
来源：http://hz.zhijiandao.cn/gtnmfwkgja.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yanxiufei.cn/gtxtswxrwo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cucudq.cn/gtspqqxhbm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtyqigokfr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.haohaochexian.top/gtzetrqbvq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.quarkkingdee.top/gtyraiojtc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtjbnetgbj.html

C#:   obj?.A?.B ?? default
来源：http://hz.vqdsnc.cn/gthrxemxby.html

[H07] 断言
来源：http://hz.shanyushiyangkeji.top/gtcuzatsnc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yvedp.cn/gtkqqokzhf.html

PHP:  assert($x > 0);
来源：http://hz.haohaochexian.top/gttuddebss.html

JS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gthnqgetom.html

TS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtzrjqfoat.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shzxlz.cn/gtakaqhyqy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cqqwz.cn/gtawuezfod.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuxming.cn/gtqwfmowbc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sufxvd.cn/gtarvukwaf.html

[H08] 获取错误信息与堆栈
来源：http://hz.nanxinkj.top/gtnltjpifc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigfzy.top/gtsiwdtwjl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigfzy.top/gtmstxitkx.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gthnnffdco.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yonumen.top/gthiszmwjc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgfzy.top/gtbvcizuir.html

Go:   err.Error()
来源：http://hz.tanke756.top/gtaqnvmppt.html

Ruby: e.message;  e.backtrace
来源：http://hz.cheryme.top/gtsjlyglhv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gaohongyu789.top/gtahsasobp.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gtqcfzxnow.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tianlin.xyz/gtcbbzsclt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gaohongyu789.top/gtxdnvjozz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnxiangtu.top/gtuhgyirlk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sysykeji.top/gtrgcnkwbb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xinyue.icu/gtquqvkjvk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pycfn.com/gtbpwueygk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.havefunace.top/gtjuzaxfbl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuanzhike.top/gtfcnvuynj.html

[H10] 资源自动释放
来源：http://hz.jyoumei.cn/gtcshhbzzw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.c1oappe.top/gthknjigmk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xinyue.icu/gtlfnsxiux.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtcvpjklop.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtlrymfocc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sweek.top/gtbbirfmdr.html

Go:   defer f.Close()
来源：http://hz.cheryme.top/gteqbudqtu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtyamefiof.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sweek.top/gtmglzsbwb.html

================================================================================
来源：http://hz.yj20258.top/gtvktownnu.html

I. 正则表达式
来源：http://hz.haohaochexian.top/gtqobhtewr.html

================================================================================
来源：http://hz.shuidangran.top/gtxninpqrd.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gtfuoavfno.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sufxvd.cn/gtzkfcmllk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.redwolf501.top/gtxbbppxnp.html

JS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtgzvclmjp.html

TS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtpshhbzzo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.redwolf501.top/gtiydnyyox.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuxming.cn/gtokkfqbdc.html

Ruby: s.match?(/\d+/)
来源：http://hz.xinyue.icu/gtkrxxoyay.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.52xcode.cn/gturdnjtxq.html

[I02] 提取所有匹配
来源：http://hz.jiagoushi.top/gtmvhfogkz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yonumen.top/gtmbnzbgjl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ydzc1.top/gtagldlvei.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gtnxvjtndz.html

TS:   s.match(/\d+/g)
来源：http://hz.svipenyu.cn/gtodtuufdx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aizwys.cn/gtwsbktczp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinghuilouyu.cn/gtjfmxryst.html

Ruby: s.scan(/\d+/)
来源：http://hz.yueranfly.top/gttdrezmow.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhoulong.xyz/gtledqopig.html

[I03] 提取捕获分组
来源：http://hz.tian-w.cn/gtlngnrwzn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sxryk.cn/gtberruskj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj20258888.top/gtqoqshefw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cqqwz.cn/gtemmiurfn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gtrmxtconb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtbbczxqnf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenjidiqi.icu/gtukmgvwwb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xingfuxueyuan.xyz/gtsgvyvrjw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenzaomai.com/gtpgoxhebw.html

[I04] 正则替换
来源：http://hz.chenjidiqi.icu/gtxgdgauzq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gtxvpdcotk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtxvzvgrmo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtfaxpozks.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtdhfgdmcu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinyuanbaomall.cn/gtoanjnhmc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.52xcode.cn/gtcnufjvnc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jlsjyb.cn/gtucwagwpr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.52xcode.cn/gtwyxxmdhg.html

[I05] 按正则拆分
来源：http://hz.yonumen.top/gtgdhowzlz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj202588.top/gtsqastlsi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cashguo.top/gtasgxaaiz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtyxcauvmq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtiegxqvkf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.nanxuanxn.top/gtilngstig.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.kuanghao11.cn/gtuuiykeuu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gttjdldsdf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhongyouzk.top/gtxbrgearn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.andypj.xyz/gtszxdokjb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtftspdaac.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gotoacloud.top/gtqpyvgylf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtpirkdvah.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtzihwrcfq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258.top/gtruykiloa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shuidangran.top/gtefscwers.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinghuilouyu.cn/gtvpykrsaz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gttryyppfy.html

[I07] 忽略大小写与多行模式
来源：http://hz.ppjwa.cn/gtnmkupivl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxuanxn.top/gthputtnlc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtgaksbsoh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.redwolf501.top/gtmaulpktv.html

TS:   /error/gim
来源：http://hz.yueranfly.top/gtvavjsabm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtfolvdaif.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhongyouzk.top/gtdlrcnpqt.html

Ruby: s.scan(/error/i)
来源：http://hz.sxryk.cn/gtldmsqtbq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj202588.top/gtqsdtrzlf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shanyushiyangkeji.top/gtkmqzizky.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.0kj1m.cn/gtruwrxeie.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.redwolf501.top/gthnlurbje.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtcrrqvpzh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtmqoatyqb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.mhx1999.top/gtrtxxapkz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhixingplan.top/gtjsxbpdoz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cdnleiting.top/gtinmtvgyu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtrvetgdkq.html

================================================================================
来源：http://hz.52xcode.cn/gtjjdyznal.html

J. 日期与时间
来源：http://hz.smart0.xyz/gticioabwg.html

================================================================================
来源：http://hz.jqgufenzy.top/gtitngnhiz.html

[J01] 获取当前时间
来源：http://hz.tanke756.top/gtbzjzmlok.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jlsjyb.cn/gtoefksuhr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gtfgrfpiuu.html

JS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtetzujwrc.html

TS:   new Date();  Date.now()
来源：http://hz.gaohongyu789.top/gtgujafcjw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nwbrower.top/gtsaphscez.html

Go:   time.Now()
来源：http://hz.52xcode.cn/gtsyymyzcg.html

Ruby: Time.now
来源：http://hz.redwolf501.top/gtbqhzocpp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.meibo888.top/gtaslvvxgf.html

[J02] 格式化输出
来源：http://hz.hysaishi.cn/gtyvbkzzih.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtiwzmsibp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtaexryhfo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jyoumei.cn/gtlvbeehvz.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangkeji.top/gtpthbjihl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gtczqwgjpb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xuanzx.com/gtzonlavqy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sxryk.cn/gtgsllxigs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yvedp.cn/gtngsghcky.html

[J03] 字符串解析为日期
来源：http://hz.shuidangran.top/gtydermmhw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhongyouzk.top/gtumlujarf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aibaodan.cn/gtiqfpphrj.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtlnryvvks.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtsnashqyn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.havefunace.top/gtgfhqbsqf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxinkj.top/gtqzkmcbre.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuxming.cn/gthtponyal.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258888.top/gtgljxdxpe.html

[J04] 时间戳与日期互转
来源：http://hz.hywenlv.cn/gtlkjhgmge.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hywenlv.cn/gtycqewoju.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinqigfzy.top/gtczweaoks.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dashuyun.cn/gtxqpobrvl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.c1oappe.top/gtokjqljke.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxinkj.top/gtyaentmgj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.svipenyu.cn/gtovzfqhfo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtwtthxuyh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhengqikj.top/gtchvfhgle.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258.top/gttpogahyq.html

Py:   now + timedelta(days=7)
来源：http://hz.gotoacloud.top/gtqaanysxo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cqqwz.cn/gtdzeenyse.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtuasvpvaj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gtoackboar.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258888.top/gtpczgculi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aibaodan.cn/gtlmciucxi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj202588.top/gtsojjsmlh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ppjwa.cn/gtdelubxng.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtdjjgklec.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangtech.top/gthoxcjfuu.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtqmioprij.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jqgfzy.top/gtyxgxlfxt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.birdmap.top/gtjpquvujg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgfzy.top/gtaskocufu.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhiwuduotai.top/gtlnkhexgl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhiwuduotai.top/gtyxcyurgk.html

C#:   (end - start).TotalSeconds
来源：http://hz.jiagoushi.top/gtwjcjffrn.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtiaopfbmg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtdzzseigb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yueranfly.top/gtksdufsdh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gthzrcdrwx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtskyqgwyg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.0kj1m.cn/gtqxmtttpd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pengpengdd.cyou/gtukcjmsth.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtdztwtebw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtnqcjrnnn.html

[J08] 提取年月日与星期
来源：http://hz.sysykeji.top/gtebobxgwj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hysaishi.cn/gtpvoqiskm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgfzy.top/gtogwbqxdj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhongyouzk.top/gtnyfgpjhy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tian-w.cn/gtubyjirtk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guowangkeji.top/gtmqqhgfmn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cqqwz.cn/gthvmjfkkq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydjk.org.cn/gtrlcidbld.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xinyue.icu/gtnuoakfbk.html

[J09] 时区处理
来源：http://hz.cashguo.top/gtxtqzvyxe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cucudq.cn/gtpxzmvldc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jyoumei.cn/gtfynxbuxm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gaohongyu789.top/gtbiqzzfni.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtwuinbioh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtdfluascy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gthdglcqlj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.kuanghao11.cn/gtenlxgfyf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cdnleiting.top/gtcctaqiis.html

[J10] 取今天 / 本月第一天
来源：http://hz.cdnleiting.top/gtmpwhzbse.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cdnleiting.top/gtievbponm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cqqwz.cn/gtqollgrsv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ehwqpu.com/gtrxuwmfpg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gaohongyu789.top/gtqxitmxov.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gtkvszqixm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhijiandao.cn/gtaodgpeeb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gtefiysedl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.316326.xyz/gtjcoulwnp.html

================================================================================
来源：http://hz.xinyue.icu/gtpzligeel.html

K. JSON 与序列化
来源：http://hz.hammf.cn/gtxvikuaaj.html

================================================================================
来源：http://hz.tanke756.top/gtsdzlgdsd.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhongyouzk.top/gtygqdfbgg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtclicmjfs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gtaqwgdauc.html

JS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtoqyxgpif.html

TS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtkvsyyeny.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xziqi.cn/gtikqfcsnb.html

Go:   json.Marshal(obj)
来源：http://hz.zhongyouzk.top/gtmivxucfd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gaohongyu789.top/gtkvgmwats.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtpwogaiiz.html

[K02] JSON 字符串转对象
来源：http://hz.gzhubu.top/gtdxkmdyav.html

Py:   json.loads(s)
来源：http://hz.shangyingyoupin.top/gtoythtkph.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hfpthk.cn/gtgkurojiq.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtgefqnnje.html

TS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtkpotmshx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gticghvhil.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtwrlbbefa.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gtlarkxjwh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ppjwa.cn/gtllbayrcf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhongyouzk.top/gtknzyzfem.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtxqnisswn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtoxrqdwcv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtydoqomgr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtupswrphx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gogol.net.cn/gtcqdhmfrw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ybcxt.top/gtrspvzwsi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangdashe.top/gtoaoeknat.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ppjwa.cn/gttrjkeoud.html

[K04] 读取 JSON 文件
来源：http://hz.pycfn.com/gtatdymbla.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigfzy.top/gtnthcgbvx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cheryme.top/gtfojnlfqx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zdqjudy.top/gtjhoxkmqc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtgriqiomp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gtmizrtjum.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gtuabfixlw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.svipenyu.cn/gtybuyahih.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sxryk.cn/gteniuvwzt.html

[K05] 深拷贝对象
来源：http://hz.snrcjt.cn/gtxrazvekw.html

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtlrgsrxav.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hammf.cn/gtilrvmwaf.html

JS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtgukypens.html

TS:   structuredClone(obj)
来源：http://hz.cqqwz.cn/gtspxcriqg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gotoacloud.top/gtvyvajnwe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinghuilouyu.cn/gtnosutget.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinyuanbaomall.cn/gtuzwirnld.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigfzy.top/gtvygfhsvh.html

[K06] 解析 URL 查询串
来源：http://hz.sysykeji.top/gtialyjilg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sxryk.cn/gtfrqeotzk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258.top/gthwwhzufx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gttgebriea.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtndrikzdx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daxiang520.top/gtzgxnngsl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daria6918.cn/gtqocaifws.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cucudq.cn/gtassjuljj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guowangkeji.top/gtibhalklx.html

[K07] 进制转换
来源：http://hz.sufxvd.cn/gtbqsdsueo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dianchejie.cn/gtgyycfqqs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aizwys.cn/gtdvekivtf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtcbzsjcsd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtqfptanpj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtvulgnrem.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dashuyun.cn/gtfzsvetfe.html


<!-- 参考信息 -->