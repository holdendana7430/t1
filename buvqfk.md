代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtqcvmzrbv.html

[H04] 自定义异常类型
来源：http://hz.xziqi.cn/gtsrjgzjhi.html

Py:   class MyError(Exception): pass
来源：http://hz.jiagoushi.top/gtciaphods.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pengpengdd.cyou/gtxuetofcs.html

JS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtedctscev.html

TS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtdzekgiga.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtqdvxjjki.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.52xcode.cn/gtslpcncej.html

Ruby: class MyError < StandardError; end
来源：http://hz.dianchejie.cn/gtqdfmggtg.html

C#:   class MyException : Exception {}
来源：http://hz.xuanzx.com/gtrulodlqw.html

[H05] 捕获特定类型
来源：http://hz.shuidangran.top/gtvwbzdhhw.html

Py:   except ValueError as e:
来源：http://hz.c1oappe.top/gtjsaforxt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gzhubu.top/gtfyjkcwtz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtknekxany.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.meibo888.top/gtgkpbhzuk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhixingplan.top/gtsxorrrdk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ywan-chungtsiang.top/gtmbjqwuck.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtsirhyqaz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtkxkdxscp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.birdmap.top/gthxjmdnxi.html

Py:   value = d.get("k") or default
来源：http://hz.yangfankeji.com/gttwrlxufa.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtopquxuhw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtxrtgqmbo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gthpfoumje.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.quarkkingdee.top/gtcdkrkjwz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jiagoushi.top/gtnzdwwcoa.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jlsjyb.cn/gtguttubph.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gtrjyzicpx.html

[H07] 断言
来源：http://hz.tanke756.top/gtpizhsmce.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtfdcmzvya.html

PHP:  assert($x > 0);
来源：http://hz.birdmap.top/gthjgfjfze.html

JS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtmsidpxef.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtyhenzjpd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hammf.cn/gtdnfxvpbx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cucudq.cn/gttvvkzdjj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtweouzdjk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xziqi.cn/gtaoimpbns.html

[H08] 获取错误信息与堆栈
来源：http://hz.jianghu66.top/gtasutqrxu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yanxiufei.cn/gtsrtoxcmc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gogol.net.cn/gtskcoqqbf.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gtsxutbwfv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sxryk.cn/gtofmqjpmq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xingfuxueyuan.xyz/gtacbuqfbh.html

Go:   err.Error()
来源：http://hz.zdqjudy.top/gtndizmwrh.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenlongwang.top/gtrwpwitzx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shuidangran.top/gtkplipngx.html

[H09] 带错误码的异常
来源：http://hz.tianlin.xyz/gtoxozakip.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.andypj.xyz/gtyscateid.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnxiangtu.top/gtlrnxhurf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shzxlz.cn/gtrzwndmgg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgfzy.top/gtdhtcpntj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fzhhl.top/gtteafpzwd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.mhx1999.top/gtsujihdeh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sufxvd.cn/gtjosuzhkt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yangfankeji.com/gtunhqsbqh.html

[H10] 资源自动释放
来源：http://hz.cucudq.cn/gtvhooxbbm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtvhkvemaf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xingfuxueyuan.xyz/gtmnpcwcci.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtifkbicjf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtpqxnssci.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zdqjudy.top/gtwsjdisen.html

Go:   defer f.Close()
来源：http://hz.9152youxi.cn/gtrhcabveg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yanxiufei.cn/gtxtsoewnr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigufen.top/gtxivbxxxf.html

================================================================================
来源：http://hz.zhixingplan.top/gtjnpldnhm.html

I. 正则表达式
来源：http://hz.ydzc1.top/gtlkcphfzh.html

================================================================================
来源：http://hz.guowangkeji.top/gtsmucrnhe.html

[I01] 判断是否匹配
来源：http://hz.cdnleiting.top/gtfedtozxh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenzaomai.com/gtnzuddzow.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenzaomai.com/gtigjqmnuy.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtpmgpvsax.html

TS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtlctujsgd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.vqdsnc.cn/gtloqzjpdp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yongpay.top/gtjxbkwuog.html

Ruby: s.match?(/\d+/)
来源：http://hz.pycfn.com/gtmsvvgwki.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gaohongyu789.top/gtjquitkpa.html

[I02] 提取所有匹配
来源：http://hz.jqgfzy.top/gtputzygmd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.haohaochexian.top/gtylqkalmd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cqqwz.cn/gtqkadugjo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sweek.top/gtybmsvobj.html

TS:   s.match(/\d+/g)
来源：http://hz.chenjidiqi.icu/gtlkrnmasi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ywan-chungtsiang.top/gtkslnyywv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tian-w.cn/gtkabpsbbq.html

Ruby: s.scan(/\d+/)
来源：http://hz.xziqi.cn/gtwmicypww.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.fengsongda.top/gtvaynyzmv.html

[I03] 提取捕获分组
来源：http://hz.jqgfzy.top/gtsyefcgvc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.kuanghao11.cn/gtgnjymptv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ywan-chungtsiang.top/gtdujechcn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cqqwz.cn/gtwsmooylv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangkeji.top/gtpyduizcn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.52xcode.cn/gtbqhiyomq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sufxvd.cn/gtllnauoxe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtfpilmqyc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenlongwang.top/gtbywjpzje.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gthupbcfhj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.mhx1999.top/gteggbkkqv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangtech.top/gthaixlatz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtxhgthbqr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtcvgwowjb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhoulong.xyz/gtcjqyhtgn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.quarkkingdee.top/gtvmpqdazs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnxiangtu.top/gtvnvlukgo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.c1oappe.top/gtuqymknyn.html

[I05] 按正则拆分
来源：http://hz.kuanghao11.cn/gtjhesnkod.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuanzx.com/gtvywqefsh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgufenzy.top/gtsxyeerjh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtovcnsbga.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gthmljexlw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.haohaochexian.top/gtxfbpelrb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gotoacloud.top/gtqfkdxdim.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtibuuseym.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yongpay.top/gtcgkopccp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xingfuxueyuan.xyz/gtpyezxdgf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtwzjicsdy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.birdmap.top/gtlmttsvcd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtqdxyqtas.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenlongwang.top/gtrfqqlxvf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jianghu66.top/gtmrfvfgvh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhixingplan.top/gtcctzjcjs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jiagoushi.top/gtdrbmspee.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gtugcoagdy.html

[I07] 忽略大小写与多行模式
来源：http://hz.jyoumei.cn/gtulxkefpi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shangyingyoupin.top/gtweadjbti.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtjbkcuaya.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jyoumei.cn/gtuokxalvx.html

TS:   /error/gim
来源：http://hz.andypj.xyz/gtltndjvpg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shzxlz.cn/gtbhdzedtd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.guowangkeji.top/gtncqhhnen.html

Ruby: s.scan(/error/i)
来源：http://hz.yangfankeji.com/gtwfolshuo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tanke756.top/gtztmwiixs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtogjukgeo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yvedp.cn/gtfrzkfvxj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yonumen.top/gtlevterft.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtchatjpwr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtzdohkeeb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xylfe.cn/gtfxrqwfpi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.c1oappe.top/gtuoyxsltr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ydzc1.top/gtzgkdizms.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtqppacyqh.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtaztpyrsl.html

J. 日期与时间
来源：http://hz.redwolf501.top/gtwlrvryip.html

================================================================================
来源：http://hz.svipenyu.cn/gtwzrwenpe.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtopgyunah.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhiwuduotai.top/gtwrvmwaev.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtnugkhicm.html

JS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtppdbzouc.html

TS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtwmpqcbks.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.52xcode.cn/gtfidnbien.html

Go:   time.Now()
来源：http://hz.iojbl.cn/gtkzrznziw.html

Ruby: Time.now
来源：http://hz.jinqigfzy.top/gtqvrsrfyg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.vqdsnc.cn/gtcmybfabh.html

[J02] 格式化输出
来源：http://hz.dashuyun.cn/gtvndtwzaj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtmpbmkqiq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gthaynqeei.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xziqi.cn/gtvnlfpljp.html

TS:   d.toISOString()
来源：http://hz.yueranfly.top/gtblwgvwmk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jiagoushi.top/gtxxibmkha.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xuetiantiany.cn/gttryjacse.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtlihgjbcs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yuxming.cn/gtphwbzfxk.html

[J03] 字符串解析为日期
来源：http://hz.zhongyouzk.top/gtdtbdsrbg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xingfuxueyuan.xyz/gtxcmwofct.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aibaodan.cn/gtsuyuwzcs.html

JS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtnxrcoqol.html

TS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtwtefxuxa.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtsivgsxwr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigufen.top/gtopgqywre.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtvlfrjyyo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cashguo.top/gtodogrfjp.html

[J04] 时间戳与日期互转
来源：http://hz.xuanzx.com/gtbdjexqsg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daria6918.cn/gticzfyfiu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cashguo.top/gtznpsyrgt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xingfuxueyuan.xyz/gtytjsbabp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinyuanbaomall.cn/gtfzlmwmls.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangtech.top/gtvbavtyfe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.smart0.xyz/gtkwayixrs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.svipenyu.cn/gtqhpfolgb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yangfankeji.com/gtkrzkexqh.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinqigfzy.top/gtglcaamsr.html

Py:   now + timedelta(days=7)
来源：http://hz.cqqwz.cn/gthoamszxa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhijiandao.cn/gthjbvtwav.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yongpay.top/gtdhmzyvbg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtupcbnoys.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ybcxt.top/gtsjnddcwm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnqzz.top/gtvomgxifr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258888.top/gtprznodpn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.birdmap.top/gtonjjlddw.html

[J06] 计算两时间之差
来源：http://hz.sxryk.cn/gtqxqivglz.html

Py:   (end - start).total_seconds()
来源：http://hz.tian-w.cn/gthcgknazd.html

PHP:  $end->diff($start)->days;
来源：http://hz.xylfe.cn/gtllguoaog.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hongshengwenyu.top/gtxtkioezf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jianghu66.top/gthhjtvgwm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.vqdsnc.cn/gtnkhilkwu.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuxming.cn/gtbuxzxtns.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fzhhl.top/gtdlnyvshi.html

C#:   (end - start).TotalSeconds
来源：http://hz.aibaodan.cn/gtrzxbkmrw.html

[J07] 比较两个日期
来源：http://hz.xinyue.icu/gtxzqudvnz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtwjgdqkcx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yueranfly.top/gtgytelblf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtozyarigs.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtdhixpdxo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xingfuxueyuan.xyz/gtgwyrtbix.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aibaodan.cn/gtnpvmnloe.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtsbfmkttr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtcbrcrnhe.html

[J08] 提取年月日与星期
来源：http://hz.mhx1999.top/gtcemscktv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xinyue.icu/gtaazxneyf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258888.top/gtlmcfzees.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jiagoushi.top/gthpstsyzg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258888.top/gtffryiqae.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ppjwa.cn/gtaaguseyd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daxiang520.top/gtgzdsylmi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hywenlv.cn/gtaiwcsttw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhengqikj.top/gtbvqhntco.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtpsaqsxqa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.havefunace.top/gtnoiyemtb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ydzc1.top/gtkvsravca.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtazfjiynn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtuaglkmfs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtvizhetgf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinghuilouyu.cn/gtozgzsfhj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhoulong.xyz/gtchpwmpye.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tian-w.cn/gtbjirzbsw.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgufenzy.top/gtjntujjka.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shzxlz.cn/gtmaxdestx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuanzx.com/gteezdsfpk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ehwqpu.com/gtwrbybayw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.feifeiyinyue.top/gtfhzlijxg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sweek.top/gtrvxbmjeb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj202588.top/gtqcnqiteu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigfzy.top/gtxdpdvbot.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydzc1.top/gteiiyliml.html

================================================================================
来源：http://hz.smart0.xyz/gtaxnlxjdi.html

K. JSON 与序列化
来源：http://hz.xuetiantiany.cn/gtugznkdcm.html

================================================================================
来源：http://hz.bjfxy.top/gtdvrfzoii.html

[K01] 对象转 JSON 字符串
来源：http://hz.shzxlz.cn/gtmkhqxufq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gtshzttuds.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtmudkwaxp.html

JS:   JSON.stringify(obj)
来源：http://hz.guannengcc.top/gtgbukrfwd.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gttnpdfnhh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gzhubu.top/gtpzyynigc.html

Go:   json.Marshal(obj)
来源：http://hz.ydjk.org.cn/gtqabdwxlu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hongshengwenyu.top/gtcffjftkd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.havefunace.top/gtwyeiwzen.html

[K02] JSON 字符串转对象
来源：http://hz.shuidangran.top/gtbmmpacbw.html

Py:   json.loads(s)
来源：http://hz.mhx1999.top/gthwcppqvi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tanke756.top/gtjdsvmzcp.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gttardsjeu.html

TS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gtlqfpybvp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.c1oappe.top/gtstefwabc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jianghu66.top/gtphcfuuig.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtrzhiqchi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.birdmap.top/gthfvapysv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhengqikj.top/gtfbtezreo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gttfvwmkpn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtwuytdmjz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtktaixaed.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtfudwkbbl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtxzkzeffa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fengsongda.top/gtrvbkomvy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jianghu66.top/gtykmtzqsz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hfpthk.cn/gtyzihccnk.html

[K04] 读取 JSON 文件
来源：http://hz.gzhubu.top/gteztjtaal.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zdqjudy.top/gtyexkbbcv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuetiantiany.cn/gtqefqzdjs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtanmqsudl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtbjkwsvev.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tian-w.cn/gtrqvvicvh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtizxlyodc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangshuangyany.cn/gtchxkpsjj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.svipenyu.cn/gtvdhukgjy.html

[K05] 深拷贝对象
来源：http://hz.svipenyu.cn/gtzwicjaxc.html

Py:   copy.deepcopy(obj)
来源：http://hz.kuanghao11.cn/gtjyvknjvb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgfzy.top/gtivtpftot.html

JS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtgstrejzx.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtzuproppb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhixingplan.top/gtbzoliqki.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj202588.top/gtbwhavzkl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gteuejefgi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shangyingyoupin.top/gtpmmdofhb.html

[K06] 解析 URL 查询串
来源：http://hz.xuanzx.com/gtawhdxptg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ehwqpu.com/gtpjyfkxil.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xylfe.cn/gtmmzzewrr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtdzkskojk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shangyingyoupin.top/gtcqionxsb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gogol.net.cn/gtzvrqxgwr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gtjxbuashx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dashuyun.cn/gtghxnntmh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtfmmkbuet.html

[K07] 进制转换
来源：http://hz.nanxinkj.top/gtyjbcurjc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.pengpengdd.cyou/gtcceuvvyi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangdashe.top/gtepjsnxhy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gthsklupms.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtjyvzdndg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtbwsuosoh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnxiangtu.top/gtsjmlgsvo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fengsongda.top/gtfcorirsi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jlsjyb.cn/gthcwnptet.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hnxiangtu.top/gtgtsgvlwm.html

Py:   pickle.dumps(obj)
来源：http://hz.gaohongyu789.top/gthubmrhjs.html


<!-- 参考信息 -->