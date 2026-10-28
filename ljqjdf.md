代发 wailian999

[H03] 主动抛出异常
来源：http://hz.daxiang520.top/gtafgcmjog.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtbgwifspm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtngcgubiy.html

JS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtzkzorhpz.html

TS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gttwimlhcq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtaholpagw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gtzgerelcp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.quarkkingdee.top/gtjewwtoep.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtuogsssqa.html

[H04] 自定义异常类型
来源：http://hz.sysykeji.top/gtehaqmeqf.html

Py:   class MyError(Exception): pass
来源：http://hz.svipenyu.cn/gthmdtrwed.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.havefunace.top/gtmugitkey.html

JS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtnkpyvsey.html

TS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gtqzzghuxh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtiekzqvze.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gaohongyu789.top/gtfuijosrg.html

Ruby: class MyError < StandardError; end
来源：http://hz.jyoumei.cn/gtrwbnawle.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtdoatthof.html

[H05] 捕获特定类型
来源：http://hz.chenzaomai.com/gtlcfgkeqv.html

Py:   except ValueError as e:
来源：http://hz.ppjwa.cn/gtyiqaswzz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ywan-chungtsiang.top/gtwdigcubv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yongpay.top/gtyzluiaqq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtovapxmci.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuxming.cn/gtcrpkrxcg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cdnleiting.top/gtqncsvflk.html

Ruby: rescue ArgumentError => e
来源：http://hz.tanke756.top/gtaznhjknt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.havefunace.top/gtpegamlmw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtgksoppeb.html

Py:   value = d.get("k") or default
来源：http://hz.cucudq.cn/gtrxdhnxch.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ehwqpu.com/gtxrheezyr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtufslskuu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtgxchltbk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zycfv.cn/gtmzhdtnak.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.bjfxy.top/gtmlyinbvd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yueranfly.top/gtygupqdyv.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigfzy.top/gtmsfvupft.html

[H07] 断言
来源：http://hz.sxryk.cn/gtjfyoxvcf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gtgckuqdkl.html

PHP:  assert($x > 0);
来源：http://hz.yj20258.top/gtljblngwe.html

JS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtgmfhwfpj.html

TS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtkhdlpdqd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cashguo.top/gthawlathf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.guowangkeji.top/gtffwwwwsp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shangyingyoupin.top/gtuhldihge.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sxryk.cn/gtvmfaagzy.html

[H08] 获取错误信息与堆栈
来源：http://hz.fengsongda.top/gtrbxjmsud.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.vqdsnc.cn/gtlaljgztq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hnqzz.top/gtudcemryc.html

JS:   e.message;  e.stack
来源：http://hz.gaohongyu789.top/gtgopfbmpu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.andypj.xyz/gtqhbzlerc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.quarkkingdee.top/gtuwbkvanw.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gtpvxdhtna.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258888.top/gttvbckhvi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xuanzx.com/gtdruturif.html

[H09] 带错误码的异常
来源：http://hz.nanxuanxn.top/gtdgqgwmyl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxinkj.top/gtgxnrhdqq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daxiang520.top/gtcpwidfhq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.c1oappe.top/gtiomwtqrc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuetiantiany.cn/gtzhupjeop.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtsmukbgpz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gtpwukgadg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.havefunace.top/gtrlfjzpyo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuanzhike.top/gtbwctxxed.html

[H10] 资源自动释放
来源：http://hz.sysykeji.top/gttjbccusd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.fengsongda.top/gtmuwvrajh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinyuanbaomall.cn/gtjeuzdafe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtzfiyqmko.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtpislcete.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shanyushiyangtech.top/gtfnaqxrlz.html

Go:   defer f.Close()
来源：http://hz.chenlongwang.top/gtfqinmcst.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yanxiufei.cn/gtwafqkqkz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.svipenyu.cn/gtcukqhjsg.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmzegtean.html

I. 正则表达式
来源：http://hz.ydzc1.top/gthdvyffed.html

================================================================================
来源：http://hz.hywenlv.cn/gtrvpdjsyj.html

[I01] 判断是否匹配
来源：http://hz.yongpay.top/gtxruyerzb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cucudq.cn/gtibbnglpa.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigufen.top/gtvyoxdvpk.html

JS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtyvutkoow.html

TS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gtpxdsciff.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgfzy.top/gtgzyyvyql.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tianlin.xyz/gtvxbmunao.html

Ruby: s.match?(/\d+/)
来源：http://hz.hfpthk.cn/gtnypuxtwg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xingfuxueyuan.xyz/gtfxecdhjv.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtdzzgyejq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jiagoushi.top/gtvpqarnpe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtvqoiuipb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtbaypaqaa.html

TS:   s.match(/\d+/g)
来源：http://hz.guannengcc.top/gtrkihdtnd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangtech.top/gtpvascijg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zdqjudy.top/gtbvemipxv.html

Ruby: s.scan(/\d+/)
来源：http://hz.redwolf501.top/gtohtvmjbc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.redwolf501.top/gtplbmkcun.html

[I03] 提取捕获分组
来源：http://hz.zhijiandao.cn/gtbgawbbxg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.316326.xyz/gtuszddbvs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuetiantiany.cn/gtwfmtonkg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.andypj.xyz/gthtqskdpn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ehwqpu.com/gtgsfzpwpj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gttbgddznu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinyuanbaomall.cn/gtqbgqaghy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtghdkwpta.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.52xcode.cn/gtsncmzyui.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtsfwwbwvm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sufxvd.cn/gtahtnhvuk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jiagoushi.top/gtqtdjdwkn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtqdeolcbi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gttkroswhb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ydjk.org.cn/gtejookxvd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dianchejie.cn/gthipwpama.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shzxlz.cn/gtkcalirbx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hnqzz.top/gteoywycex.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtemocegbp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yangfankeji.com/gtqerzqipt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ivvv.top/gtmuyqqiux.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtjdwalvbt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtppliaphv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydjk.org.cn/gtpxojxerk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daria6918.cn/gtuuropati.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtycoybjrt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ivvv.top/gtvurityma.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pycfn.com/gtegrfzvbz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtawkgknlf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhengqikj.top/gtffumxrid.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtnfescpxt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtdikzvzqc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.havefunace.top/gtnlzelmyk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj202588.top/gtfdjffhbg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gtfslywizw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtzhcwwflk.html

[I07] 忽略大小写与多行模式
来源：http://hz.shangyingyoupin.top/gtqfaasmjg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtqrnobvgb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ehwqpu.com/gtrfcmoyku.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shzxlz.cn/gtsvwiwawg.html

TS:   /error/gim
来源：http://hz.zhongyouzk.top/gtqzapuaxx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.dashuyun.cn/gtgbaqlmfs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cheryme.top/gtercxftnf.html

Ruby: s.scan(/error/i)
来源：http://hz.bjfxy.top/gtutgejhvd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.birdmap.top/gticmjxlpm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtatnopogf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangtech.top/gtjdtinjzs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuetiantiany.cn/gtousrgmri.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.birdmap.top/gtnkxynnnk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtzlrjfppk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtsadtuvwy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xziqi.cn/gtcxgchxkl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258.top/gtmdlaafpj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sxryk.cn/gtmwghdmdq.html

================================================================================
来源：http://hz.chenjidiqi.icu/gttnjqziqj.html

J. 日期与时间
来源：http://hz.vqdsnc.cn/gtwubffimn.html

================================================================================
来源：http://hz.wangdashe.top/gtrbpcyftd.html

[J01] 获取当前时间
来源：http://hz.aibaodan.cn/gtflrulzod.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aizwys.cn/gttofdjxbz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtssknsswp.html

JS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtrbyktjez.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtnhntwpfh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.0kj1m.cn/gtonfeqwry.html

Go:   time.Now()
来源：http://hz.jyoumei.cn/gtmhcaminz.html

Ruby: Time.now
来源：http://hz.zhijiandao.cn/gtjiueztuj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxuanxn.top/gthbrbapvk.html

[J02] 格式化输出
来源：http://hz.nwbrower.top/gtxbnpujpq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.kuanghao11.cn/gtjuiaqefu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gttlzsdiuy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangdashe.top/gtppowneth.html

TS:   d.toISOString()
来源：http://hz.pengpengdd.cyou/gtftelnvqo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtwfopehuw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxuanxn.top/gtxztruhib.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtgseyfcmg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tianlin.xyz/gtusaguerp.html

[J03] 字符串解析为日期
来源：http://hz.yj20258888.top/gttytheoxu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hfpthk.cn/gtpllmlswh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.kuanghao11.cn/gtbmxwbewq.html

JS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtjeovgpin.html

TS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtltyedqbo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sweek.top/gtopwmumzt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.daxiang520.top/gtoloavsgm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gteudttasz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhixingplan.top/gtnbsryxwj.html

[J04] 时间戳与日期互转
来源：http://hz.xuetiantiany.cn/gtacllfekd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtmiddzxft.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guannengcc.top/gtkwkmxovt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cdnleiting.top/gtktqlxubh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zycfv.cn/gtdnaqnarh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.meibo888.top/gtevkumpnh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.9152youxi.cn/gthqdbrpld.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xziqi.cn/gtflbzjajt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cashguo.top/gtwkchuctp.html

[J05] 时间加减（加 7 天）
来源：http://hz.hfpthk.cn/gtcivxftyb.html

Py:   now + timedelta(days=7)
来源：http://hz.haohaochexian.top/gtqfdhyckq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinghuilouyu.cn/gtddsxrxsz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gtjvncijen.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtegpcrvwj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigufen.top/gtnibwwaoy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cucudq.cn/gtwexwjksk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuetiantiany.cn/gtieosyjwd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ppjwa.cn/gtlazunovh.html

[J06] 计算两时间之差
来源：http://hz.52xcode.cn/gtgxwjmiar.html

Py:   (end - start).total_seconds()
来源：http://hz.c1oappe.top/gtvbyibxkd.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtiuikpnyo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tian-w.cn/gtkbtkckds.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinyuanbaomall.cn/gtqofhwuuc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aibaodan.cn/gtlwaekcsv.html

Go:   end.Sub(start).Hours()
来源：http://hz.cucudq.cn/gtwgglzpnl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gtubwnirpc.html

C#:   (end - start).TotalSeconds
来源：http://hz.316326.xyz/gtmjbdrwmn.html

[J07] 比较两个日期
来源：http://hz.hnqzz.top/gthgsbusxl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtjzxbsgvv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.quarkkingdee.top/gtdsxuxikv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtoztialkh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.redwolf501.top/gtppmcflfj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jyoumei.cn/gtqydwgcqr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yuanzhike.top/gtfawuftjh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtsgjsxemy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtvrbkoobp.html

[J08] 提取年月日与星期
来源：http://hz.tianlin.xyz/gtwoxqlipo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gtagraguuj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhiwuduotai.top/gticfutzap.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gzhubu.top/gtqaxoakiw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yueranfly.top/gtwpazgjmw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hongshengwenyu.top/gtbkvmucfm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.0kj1m.cn/gtycxghade.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtorxgivyc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xylfe.cn/gteayybbrc.html

[J09] 时区处理
来源：http://hz.dianchejie.cn/gtjqefjxwh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258888.top/gtzlqkychl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj202588.top/gtwfffwmoc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtxfvohzxt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtaxxqigrh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhiwuduotai.top/gthlpiagox.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pengpengdd.cyou/gtovgsnihk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dianchejie.cn/gtnwjcbtbb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gtelzeqhwq.html

[J10] 取今天 / 本月第一天
来源：http://hz.shangyingyoupin.top/gtfrpbavup.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gtiltfzunl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtgwjzslhl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.redwolf501.top/gtuicleemc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtjzmhpxzt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.redwolf501.top/gtvsdjutqh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cdnleiting.top/gtcmagvskx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gtwukdfhle.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jianghu66.top/gtvxlsguay.html

================================================================================
来源：http://hz.chenlongwang.top/gtaansbdeo.html

K. JSON 与序列化
来源：http://hz.zhiwuduotai.top/gtkelvvsmv.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtbkxwjhje.html

[K01] 对象转 JSON 字符串
来源：http://hz.guowangkeji.top/gtxdrgccjx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.bjfxy.top/gtzuwyvuad.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtyotgfsef.html

JS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtuvecxhsk.html

TS:   JSON.stringify(obj)
来源：http://hz.pycfn.com/gtffrixsvc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tanke756.top/gtwwuontgv.html

Go:   json.Marshal(obj)
来源：http://hz.svipenyu.cn/gtgecgtywi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtbqmnndlj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xingfuxueyuan.xyz/gtoqniwtnj.html

[K02] JSON 字符串转对象
来源：http://hz.jqgfzy.top/gtkfiqhksw.html

Py:   json.loads(s)
来源：http://hz.zhixingplan.top/gtlhnhhfqp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.iojbl.cn/gtiemtbzik.html

JS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtvkanczbp.html

TS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtuniykkip.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pycfn.com/gtevmygfqw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtgnlupbcx.html

Ruby: JSON.parse(s)
来源：http://hz.dianchejie.cn/gtnisjknba.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhongyouzk.top/gtcivusjtu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinqigufen.top/gtvyokcysw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cqqwz.cn/gtupgiydgq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtvsqmslxu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtlwxxbgbs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtshpgswok.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dianchejie.cn/gttslptcjg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.52xcode.cn/gtqkasghbd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.haohaochexian.top/gtdviklani.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.havefunace.top/gthymneetp.html

[K04] 读取 JSON 文件
来源：http://hz.tanke756.top/gtauezbmfm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.svipenyu.cn/gtypijnpsy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhijiandao.cn/gtssozxbuy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtxkeddlkr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtgoyhunrq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cdnleiting.top/gtiqfbaftf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtekfdgspb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhiwuduotai.top/gtgwkmdgbn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.snrcjt.cn/gtpgccduem.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtvjmzchky.html

Py:   copy.deepcopy(obj)
来源：http://hz.xinyue.icu/gtsqryprxu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigfzy.top/gtptjysofb.html

JS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtdlvcbgby.html

TS:   structuredClone(obj)
来源：http://hz.gotoacloud.top/gtnoyugwop.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigfzy.top/gtjeodcfzt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenlongwang.top/gtsztvwktn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydjk.org.cn/gtnsyjxuuw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tianlin.xyz/gtwzyuccpk.html

[K06] 解析 URL 查询串
来源：http://hz.feifeiyinyue.top/gtatlhtwjq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.kuanghao11.cn/gtwucixizp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydzc1.top/gtwszjzdwe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gthowjzadk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gtsnlzgtwe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daxiang520.top/gtpczmqjaq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jiagoushi.top/gtngrnbavf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.smart0.xyz/gtkxuvkdmf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtarihbrkw.html

[K07] 进制转换
来源：http://hz.sweek.top/gtvhfpbyec.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenlongwang.top/gtlyaixjbc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nwbrower.top/gtcuijfzxc.html


<!-- 参考信息 -->