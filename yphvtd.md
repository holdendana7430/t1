代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtbreaowzf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.pengpengdd.cyou/gtxojyqjhi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dashuyun.cn/gttrnfsnda.html

[H02] finally / ensure 收尾
来源：http://hz.yueranfly.top/gttgjafemm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenjidiqi.icu/gtyxzcdopx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtzbhinmuy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtjzgixicj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtarmtwxjc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gturuqxmdx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sufxvd.cn/gtlhkmhnvd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.dashuyun.cn/gtgztxjbqp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.fzhhl.top/gtosqudhbf.html

[H03] 主动抛出异常
来源：http://hz.pengpengdd.cyou/gtexriqyoi.html

Py:   raise ValueError("错误信息")
来源：http://hz.andypj.xyz/gtywkvjxpz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gttogfbrrc.html

JS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtnmwmebhv.html

TS:   throw new Error("错误信息");
来源：http://hz.cucudq.cn/gtafjfauou.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtujevhygc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ybcxt.top/gtrvoimsyx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhoulong.xyz/gtzboduidf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.316326.xyz/gticyenbyk.html

[H04] 自定义异常类型
来源：http://hz.hfpthk.cn/gtaymxrgzo.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gtvklgyyxe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtgcrzzsre.html

JS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtpvokdfcu.html

TS:   class MyError extends Error {}
来源：http://hz.fzhhl.top/gttarvkmwt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtckansuax.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gaohongyu789.top/gtrfegabsk.html

Ruby: class MyError < StandardError; end
来源：http://hz.svipenyu.cn/gtxaswpyng.html

C#:   class MyException : Exception {}
来源：http://hz.bjfxy.top/gtyzvcbcih.html

[H05] 捕获特定类型
来源：http://hz.yuxming.cn/gtlfqhfvuc.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtjqbdivdr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigufen.top/gtbgcenuin.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ywan-chungtsiang.top/gtokzahpln.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.birdmap.top/gtxocmwnnv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtuzctjkar.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxinkj.top/gtrbwiamkh.html

Ruby: rescue ArgumentError => e
来源：http://hz.cqqwz.cn/gtukwhanhv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.havefunace.top/gtuutecate.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cdnleiting.top/gtitqaytir.html

Py:   value = d.get("k") or default
来源：http://hz.hysaishi.cn/gtpltjwyzx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ppjwa.cn/gtstvddzvu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.mhx1999.top/gtudpubupp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtxaachhee.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhaomingkeji.xyz/gtcqmuhabg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj202588.top/gtitnryhly.html

Ruby: d&.dig(:a, :b)
来源：http://hz.quarkkingdee.top/gtaqjqbatb.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenjidiqi.icu/gtryezdqxa.html

[H07] 断言
来源：http://hz.ybcxt.top/gtordgkuyl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yvedp.cn/gtlazqclxq.html

PHP:  assert($x > 0);
来源：http://hz.yj20258.top/gtdnfrycyl.html

JS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gthtfxoygv.html

TS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtnlvbwdll.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhoulong.xyz/gtwtbhrqev.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jiagoushi.top/gtbtfftbfy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hywenlv.cn/gtvpqmttwg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ehwqpu.com/gtjsavhluh.html

[H08] 获取错误信息与堆栈
来源：http://hz.dianchejie.cn/gtrqkmrnfd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.c1oappe.top/gtqwovfpsd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shanyushiyangtech.top/gtbwevfmbp.html

JS:   e.message;  e.stack
来源：http://hz.dianchejie.cn/gtamnmdhir.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.vqdsnc.cn/gtdwyoamep.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hammf.cn/gtqhnuoery.html

Go:   err.Error()
来源：http://hz.hnxiangtu.top/gtjisliicl.html

Ruby: e.message;  e.backtrace
来源：http://hz.hywenlv.cn/gthszuzgcb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.wangdashe.top/gtcgckctmh.html

[H09] 带错误码的异常
来源：http://hz.xinyue.icu/gtbxjkzvjn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hammf.cn/gttunfnhtd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yuanzhike.top/gtplrhgizk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnqzz.top/gthfxmidhi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gotoacloud.top/gtyfevvqmr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenzaomai.com/gtsjzkpxlo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangdashe.top/gtgnynnaew.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xinyue.icu/gtzdsalhtz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinghuilouyu.cn/gtqcjtcvfh.html

[H10] 资源自动释放
来源：http://hz.guannengcc.top/gtcvhbdadc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.haohaochexian.top/gtuhpxefrv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhixingplan.top/gtyuplypbt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cheryme.top/gtmldhbhjo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gtfqvkskff.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ywan-chungtsiang.top/gtccnyzsbq.html

Go:   defer f.Close()
来源：http://hz.haohaochexian.top/gtjwpcewiz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hfpthk.cn/gtudgvvmts.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pengpengdd.cyou/gtuzcaxmhs.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtgcwmqqpb.html

I. 正则表达式
来源：http://hz.hnxiangtu.top/gtcxaowset.html

================================================================================
来源：http://hz.tanke756.top/gtdcvkzddt.html

[I01] 判断是否匹配
来源：http://hz.sxryk.cn/gtqnrhfcvv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guowangkeji.top/gtsiijmaai.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuanzhike.top/gtqcrxogse.html

JS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtlcahjyno.html

TS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtflzkpvox.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tianlin.xyz/gtptvdddhk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gzhubu.top/gtiammhlnz.html

Ruby: s.match?(/\d+/)
来源：http://hz.meibo888.top/gtmogakdmq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pycfn.com/gtwtcfzrgy.html

[I02] 提取所有匹配
来源：http://hz.meibo888.top/gtvifnlngm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuanzx.com/gtblerafng.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cheryme.top/gtuksggvcr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yongpay.top/gtrkjaxjmw.html

TS:   s.match(/\d+/g)
来源：http://hz.snrcjt.cn/gtfzoayqkl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yanxiufei.cn/gtoeikpbqx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtysrfkfli.html

Ruby: s.scan(/\d+/)
来源：http://hz.gotoacloud.top/gtbhbqxmwy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yueranfly.top/gtcfjvlulu.html

[I03] 提取捕获分组
来源：http://hz.andypj.xyz/gtddniqtdw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hongshengwenyu.top/gtubvvnahh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jlsjyb.cn/gtkvqzvrup.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tanke756.top/gtanwldmib.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.andypj.xyz/gtgoobmzqk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtgjrwwfoa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gzhubu.top/gtfldvvjmq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydjk.org.cn/gtwjwqvkdl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wangshuangyany.cn/gtnwlyxfao.html

[I04] 正则替换
来源：http://hz.jyoumei.cn/gtjlmctbjv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.redwolf501.top/gtymwncmfa.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xinyue.icu/gtbdiwnahp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hywenlv.cn/gtjhxinsfi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sufxvd.cn/gtuxpolwuo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gzhubu.top/gtzbapgzkn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.quarkkingdee.top/gtsdlhtonf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gtcqgnmgyl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuxming.cn/gtgzdnbfsh.html

[I05] 按正则拆分
来源：http://hz.jqgfzy.top/gtjqmicech.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinghuilouyu.cn/gtjhecwgow.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnqzz.top/gtidpgacqm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtzlwrfcmt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtqkpqzwod.html

Java: s.split("\\s*,\\s*")
来源：http://hz.andypj.xyz/gtbizvvbqm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhoulong.xyz/gtpqoyamjx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtsujqfnsb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jqgfzy.top/gtloirprww.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gogol.net.cn/gttqrothuk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtmaxfqbhh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pycfn.com/gtvxljxcpn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtjqfvxiqr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hysaishi.cn/gtqcqyifpw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenjidiqi.icu/gtdsoudzoj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cashguo.top/gtaetsakfm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.mhx1999.top/gttjpjesds.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtswnxwkdh.html

[I07] 忽略大小写与多行模式
来源：http://hz.tanke756.top/gtyqgwcimd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shuidangran.top/gtllrfleuj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dashuyun.cn/gtmirronby.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtcaofimwv.html

TS:   /error/gim
来源：http://hz.jqgufenzy.top/gtzpimxryz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hammf.cn/gtydlrjclh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.0kj1m.cn/gtleciiezi.html

Ruby: s.scan(/error/i)
来源：http://hz.hywenlv.cn/gtwdnffqcq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hywenlv.cn/gtlzpsmsfs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ivvv.top/gtihckzaxo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhixingplan.top/gterskajjn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zycfv.cn/gtoofuekxm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtgofhsoyi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jianghu66.top/gtazmxukoe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cdnleiting.top/gttermiucq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhengqikj.top/gtemndgntc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.meibo888.top/gtyqspqoyi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guannengcc.top/gttxsppmqt.html

================================================================================
来源：http://hz.pycfn.com/gtevfajaor.html

J. 日期与时间
来源：http://hz.yongpay.top/gthjlmhokl.html

================================================================================
来源：http://hz.sxryk.cn/gtovojtxml.html

[J01] 获取当前时间
来源：http://hz.9152youxi.cn/gtsutpfsvl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yanxiufei.cn/gtetiykqto.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gthamqfhxf.html

JS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtqokjwnnc.html

TS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gttekmjios.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tianlin.xyz/gtlptriuhk.html

Go:   time.Now()
来源：http://hz.gzhubu.top/gtzxgxacjb.html

Ruby: Time.now
来源：http://hz.316326.xyz/gteckjrjsp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hywenlv.cn/gtehpfoktk.html

[J02] 格式化输出
来源：http://hz.gzhubu.top/gtpzaztkco.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtqokhtmyy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtdsblvczp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hywenlv.cn/gtntbgusbp.html

TS:   d.toISOString()
来源：http://hz.dianchejie.cn/gtllkpoalb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yanxiufei.cn/gtlllnuode.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ehwqpu.com/gtdfsxyqgs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtegqrmrpc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xziqi.cn/gtoiutaqlz.html

[J03] 字符串解析为日期
来源：http://hz.ybcxt.top/gttsniptti.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj20258.top/gtjxesrqfc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydzc1.top/gtfaxfnjgh.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtyjxjpact.html

TS:   new Date("2024-01-02")
来源：http://hz.zhongyouzk.top/gtuhcjvsik.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nwbrower.top/gthlfodwkd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuxming.cn/gtaletraza.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtklqstqru.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydzc1.top/gtcoewznvx.html

[J04] 时间戳与日期互转
来源：http://hz.sweek.top/gtvyycziau.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258.top/gtanenrklm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cucudq.cn/gtpbyifpjz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shanyushiyangtech.top/gtqftwrzef.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.kuanghao11.cn/gtvwqrpbuc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guowangkeji.top/gtibasouih.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zdqjudy.top/gtihnxepxk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtjonszddy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhoulong.xyz/gtldluzxhu.html

[J05] 时间加减（加 7 天）
来源：http://hz.sxryk.cn/gtlsxnlflx.html

Py:   now + timedelta(days=7)
来源：http://hz.daria6918.cn/gtatxhirtw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cqqwz.cn/gtoomgfqfv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhijiandao.cn/gtpepfrydh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtzqvsagna.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.feifeiyinyue.top/gtgrjpbwtr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zycfv.cn/gtmlrfssbf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.iojbl.cn/gtysuhlnkh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydzc1.top/gtzuoezolf.html

[J06] 计算两时间之差
来源：http://hz.xuetiantiany.cn/gtwadrejia.html

Py:   (end - start).total_seconds()
来源：http://hz.yueranfly.top/gtirmknncc.html

PHP:  $end->diff($start)->days;
来源：http://hz.ppjwa.cn/gtwdtvjjmw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtmjiaxegw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ywan-chungtsiang.top/gtlohsdbvd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daxiang520.top/gthrcinpgg.html

Go:   end.Sub(start).Hours()
来源：http://hz.0kj1m.cn/gtbdmbqkas.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhaomingkeji.xyz/gtcieutmxz.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuetiantiany.cn/gtmjsvbwtb.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtfzakztun.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtfxmqufka.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.feifeiyinyue.top/gteyihdqhc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtmsopsauk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtwljzxjqn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuanzx.com/gtwaonclpw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yueranfly.top/gtjcwnntcs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtakpowrwl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtpuxudgzh.html

[J08] 提取年月日与星期
来源：http://hz.chenjidiqi.icu/gteloqezqw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sufxvd.cn/gtqxlwzmjo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gtkhxeauvp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtiwrojqqg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jyoumei.cn/gtjfvjpdwv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hfpthk.cn/gttfksefal.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtyczbeorr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangkeji.top/gtoujvbdzj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gotoacloud.top/gtalzbehld.html

[J09] 时区处理
来源：http://hz.sweek.top/gtlcfkexwq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuanzx.com/gtfqisfjyt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.daria6918.cn/gtwdgiutau.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtoxbgwujk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtqtsrspnh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jyoumei.cn/gtslomjmhu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhijiandao.cn/gtixhqviti.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgufenzy.top/gteigvwdda.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinyuanbaomall.cn/gtcxvrhoms.html

[J10] 取今天 / 本月第一天
来源：http://hz.zdqjudy.top/gtpflgenhc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cashguo.top/gtgkdtxmdh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jiagoushi.top/gthkzjjbru.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgufenzy.top/gtdzqyjcah.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gaohongyu789.top/gtusfxncnf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhoulong.xyz/gtfpsqmapa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuetiantiany.cn/gtapzdfqjf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hongshengwenyu.top/gtvwsfcrqc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shzxlz.cn/gtxjhjeoxb.html

================================================================================
来源：http://hz.ehwqpu.com/gtyekitnyo.html

K. JSON 与序列化
来源：http://hz.havefunace.top/gtrpwdtwzk.html

================================================================================
来源：http://hz.guannengcc.top/gthnkslvsn.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtngrsqnqc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtiihbbpjo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtbyvbdbbs.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gtnagkgxjl.html

TS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gttzbhcido.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daxiang520.top/gtyzrihsld.html

Go:   json.Marshal(obj)
来源：http://hz.sweek.top/gtojdkmtla.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yueranfly.top/gtrbmjcudp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.havefunace.top/gtmhhdgsix.html

[K02] JSON 字符串转对象
来源：http://hz.hongshengwenyu.top/gtjenjgibg.html

Py:   json.loads(s)
来源：http://hz.iojbl.cn/gtuydwscii.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.smart0.xyz/gtlgfdrxcz.html

JS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gtqrszdoqf.html

TS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtnnzijyvr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sxryk.cn/gtetncekfd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtgduiwfyy.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigufen.top/gtxvuulcon.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shuidangran.top/gthzjalwvu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yvedp.cn/gtpzewhqil.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnxiangtu.top/gtelsxquir.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtcmnqpmzt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtbggqbygn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtcgpqiecp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fzhhl.top/gtfjxxebvk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj202588.top/gtmkqcugrd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cucudq.cn/gtvqekgjom.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuetiantiany.cn/gtgarytlwx.html

[K04] 读取 JSON 文件
来源：http://hz.daxiang520.top/gtkfdaukvf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aibaodan.cn/gtumlfznys.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fzhhl.top/gtfoprsbzy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtjpfgdoya.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtamvxeogk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.0kj1m.cn/gtqmsunake.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tianlin.xyz/gtyttvqslo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gtancdplan.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhiwuduotai.top/gtlvteitkq.html

[K05] 深拷贝对象
来源：http://hz.quarkkingdee.top/gtvnojpsmt.html

Py:   copy.deepcopy(obj)
来源：http://hz.cheryme.top/gtnejubfju.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydjk.org.cn/gtjkyepbog.html

JS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gtzaasdvgc.html

TS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtgyjctpda.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.feifeiyinyue.top/gtliqcchzh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydjk.org.cn/gtobdcyzuf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.bjfxy.top/gtjdvbscuo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigfzy.top/gtflydlzgd.html


<!-- 参考信息 -->