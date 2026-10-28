代发 wailian999

[H03] 主动抛出异常
来源：http://hz.jlsjyb.cn/gtmunezwsp.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhongyouzk.top/gtulznqgxm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtxqcmetkd.html

JS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtbcnkspze.html

TS:   throw new Error("错误信息");
来源：http://hz.bjfxy.top/gtorgavpct.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daria6918.cn/gttjjbuvlj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ybcxt.top/gtfgwkpndx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.52xcode.cn/gtqomamqlp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sweek.top/gtqqihxrbe.html

[H04] 自定义异常类型
来源：http://hz.jinghuilouyu.cn/gtklloigvk.html

Py:   class MyError(Exception): pass
来源：http://hz.fengsongda.top/gtinuligea.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gthdjolaiw.html

JS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtsjueivvk.html

TS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gtskxfzlvb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtaikcidkj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhengqikj.top/gtclklrayn.html

Ruby: class MyError < StandardError; end
来源：http://hz.fengsongda.top/gtmxvkajsn.html

C#:   class MyException : Exception {}
来源：http://hz.yuxming.cn/gtzvfcmifl.html

[H05] 捕获特定类型
来源：http://hz.chenjidiqi.icu/gtkvspecgr.html

Py:   except ValueError as e:
来源：http://hz.jiagoushi.top/gtqitzuuua.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxuanxn.top/gtildlharx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.0kj1m.cn/gtnnugrckr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtqhokqrcl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnxiangtu.top/gtjfmhcetm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jianghu66.top/gtelwojhzt.html

Ruby: rescue ArgumentError => e
来源：http://hz.sxryk.cn/gtrwabhcub.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.haohaochexian.top/gtxehffwsm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhengqikj.top/gttrclxvha.html

Py:   value = d.get("k") or default
来源：http://hz.ppjwa.cn/gtimozwoby.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenzaomai.com/gtrcobgzdt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtnemcktgl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhixingplan.top/gtysgbmaoc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtslqpyyhh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ywan-chungtsiang.top/gtytipducb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gthwkiiaxk.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtmggyfovn.html

[H07] 断言
来源：http://hz.xuetiantiany.cn/gtqnziutlx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jlsjyb.cn/gthruyrvqz.html

PHP:  assert($x > 0);
来源：http://hz.ydzc1.top/gtoxxawtrs.html

JS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gttegxesgb.html

TS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtmulswjxl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tian-w.cn/gtrmouqljx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.c1oappe.top/gtmupocrek.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yangfankeji.com/gtoaiqttoy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daxiang520.top/gtbhazvopo.html

[H08] 获取错误信息与堆栈
来源：http://hz.shangyingyoupin.top/gtvlyfciyk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gtzlsmvyui.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daxiang520.top/gtodjfhgzh.html

JS:   e.message;  e.stack
来源：http://hz.jqgufenzy.top/gthaypyrjc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ybcxt.top/gtkvehkxdl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ehwqpu.com/gtwbsrrxdg.html

Go:   err.Error()
来源：http://hz.vqdsnc.cn/gtzfjdujjv.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinyuanbaomall.cn/gtnlkspexh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shangyingyoupin.top/gteojkvodf.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtuldipujs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ywan-chungtsiang.top/gtaeoohxhy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtxnymtpto.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xinyue.icu/gthgqtfcvt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangkeji.top/gtphjvgzjh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xziqi.cn/gthwzvtsjn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gotoacloud.top/gtomrrgkis.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sxryk.cn/gtmtesynlm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.mhx1999.top/gtrfdzdvcs.html

[H10] 资源自动释放
来源：http://hz.jinyuanbaomall.cn/gtbrvgvdiq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ivvv.top/gtrtnuddcg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yongpay.top/gtbejhykgh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtatriawqn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtqiqgmvud.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgufenzy.top/gtjfwdsork.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gtvqobwpsv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cqqwz.cn/gtnkmvehnh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gotoacloud.top/gtoimnxuoh.html

================================================================================
来源：http://hz.jyoumei.cn/gtwntgyzct.html

I. 正则表达式
来源：http://hz.cheryme.top/gtuoqinrun.html

================================================================================
来源：http://hz.mhx1999.top/gtlpfthqtp.html

[I01] 判断是否匹配
来源：http://hz.ydjk.org.cn/gttypihqep.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.andypj.xyz/gtndfflijk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj202588.top/gtiraktugg.html

JS:   /\d+/.test(s)
来源：http://hz.hywenlv.cn/gtyrwzcdvu.html

TS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtiybvjwqf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sufxvd.cn/gtlbpnrzwx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.svipenyu.cn/gtflanguni.html

Ruby: s.match?(/\d+/)
来源：http://hz.tian-w.cn/gttwucickb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shanyushiyangtech.top/gttdkbbeeh.html

[I02] 提取所有匹配
来源：http://hz.feifeiyinyue.top/gtodkixagl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sxryk.cn/gttvngkwyd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jianghu66.top/gthxwhtvmm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daria6918.cn/gtrxibtvcr.html

TS:   s.match(/\d+/g)
来源：http://hz.hysaishi.cn/gtiftrxlbi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hfpthk.cn/gtqteywcky.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.c1oappe.top/gthaefvvwo.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxuanxn.top/gtepsmpjow.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gtickxflmq.html

[I03] 提取捕获分组
来源：http://hz.yueranfly.top/gtyptnisvg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jyoumei.cn/gtfrsejmbp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinghuilouyu.cn/gtbzvheoth.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sufxvd.cn/gtdplekpqq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.quarkkingdee.top/gtssohggek.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fzhhl.top/gtbmxcrtoc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xziqi.cn/gtiolvypht.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhoulong.xyz/gtoxpuwotm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.redwolf501.top/gtywkspjbe.html

[I04] 正则替换
来源：http://hz.yuanzhike.top/gtcnpxxmud.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhoulong.xyz/gtfjusypuz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtaueuzfxs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtxhnkpihr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtztlstkgr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ppjwa.cn/gtfsxwmvej.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydzc1.top/gtnmzgcaas.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnxiangtu.top/gtedxxpsfv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cheryme.top/gtwxzpmrqd.html

[I05] 按正则拆分
来源：http://hz.shzxlz.cn/gtoxzimvzh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zycfv.cn/gtefgpclam.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.316326.xyz/gtrezcguuw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtigmdcvpq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtprzyrypu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj202588.top/gtwmidrrkz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shzxlz.cn/gtdkhftwul.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtpqdgywar.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhaomingkeji.xyz/gtngesghuy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daria6918.cn/gtgkccfjnr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtxlofoysd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gtnxjobgqk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtgfmklfoz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jyoumei.cn/gtyhjhdstb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shzxlz.cn/gtpnwpdoog.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shangyingyoupin.top/gtbawuibew.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgufenzy.top/gtngiblyyy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtgmnqwmsj.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gttbjywbeq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cheryme.top/gtwujexkhx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.guowangkeji.top/gtbfwatomd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.svipenyu.cn/gtyxxzzgpz.html

TS:   /error/gim
来源：http://hz.hywenlv.cn/gtoakxpjem.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xylfe.cn/gtblllswda.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cheryme.top/gtumpjdzvq.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtedpexktc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.bjfxy.top/gtoptqnxqk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.smart0.xyz/gtkvspnmkz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.iojbl.cn/gtcmylkjhs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yongpay.top/gthcunvemv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tianlin.xyz/gtuqtzwhgf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtjgrdhldn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.havefunace.top/gtzfnncawk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tianlin.xyz/gtnclbrsng.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxinkj.top/gtltrjehlq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtsbkoigiw.html

================================================================================
来源：http://hz.316326.xyz/gtafooihbm.html

J. 日期与时间
来源：http://hz.tianlin.xyz/gtmukypaki.html

================================================================================
来源：http://hz.ppjwa.cn/gtaugaeulj.html

[J01] 获取当前时间
来源：http://hz.nanxuanxn.top/gtllwdiljt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.bjfxy.top/gttkjdrdoy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtkgfzdjuk.html

JS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtbbdcyarr.html

TS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtemmpbubj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yvedp.cn/gtjofjhlab.html

Go:   time.Now()
来源：http://hz.yj20258.top/gtkzutraez.html

Ruby: Time.now
来源：http://hz.0kj1m.cn/gtmxrajots.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hfpthk.cn/gtwyldbxgk.html

[J02] 格式化输出
来源：http://hz.guowangkeji.top/gtkkvpkwvo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.haohaochexian.top/gtkjekhtgv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hysaishi.cn/gtvseeimmg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pycfn.com/gtidqiklvp.html

TS:   d.toISOString()
来源：http://hz.jiagoushi.top/gttdajniml.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sysykeji.top/gttdqxymkj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.svipenyu.cn/gtjefiklrx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtzpsppcav.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.52xcode.cn/gtjrrkjhad.html

[J03] 字符串解析为日期
来源：http://hz.jinqigufen.top/gtmsfmtvrn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sweek.top/gttwyaghdv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.52xcode.cn/gtwabphpxo.html

JS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtrjeenohv.html

TS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtibfswufl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtlulirxap.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuxming.cn/gthfchzvuq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gttsawjupf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.meibo888.top/gtkwtvompu.html

[J04] 时间戳与日期互转
来源：http://hz.iojbl.cn/gtggnquiuv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tanke756.top/gtclwmdjwl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fzhhl.top/gtgvrxdnjn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dianchejie.cn/gtkudtcqft.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhengqikj.top/gtqfpwrmdh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hysaishi.cn/gtsvrrzeoc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aizwys.cn/gtfojvfenk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hammf.cn/gtrniueigm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.quarkkingdee.top/gthtanlsmo.html

[J05] 时间加减（加 7 天）
来源：http://hz.tanke756.top/gtzgeweeis.html

Py:   now + timedelta(days=7)
来源：http://hz.yvedp.cn/gtsgxtipcg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sufxvd.cn/gtikiybupi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtzermhkyw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gtxdhujjxd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sufxvd.cn/gtuxazcgqe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hywenlv.cn/gtaxqgxupc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gtmbxtqjte.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jyoumei.cn/gttexkrjhg.html

[J06] 计算两时间之差
来源：http://hz.fzhhl.top/gtdzhapowg.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gtvvebbsvy.html

PHP:  $end->diff($start)->days;
来源：http://hz.guannengcc.top/gtpmzjbwgk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenjidiqi.icu/gtfbhhvcpu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj20258.top/gtxfeclcbj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xylfe.cn/gtfwlisyyb.html

Go:   end.Sub(start).Hours()
来源：http://hz.hammf.cn/gtrfbhpvvp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cdnleiting.top/gtaqadrdnc.html

C#:   (end - start).TotalSeconds
来源：http://hz.shzxlz.cn/gtzqpwziml.html

[J07] 比较两个日期
来源：http://hz.zdqjudy.top/gtdtglyzlm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtanmfkgbi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gtsaixamiu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hywenlv.cn/gtuycpyfom.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.aibaodan.cn/gtueblyegl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangshuangyany.cn/gtjcmqxtsz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnqzz.top/gtyvemntsa.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtibwgvycx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtgjrqsdug.html

[J08] 提取年月日与星期
来源：http://hz.fengsongda.top/gtonrzixdi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.haohaochexian.top/gtmleuogxb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ybcxt.top/gtocqvzyin.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fzhhl.top/gttxzqnasf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.vqdsnc.cn/gtyvxzgbhz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ehwqpu.com/gtchusyiuk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dashuyun.cn/gtnmouesxt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dashuyun.cn/gtajsciktc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yangfankeji.com/gttuaatqcj.html

[J09] 时区处理
来源：http://hz.pengpengdd.cyou/gttxvcpltn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtcmakztog.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhixingplan.top/gtmqacxnae.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtzrkfbdit.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gthlxonfkj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgfzy.top/gtlzbvaqdb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cqqwz.cn/gtqledursi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.kuanghao11.cn/gtmnjhgndi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hywenlv.cn/gtqeorivvr.html

[J10] 取今天 / 本月第一天
来源：http://hz.jlsjyb.cn/gtreiytyrm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.svipenyu.cn/gtjlhuvutr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.316326.xyz/gtofgfxtat.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tianlin.xyz/gtzcajwojn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.smart0.xyz/gtzzlbwxwx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.quarkkingdee.top/gtegsqitms.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xylfe.cn/gtkfrltxze.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgufenzy.top/gtlcirlgpo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hysaishi.cn/gtrxrkitiu.html

================================================================================
来源：http://hz.jyoumei.cn/gtosddrrzc.html

K. JSON 与序列化
来源：http://hz.birdmap.top/gtoeprcfkb.html

================================================================================
来源：http://hz.guannengcc.top/gtciiszeci.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtyryluokq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtaihmikto.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xinyue.icu/gtdvsxacbq.html

JS:   JSON.stringify(obj)
来源：http://hz.bjfxy.top/gtqmevktbb.html

TS:   JSON.stringify(obj)
来源：http://hz.sufxvd.cn/gtukwjbiwv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gtdoptbeyw.html

Go:   json.Marshal(obj)
来源：http://hz.hongshengwenyu.top/gthxkajysd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhijiandao.cn/gtlfzzblbt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jlsjyb.cn/gtqgqgtguv.html

[K02] JSON 字符串转对象
来源：http://hz.feifeiyinyue.top/gthukcrrzy.html

Py:   json.loads(s)
来源：http://hz.mhx1999.top/gtxlmzowss.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenzaomai.com/gtzefidotr.html

JS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtgzhzlwtb.html

TS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gtvmkomyfi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhaomingkeji.xyz/gtdezwmjdc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtrdfnvuho.html

Ruby: JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtkvjzhrur.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hammf.cn/gtsdoolzbe.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gteusdjssd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtvdehbopl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtttfuakxz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtpoxhrzpl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtxotasobw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnxiangtu.top/gtsndxqjzu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangshuangyany.cn/gtkyatundl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtfonrmpci.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tian-w.cn/gteypsknnl.html

[K04] 读取 JSON 文件
来源：http://hz.guannengcc.top/gtzhempfpr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgufenzy.top/gtntjciksv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.9152youxi.cn/gtfqzhpztv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtdykpkgys.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtgfppcnsa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenlongwang.top/gthyvcdkei.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtzhzixukb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhoulong.xyz/gtyuljadyx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zycfv.cn/gthklxshvb.html

[K05] 深拷贝对象
来源：http://hz.ivvv.top/gtnzsaaeyx.html

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtmxbdcgeu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenlongwang.top/gtvbwovvqm.html

JS:   structuredClone(obj)
来源：http://hz.hnqzz.top/gtyuhhdmym.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtmhmxlzeh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fengsongda.top/gtfqtajusj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtutnpldti.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xziqi.cn/gthksdqxrj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtogaimoda.html

[K06] 解析 URL 查询串
来源：http://hz.hnxiangtu.top/gthcunuvet.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgufenzy.top/gtlipqfpoy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hongshengwenyu.top/gtvsuekcjs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtactjmhmq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gttjregijl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guannengcc.top/gtkdvqssbw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ybcxt.top/gtmiswkebl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fzhhl.top/gttlmkncab.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daxiang520.top/gtnptahazx.html

[K07] 进制转换
来源：http://hz.yangfankeji.com/gtnkrkhjjj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtsmasbuql.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fengsongda.top/gtovbgozdz.html


<!-- 参考信息 -->