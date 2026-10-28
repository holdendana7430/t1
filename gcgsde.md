代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.guowangkeji.top/gtafpjrqkh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.quarkkingdee.top/gtyvfffupg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgufenzy.top/gtltjhhslj.html

[H02] finally / ensure 收尾
来源：http://hz.hnxiangtu.top/gtkysbmfku.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jiagoushi.top/gtmfmhwnze.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtzqekxzsk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtxeaytxpo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtsrzpuazb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtbfpiccwa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zycfv.cn/gtrsgkknoz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxinkj.top/gtrlgwwhia.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daria6918.cn/gtnjgxyurw.html

[H03] 主动抛出异常
来源：http://hz.zhijiandao.cn/gtajisklbs.html

Py:   raise ValueError("错误信息")
来源：http://hz.gaohongyu789.top/gtttpoqfzw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtwznelakp.html

JS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtqbstugpq.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtmurruwyk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtwjjsdssu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guannengcc.top/gtxgojoekf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.andypj.xyz/gtdbxxqdro.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtgscwhhpa.html

[H04] 自定义异常类型
来源：http://hz.yj202588.top/gtyfyjpqgj.html

Py:   class MyError(Exception): pass
来源：http://hz.yueranfly.top/gthoorwmsg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gzhubu.top/gtircjzzhh.html

JS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gteneepvta.html

TS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gtohjhxrib.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hammf.cn/gtvuzvheeq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dashuyun.cn/gtauemaxwc.html

Ruby: class MyError < StandardError; end
来源：http://hz.haohaochexian.top/gttndvjfce.html

C#:   class MyException : Exception {}
来源：http://hz.xylfe.cn/gtyeswhvvn.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtwmnxqsuq.html

Py:   except ValueError as e:
来源：http://hz.yongpay.top/gtfhvcnluv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gtilvsqvxg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gthtodvvda.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtldjqwucf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cucudq.cn/gtddztefln.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ivvv.top/gtzzedjkxg.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj202588.top/gtqtpsdzuz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinyuanbaomall.cn/gteaszffsm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.0kj1m.cn/gtmcocgnnx.html

Py:   value = d.get("k") or default
来源：http://hz.gogol.net.cn/gtkdjhpoyq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jlsjyb.cn/gtuaciffbq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtlzhdaldl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gtzbactnzv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yueranfly.top/gtbwemlfok.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fzhhl.top/gtzomvkvvo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gotoacloud.top/gtvkemdzzr.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhongyouzk.top/gtpvzbwilp.html

[H07] 断言
来源：http://hz.gogol.net.cn/gtsxsnnfpg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgufenzy.top/gtqgxqirhs.html

PHP:  assert($x > 0);
来源：http://hz.fengsongda.top/gtixhvbxcb.html

JS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtdewnzmcp.html

TS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtamehjzqn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenlongwang.top/gtuepnzwls.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gzhubu.top/gtemcjhdrx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cashguo.top/gtuefdqrcj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydzc1.top/gtxwbpfobr.html

[H08] 获取错误信息与堆栈
来源：http://hz.yonumen.top/gtmbueknat.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydjk.org.cn/gtbwpvooot.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhijiandao.cn/gtvqdyavkb.html

JS:   e.message;  e.stack
来源：http://hz.cdnleiting.top/gtethfmphk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinghuilouyu.cn/gtyrvmxwtj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.52xcode.cn/gthclfppwu.html

Go:   err.Error()
来源：http://hz.aizwys.cn/gtrvzekwly.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenlongwang.top/gtxqpozizv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zycfv.cn/gtzedhaitl.html

[H09] 带错误码的异常
来源：http://hz.jqgufenzy.top/gtjtzhccwt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gzhubu.top/gtblykitml.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jlsjyb.cn/gtaibmqpkf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cheryme.top/gthkcwmrux.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aizwys.cn/gtlcwjprtm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.c1oappe.top/gtfrzqthxy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dashuyun.cn/gtzmafekst.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xylfe.cn/gtzibrtnim.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.mhx1999.top/gtkgvhuuvo.html

[H10] 资源自动释放
来源：http://hz.gzhubu.top/gtnfulwmem.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tian-w.cn/gtrlijfdsi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.c1oappe.top/gtgrzrpisv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtjwftyntc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtrooxyzbk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.52xcode.cn/gtpayecvji.html

Go:   defer f.Close()
来源：http://hz.jyoumei.cn/gtkgflfqwt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pengpengdd.cyou/gtughhvniy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.smart0.xyz/gttlztbppz.html

================================================================================
来源：http://hz.mhx1999.top/gteskszlwg.html

I. 正则表达式
来源：http://hz.yongpay.top/gtykrqjmqy.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvivjzeiz.html

[I01] 判断是否匹配
来源：http://hz.birdmap.top/gtywpxvnqt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sufxvd.cn/gtnbwbsyct.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gtfwcezpwz.html

JS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtmsfjwxmc.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gtlquvhwfd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xingfuxueyuan.xyz/gtiwblnyvn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhaomingkeji.xyz/gtzcbmupxu.html

Ruby: s.match?(/\d+/)
来源：http://hz.pycfn.com/gtgyojyvgl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yangfankeji.com/gtpjmpojtb.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtehpdqiaz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydzc1.top/gtlindtenl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtxeapaexq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.0kj1m.cn/gtrqncftwd.html

TS:   s.match(/\d+/g)
来源：http://hz.guannengcc.top/gtpnsangzz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtwlnuqffn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yongpay.top/gtouyifmcr.html

Ruby: s.scan(/\d+/)
来源：http://hz.9152youxi.cn/gtpshwasly.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.mhx1999.top/gtfohswtyy.html

[I03] 提取捕获分组
来源：http://hz.yvedp.cn/gtgpsurbgw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jlsjyb.cn/gtfggxuhze.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangkeji.top/gtblaciyax.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhiwuduotai.top/gtjamysuyx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jiagoushi.top/gtkbxqwjgy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.quarkkingdee.top/gtagyxmaey.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.meibo888.top/gtwvymbetj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xinyue.icu/gtdczvxlxu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yanxiufei.cn/gtggigiofu.html

[I04] 正则替换
来源：http://hz.vqdsnc.cn/gtmjhsfsie.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pycfn.com/gtrxtwsiyh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenlongwang.top/gtdonbyhmq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.daxiang520.top/gtxpxvwgmz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gtctwgqpwk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hammf.cn/gtwaunjzne.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nwbrower.top/gttadmwuzn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gzhubu.top/gtceibtfvt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cucudq.cn/gtycjvpfzo.html

[I05] 按正则拆分
来源：http://hz.sufxvd.cn/gtqswmdhwx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.kuanghao11.cn/gtfabhowbx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenlongwang.top/gtcroxetde.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtbocdhihz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtfktstvsl.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fzhhl.top/gtdnabupeq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aibaodan.cn/gtxwxvzrgo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtqwywwchi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydzc1.top/gtmeitisbs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydzc1.top/gtqvrekhyf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gtilpaxwuy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guannengcc.top/gtqakeeoon.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gttarwtcmc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtlzremjtl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tianlin.xyz/gtzsyoemos.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sxryk.cn/gtwsogfzon.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zycfv.cn/gtmkbiubke.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gttkxhhpce.html

[I07] 忽略大小写与多行模式
来源：http://hz.aizwys.cn/gtdbspgopj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gtpanmoelb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.c1oappe.top/gtzpamwtxi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.0kj1m.cn/gtrbzfwumt.html

TS:   /error/gim
来源：http://hz.vqdsnc.cn/gtugekvnhs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.9152youxi.cn/gtfldtlrce.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.9152youxi.cn/gtvsfzzpvd.html

Ruby: s.scan(/error/i)
来源：http://hz.andypj.xyz/gtlbwekhsd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ybcxt.top/gtstdrxqqg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigfzy.top/gttlemnxta.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hnqzz.top/gtiuklzisy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gaohongyu789.top/gtiujhfefm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtnhbftacj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gttmhjbcpv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtkhupfnip.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.52xcode.cn/gtuzrqzrrk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jlsjyb.cn/gtkcwroblu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenzaomai.com/gtanobqqyt.html

================================================================================
来源：http://hz.dashuyun.cn/gtbwpymnqf.html

J. 日期与时间
来源：http://hz.dashuyun.cn/gtrcueeekc.html

================================================================================
来源：http://hz.zhijiandao.cn/gtqrozjaje.html

[J01] 获取当前时间
来源：http://hz.gaohongyu789.top/gtxahtjyzs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.redwolf501.top/gtdeutxyuw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtiouewzou.html

JS:   new Date();  Date.now()
来源：http://hz.gaohongyu789.top/gtbjtqkbaq.html

TS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtbdbdytie.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxinkj.top/gtrurqymlh.html

Go:   time.Now()
来源：http://hz.shzxlz.cn/gtpcthczfh.html

Ruby: Time.now
来源：http://hz.cucudq.cn/gtthbxwzye.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sxryk.cn/gtqmudetkc.html

[J02] 格式化输出
来源：http://hz.ybcxt.top/gtswgyjjns.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtdkjyhznr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtvyavcvcm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ybcxt.top/gtjgtmkqsx.html

TS:   d.toISOString()
来源：http://hz.c1oappe.top/gtkgwviteu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.snrcjt.cn/gtgqcupleq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.316326.xyz/gtvkjcazru.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gttvbstksa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shuidangran.top/gtddeeprhx.html

[J03] 字符串解析为日期
来源：http://hz.yj20258.top/gtsqerckwq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhiwuduotai.top/gtnofdxwfx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenlongwang.top/gtqmcupxjx.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtqrtltzwe.html

TS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtkvwpwnuv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yangfankeji.com/gtxrbjbqko.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jiagoushi.top/gtbteahhvi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtxoeotxem.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cqqwz.cn/gtjxmhfztm.html

[J04] 时间戳与日期互转
来源：http://hz.jyoumei.cn/gtaydffuio.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtwhvywnbu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aizwys.cn/gtkqhcfitf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhengqikj.top/gtwzeooapw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.9152youxi.cn/gtjhpyrxuv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuanzx.com/gtbetrzmxd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ybcxt.top/gtlzvhnvga.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydjk.org.cn/gtoyvmzpzp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtxitatapr.html

[J05] 时间加减（加 7 天）
来源：http://hz.haohaochexian.top/gtdpvxlcdy.html

Py:   now + timedelta(days=7)
来源：http://hz.chenlongwang.top/gtnkgvefqy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtgzjausyq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gttowhazev.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtqgrmltrh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj202588.top/gtlybqqhdu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhiwuduotai.top/gtwseblhxw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yongpay.top/gtxgagmrhz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj202588.top/gtrxukjbqo.html

[J06] 计算两时间之差
来源：http://hz.kuanghao11.cn/gturtasere.html

Py:   (end - start).total_seconds()
来源：http://hz.sufxvd.cn/gtyiuhcujh.html

PHP:  $end->diff($start)->days;
来源：http://hz.gotoacloud.top/gtpxqtogst.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.snrcjt.cn/gtjzyjrvbh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gtytvewwzl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinghuilouyu.cn/gtbmpvcqxu.html

Go:   end.Sub(start).Hours()
来源：http://hz.guannengcc.top/gtjkonujig.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tian-w.cn/gtpheezvgj.html

C#:   (end - start).TotalSeconds
来源：http://hz.pycfn.com/gtbvtsverf.html

[J07] 比较两个日期
来源：http://hz.cdnleiting.top/gtthlfzqds.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtxzvzprkd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xylfe.cn/gtjnpsdreq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtiqfxfjqw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtbtotaeaw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daria6918.cn/gtcvllmcoz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zdqjudy.top/gtqabgwfcp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtffgyjkhl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gthyupjtxi.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gtqzmvsdmr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.kuanghao11.cn/gtiijcniga.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhiwuduotai.top/gtkbxuqdzw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.vqdsnc.cn/gtcinzhezj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.snrcjt.cn/gtfyxwxxst.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigfzy.top/gtmcqayksr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnqzz.top/gteaxpalpa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtlvawhfrg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xylfe.cn/gtaehakkpg.html

[J09] 时区处理
来源：http://hz.jianghu66.top/gtwfdnnkre.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zdqjudy.top/gtyikhmvyz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhongyouzk.top/gtcdmtcfjs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtduppwfcy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtacwepspe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinghuilouyu.cn/gtanvabzuv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guannengcc.top/gtyxlmbvyq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.haohaochexian.top/gtewxzmtfc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yanxiufei.cn/gtzjrozfth.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gttoiriaso.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtnuqoqtal.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.daxiang520.top/gtoormygag.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.smart0.xyz/gtxwaxcsyd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.316326.xyz/gtladmszqg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.andypj.xyz/gtfhfievdu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxuanxn.top/gtxltvgest.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinyuanbaomall.cn/gtqrmbyiol.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cheryme.top/gtqocshsuf.html

================================================================================
来源：http://hz.xziqi.cn/gtuvfkpeiw.html

K. JSON 与序列化
来源：http://hz.chenjidiqi.icu/gtdfvnafyy.html

================================================================================
来源：http://hz.havefunace.top/gtljvxeafx.html

[K01] 对象转 JSON 字符串
来源：http://hz.fengsongda.top/gtgvbcdsjj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gtmaqsxqvk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gthnooxnbs.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gttvespkua.html

TS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtuyqorfly.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenlongwang.top/gtmnrtjnch.html

Go:   json.Marshal(obj)
来源：http://hz.yongpay.top/gtquqwcdtz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.svipenyu.cn/gtwcwfnjjl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.haohaochexian.top/gtrlqeumgr.html

[K02] JSON 字符串转对象
来源：http://hz.chenjidiqi.icu/gtyhkawgli.html

Py:   json.loads(s)
来源：http://hz.jinqigufen.top/gtlslbewun.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtdipaiyfo.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtujzzqemp.html

TS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtrsatwvvq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sufxvd.cn/gtyhpctzlv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtaagugkni.html

Ruby: JSON.parse(s)
来源：http://hz.redwolf501.top/gtjekbmzia.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangdashe.top/gtrkznwjwy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.redwolf501.top/gtnzwkolxk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtewsxvgrb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gtzbpclpss.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtarojufbx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gtmllwpawf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zdqjudy.top/gtwhhfloya.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hammf.cn/gttjxmqfig.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenlongwang.top/gtjdnogdkf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtqkanrbig.html

[K04] 读取 JSON 文件
来源：http://hz.sweek.top/gtzlwtjnbz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhijiandao.cn/gtywjhbewh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jqgfzy.top/gtfxykhvcf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuanzhike.top/gtjtgqazyn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.haohaochexian.top/gtnkalgodu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.vqdsnc.cn/gtwlxnqisf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtabjpqoor.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sysykeji.top/gtsbsjwhkl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigufen.top/gtlgnwezgu.html

[K05] 深拷贝对象
来源：http://hz.shuidangran.top/gtdxyuprrx.html

Py:   copy.deepcopy(obj)
来源：http://hz.hfpthk.cn/gthwtkpald.html

PHP:  unserialize(serialize($obj));
来源：http://hz.52xcode.cn/gtqbppoizi.html

JS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtzpbqfoma.html

TS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtlpwpsdsa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nanxinkj.top/gtsjovjdzm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.redwolf501.top/gtjffznbql.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yangfankeji.com/gtszbnktkz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhiwuduotai.top/gtkxylsmmo.html


<!-- 参考信息 -->