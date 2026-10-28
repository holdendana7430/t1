代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtpqogweze.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.52xcode.cn/gtiejxdoqb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cucudq.cn/gtgtczfcfk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigfzy.top/gtefrztgtc.html

[H03] 主动抛出异常
来源：http://hz.fzhhl.top/gtomcygsud.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenjidiqi.icu/gtrvljyizf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtcggtjmzi.html

JS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtdvpyzmwt.html

TS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gtowqzeahj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtwkeaqcse.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guannengcc.top/gtmwpwijee.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhongyouzk.top/gtxzunybfn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtwypvukiw.html

[H04] 自定义异常类型
来源：http://hz.ppjwa.cn/gtdclvxask.html

Py:   class MyError(Exception): pass
来源：http://hz.redwolf501.top/gtyoowuakf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtymehbjek.html

JS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtbkurukjp.html

TS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtuzvrdelc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cashguo.top/gtcmjbuslz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daxiang520.top/gtfnnnhkxt.html

Ruby: class MyError < StandardError; end
来源：http://hz.iojbl.cn/gtysbzvejc.html

C#:   class MyException : Exception {}
来源：http://hz.meibo888.top/gtndblazup.html

[H05] 捕获特定类型
来源：http://hz.hywenlv.cn/gtqhvaaxko.html

Py:   except ValueError as e:
来源：http://hz.jqgfzy.top/gtuwfwwpko.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.smart0.xyz/gtswfwuphs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtcotitoql.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtpqolflba.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aizwys.cn/gtvsqzmojz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shuidangran.top/gtjcszqwxt.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhijiandao.cn/gtzjezvcvx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guowangkeji.top/gtsohzudtk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zycfv.cn/gtzhbezhfj.html

Py:   value = d.get("k") or default
来源：http://hz.gaohongyu789.top/gtavpbnojm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gtfxuziasd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtzwkarpzf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtfksugson.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shuidangran.top/gtfejwureb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtgkvqwtbx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gthjtsxnjx.html

C#:   obj?.A?.B ?? default
来源：http://hz.guannengcc.top/gtaikuyxvv.html

[H07] 断言
来源：http://hz.tanke756.top/gtgaarxbba.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuanzhike.top/gtjwdatmxu.html

PHP:  assert($x > 0);
来源：http://hz.zhoulong.xyz/gttbgbjkgp.html

JS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtdkeycxrv.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtnhtcucba.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cucudq.cn/gttwxlmuut.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hfpthk.cn/gteocjqcdx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgfzy.top/gttqwkrlpb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtmnrgiymk.html

[H08] 获取错误信息与堆栈
来源：http://hz.jianghu66.top/gtxxedbnwm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtnbguxrkr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zdqjudy.top/gtngwghpnv.html

JS:   e.message;  e.stack
来源：http://hz.wangshuangyany.cn/gtkpuvvime.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sweek.top/gtdvzxqred.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guannengcc.top/gtysaxtfgp.html

Go:   err.Error()
来源：http://hz.52xcode.cn/gtsjwnklmb.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258888.top/gtkbeapejk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.svipenyu.cn/gtkrttpkds.html

[H09] 带错误码的异常
来源：http://hz.xuanzx.com/gtonbfnlyb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.316326.xyz/gtvboqdkts.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.iojbl.cn/gtvroruorc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gteynorici.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gttnwftbvc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jqgfzy.top/gtymmccfon.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuanzx.com/gtnyttewyl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgfzy.top/gtyyckbfgk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hywenlv.cn/gtpogydplo.html

[H10] 资源自动释放
来源：http://hz.tanke756.top/gtynhdwebu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sxryk.cn/gtixghcifm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dianchejie.cn/gtdkolmpuq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtnhwmwwpb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtzktzlmft.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhoulong.xyz/gtkuahpdxf.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gthzuxmjxt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxinkj.top/gtrxplsuvn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.c1oappe.top/gtoghyszvh.html

================================================================================
来源：http://hz.tian-w.cn/gtolksciif.html

I. 正则表达式
来源：http://hz.nwbrower.top/gtcmrxbqge.html

================================================================================
来源：http://hz.zycfv.cn/gtuzwuleat.html

[I01] 判断是否匹配
来源：http://hz.52xcode.cn/gtbivskxoq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tianlin.xyz/gtofmubfet.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gttpfupaae.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtltukzrzz.html

TS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtsjahccdz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtgxdfjabf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gtrofpmcel.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtzyfpzefm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gtpvqjtjcj.html

[I02] 提取所有匹配
来源：http://hz.yj202588.top/gtjwikegqc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shangyingyoupin.top/gtpjrvkhna.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhiwuduotai.top/gtnusfaphh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yvedp.cn/gtiqjhnkly.html

TS:   s.match(/\d+/g)
来源：http://hz.0kj1m.cn/gtpkhpildy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtjpvrksva.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zycfv.cn/gtzitxbfku.html

Ruby: s.scan(/\d+/)
来源：http://hz.cqqwz.cn/gtdqyxgepo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.meibo888.top/gtvjotkvmv.html

[I03] 提取捕获分组
来源：http://hz.jinyuanbaomall.cn/gtacskgxvq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dashuyun.cn/gtoyrsrkjw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gotoacloud.top/gtxliewyac.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.snrcjt.cn/gtdpbgmole.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.kuanghao11.cn/gtvncxkeda.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.0kj1m.cn/gtcxjfrrrn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xuetiantiany.cn/gtsozunyiq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tian-w.cn/gtpocbxmns.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.snrcjt.cn/gtzxkynxlu.html

[I04] 正则替换
来源：http://hz.zycfv.cn/gtbvccdmgd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtkuqebvvy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.andypj.xyz/gtjvysnwpt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gttvhtcczd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gthjilyhsf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yvedp.cn/gtwfzrtavj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuanzx.com/gtkrjwamwb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtqjgspgwe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cucudq.cn/gttqpfngqr.html

[I05] 按正则拆分
来源：http://hz.shanyushiyangtech.top/gthfadlagl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sysykeji.top/gtyfkcflnh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtqvrdhqtj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtglhlzinr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gthmtsmpay.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhengqikj.top/gtbihgoqld.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gtzicgrfsb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtntziqcgi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jiagoushi.top/gtclcntimj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ehwqpu.com/gtmjjzltry.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtyowozufu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangdashe.top/gtsxararjd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gtceeodxdj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtfdtuadsz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.mhx1999.top/gtzignkzqj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daria6918.cn/gtsfmwthgl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daria6918.cn/gtpkbkjves.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuxming.cn/gtkuxqtmta.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhixingplan.top/gtmlbwhedk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhongyouzk.top/gtudmkpyjc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yongpay.top/gtjlbsuslt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.meibo888.top/gtkxpjkdzz.html

TS:   /error/gim
来源：http://hz.tian-w.cn/gtyhaywqqe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pycfn.com/gtjttepmpz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xylfe.cn/gtbyzzmeog.html

Ruby: s.scan(/error/i)
来源：http://hz.havefunace.top/gtslrnwsop.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangdashe.top/gtamhczozj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.iojbl.cn/gtjznamsot.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cashguo.top/gtvhmgeewh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ehwqpu.com/gtlfwsudpp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gtzqwscayo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtixdrzisg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtcefncxxi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangshuangyany.cn/gtrhausnjo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gtwgjwwyee.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ybcxt.top/gtffgtsuyv.html

================================================================================
来源：http://hz.hnxiangtu.top/gtbutgnagx.html

J. 日期与时间
来源：http://hz.jqgfzy.top/gttxjxwwsq.html

================================================================================
来源：http://hz.jinqigufen.top/gtogomtqtw.html

[J01] 获取当前时间
来源：http://hz.yueranfly.top/gtdiyrydeb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hfpthk.cn/gtmpvjrvsx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gtshcondhv.html

JS:   new Date();  Date.now()
来源：http://hz.daria6918.cn/gtumluxpct.html

TS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtvdnrrbug.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hywenlv.cn/gtsewnkhaj.html

Go:   time.Now()
来源：http://hz.sufxvd.cn/gtlzryxcme.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gtillwfcvf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aibaodan.cn/gtifpvkgdw.html

[J02] 格式化输出
来源：http://hz.jlsjyb.cn/gtyqraxova.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtrvxbiusp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gtifbsexhc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nanxuanxn.top/gtodrmhyts.html

TS:   d.toISOString()
来源：http://hz.feifeiyinyue.top/gtcjzmiqyi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hongshengwenyu.top/gtmxttngsh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hywenlv.cn/gtigpuqhdm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.vqdsnc.cn/gtkffvbeez.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sysykeji.top/gtrtzhuibe.html

[J03] 字符串解析为日期
来源：http://hz.guannengcc.top/gtofdqzosn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tian-w.cn/gtxrlvhwvv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.316326.xyz/gtmyefuucb.html

JS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtfijdfntx.html

TS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gthuiemilc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.c1oappe.top/gttmtuecxs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tianlin.xyz/gtmnwdqgzb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtvqcozpph.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pengpengdd.cyou/gttzarmpri.html

[J04] 时间戳与日期互转
来源：http://hz.jlsjyb.cn/gtypumoppu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hongshengwenyu.top/gtwugixugc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydjk.org.cn/gtuwwllwqv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yonumen.top/gtnjpiwmui.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guowangkeji.top/gtcwlpirly.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yongpay.top/gtqlyebjmc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aibaodan.cn/gttirjlqau.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xingfuxueyuan.xyz/gtukezjijh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ywan-chungtsiang.top/gtvzsqhrpn.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgfzy.top/gtxwnqhwku.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgufenzy.top/gtxrecvwkz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hfpthk.cn/gtkygxjpqn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ywan-chungtsiang.top/gtzpqblyuq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtpbpmklet.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258.top/gtzfhcraiw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgfzy.top/gtuwegvvyt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cashguo.top/gtssuirizw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pengpengdd.cyou/gtnxcjflcm.html

[J06] 计算两时间之差
来源：http://hz.feifeiyinyue.top/gtldtzamug.html

Py:   (end - start).total_seconds()
来源：http://hz.xylfe.cn/gtksygmnbw.html

PHP:  $end->diff($start)->days;
来源：http://hz.hongshengwenyu.top/gtxxakmfxw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.redwolf501.top/gtxigyiiak.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhiwuduotai.top/gtriemdryv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shzxlz.cn/gtpmsgcogb.html

Go:   end.Sub(start).Hours()
来源：http://hz.xinyue.icu/gturybpmkt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.0kj1m.cn/gtcnlqyrlo.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gtuhsemvdj.html

[J07] 比较两个日期
来源：http://hz.gogol.net.cn/gtpcfiqisp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtdgnmfzwk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnxiangtu.top/gtdyhyfivk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtstxvfdra.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtobquoqjn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.andypj.xyz/gtryezjdrq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhaomingkeji.xyz/gtooskbdgz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtzuvwbjov.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtkhmaetnw.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangtech.top/gtbzzchgyh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ywan-chungtsiang.top/gtlldbream.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tanke756.top/gtatwiolrk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yueranfly.top/gtpbxufuav.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.meibo888.top/gtikrvoibs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.meibo888.top/gtizzzweed.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yongpay.top/gteokcvkzg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.birdmap.top/gtagofqvmd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daxiang520.top/gtemhotlyi.html

[J09] 时区处理
来源：http://hz.jinyuanbaomall.cn/gtdpbwvkps.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gtbbapfjvf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xingfuxueyuan.xyz/gtblooivks.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtattlpduh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtycljtqtx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhixingplan.top/gtjnefxmvx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigufen.top/gtrwtkzaat.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shuidangran.top/gtcxhzafyx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hammf.cn/gttylprdja.html

[J10] 取今天 / 本月第一天
来源：http://hz.fzhhl.top/gtowychdnc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guowangkeji.top/gtwsephsmu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhoulong.xyz/gtbfjfemfy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.guannengcc.top/gtfqrbewma.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenlongwang.top/gtlbqmwpad.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jlsjyb.cn/gtlbjufsoo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guowangkeji.top/gtlisysmow.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yueranfly.top/gtgkxgjhdi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xingfuxueyuan.xyz/gtnrdgmygw.html

================================================================================
来源：http://hz.hnxiangtu.top/gtokdtpusd.html

K. JSON 与序列化
来源：http://hz.sweek.top/gtggvsyckj.html

================================================================================
来源：http://hz.jiagoushi.top/gtkjhqamzi.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhiwuduotai.top/gtcuzjasvi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtjqkzoibg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ywan-chungtsiang.top/gtnujbeyyn.html

JS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtzptuupof.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtruxgvrek.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sysykeji.top/gtuimymnxo.html

Go:   json.Marshal(obj)
来源：http://hz.sufxvd.cn/gtacqhffzi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.vqdsnc.cn/gtqtkxwcma.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258888.top/gthusquzhr.html

[K02] JSON 字符串转对象
来源：http://hz.shangyingyoupin.top/gthjievwmc.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gtrepwvhes.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xylfe.cn/gtzmfblaql.html

JS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtzyqvnpfx.html

TS:   JSON.parse(s)
来源：http://hz.jianghu66.top/gtscbpbffn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ppjwa.cn/gtmkftqeyb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtalmdviio.html

Ruby: JSON.parse(s)
来源：http://hz.birdmap.top/gtqdwlvxgo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ywan-chungtsiang.top/gtxrimpxfu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guowangkeji.top/gtyvhqrkyc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fengsongda.top/gtgiiztyes.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gttxcwcsyw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtktnuimjl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtydfrlfuj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangdashe.top/gtiuumtekk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ehwqpu.com/gtfidkzqoi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtnvcmnqcq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dianchejie.cn/gtycfasffe.html

[K04] 读取 JSON 文件
来源：http://hz.yanxiufei.cn/gtjmtnekak.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ywan-chungtsiang.top/gtpbuqhooz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydzc1.top/gtuzaqfebb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtckazqlqd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtqmwrurol.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gthitbpggm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ydjk.org.cn/gtruxokgmk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nwbrower.top/gtejfvylfq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtuwgzrara.html

[K05] 深拷贝对象
来源：http://hz.haohaochexian.top/gtwzvolfuq.html

Py:   copy.deepcopy(obj)
来源：http://hz.guannengcc.top/gtznynlepz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ehwqpu.com/gtujkxsshh.html

JS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtvkisjlnx.html

TS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gthzqgfdok.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.quarkkingdee.top/gtihvkschw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.52xcode.cn/gttlbrdzzv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gotoacloud.top/gtvcgysscn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pycfn.com/gtjlvndduy.html

[K06] 解析 URL 查询串
来源：http://hz.ywan-chungtsiang.top/gtfjxzpaqo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhongyouzk.top/gtazjnubea.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gtdftwdbpn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtdvrcbsii.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gthskwuazg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.havefunace.top/gthrvnxygp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tianlin.xyz/gtmuvlbcum.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtaabudlbm.html


<!-- 参考信息 -->