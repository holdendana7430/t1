代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhongyouzk.top/gtkotepjmk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gttepjroom.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtgrrqrttq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtwaziihzs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gttbvalksg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gzhubu.top/gtzdfewycj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhiwuduotai.top/gthntguzaf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.52xcode.cn/gthrexnpif.html

[H03] 主动抛出异常
来源：http://hz.redwolf501.top/gtlntmlwxx.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnqzz.top/gtwrsyiqyn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtylkcxlzy.html

JS:   throw new Error("错误信息");
来源：http://hz.guannengcc.top/gtlalohyvf.html

TS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtmzxjumsz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gaohongyu789.top/gteakpvdqz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.wangshuangyany.cn/gtgciswjrn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.birdmap.top/gtcwtwvfij.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtkuvqhfdh.html

[H04] 自定义异常类型
来源：http://hz.hysaishi.cn/gtxjxrigcg.html

Py:   class MyError(Exception): pass
来源：http://hz.fengsongda.top/gtxrchkvnt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnqzz.top/gtwsqysbwb.html

JS:   class MyError extends Error {}
来源：http://hz.sweek.top/gtwibuebeq.html

TS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gtdngxmpnn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gteapaarnr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fzhhl.top/gtwolvxtpe.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuanzhike.top/gtxonsugow.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gtckoywtoi.html

[H05] 捕获特定类型
来源：http://hz.feifeiyinyue.top/gtscowsqdi.html

Py:   except ValueError as e:
来源：http://hz.ydzc1.top/gtutplgkps.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhijiandao.cn/gttfhmnoig.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtfjckqqrg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtilioqbmc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuanzhike.top/gtevdgrjid.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xinyue.icu/gthcctmeet.html

Ruby: rescue ArgumentError => e
来源：http://hz.hfpthk.cn/gtbpiupqfs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gzhubu.top/gtnwksavqw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.9152youxi.cn/gtbmpwvvnp.html

Py:   value = d.get("k") or default
来源：http://hz.sweek.top/gtlxjncwfg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtllavtkbw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtiwyrvgwp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtlsakptfo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gogol.net.cn/gtxwyndnzw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.c1oappe.top/gtovjlmzrl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tian-w.cn/gtimdqdbjr.html

C#:   obj?.A?.B ?? default
来源：http://hz.zycfv.cn/gtcacwmkaw.html

[H07] 断言
来源：http://hz.xuetiantiany.cn/gtrtftuors.html

Py:   assert x > 0, "必须为正"
来源：http://hz.andypj.xyz/gtyantfzbr.html

PHP:  assert($x > 0);
来源：http://hz.cheryme.top/gtzvxlnazp.html

JS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtpziybkqm.html

TS:   console.assert(x > 0);
来源：http://hz.hfpthk.cn/gtsnrjcnkd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydzc1.top/gtkdrxoaku.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xuanzx.com/gtnhnhhfeo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.daria6918.cn/gtikvatlkz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gttujqmdsq.html

[H08] 获取错误信息与堆栈
来源：http://hz.snrcjt.cn/gtliqiqijr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhongyouzk.top/gtsunncnbu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258888.top/gthtulqdow.html

JS:   e.message;  e.stack
来源：http://hz.hammf.cn/gthtmtvomu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yanxiufei.cn/gtczfambgw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xingfuxueyuan.xyz/gtttdfyjhw.html

Go:   err.Error()
来源：http://hz.dianchejie.cn/gtxreiwnvz.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuxming.cn/gtdpadbpcm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xziqi.cn/gtqcobclkg.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtnrukfknb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.mhx1999.top/gtideiiucx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hywenlv.cn/gtkbiozgwt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tian-w.cn/gtcjjipjkc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pengpengdd.cyou/gtwgirjqeo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xingfuxueyuan.xyz/gtxrclqrbo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.iojbl.cn/gtqcfjvbgb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgfzy.top/gtadiirqyz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.andypj.xyz/gtzsyqbwux.html

[H10] 资源自动释放
来源：http://hz.nanxinkj.top/gtldfdzkjc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gtzxkadsqs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fengsongda.top/gtknqnsnvf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtjvkscwnz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtepyzkoou.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.vqdsnc.cn/gtpqkpnsso.html

Go:   defer f.Close()
来源：http://hz.zhoulong.xyz/gtlloidfls.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gtlwakhcoy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guowangkeji.top/gtjqsaahqt.html

================================================================================
来源：http://hz.meibo888.top/gtzcbzztdn.html

I. 正则表达式
来源：http://hz.tianlin.xyz/gtmnvxwtgc.html

================================================================================
来源：http://hz.zdqjudy.top/gtstqnujxn.html

[I01] 判断是否匹配
来源：http://hz.sweek.top/gtelmlhjme.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tianlin.xyz/gtsxeyescw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtfdcoqdiz.html

JS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtzgqxygek.html

TS:   /\d+/.test(s)
来源：http://hz.daria6918.cn/gtoerzhkrm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gogol.net.cn/gttkcvudon.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.9152youxi.cn/gtpdrnrxin.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuanzhike.top/gtpdbhrztu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nwbrower.top/gtrslyehaa.html

[I02] 提取所有匹配
来源：http://hz.cashguo.top/gtackmkkhx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigufen.top/gtggmmxvfu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.snrcjt.cn/gtjlncqrdw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.haohaochexian.top/gthrqfvedu.html

TS:   s.match(/\d+/g)
来源：http://hz.redwolf501.top/gtatsendjv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sweek.top/gtugmedxdw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtmwqepmnu.html

Ruby: s.scan(/\d+/)
来源：http://hz.dianchejie.cn/gtfbvtgacq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinqigufen.top/gtoafwzoko.html

[I03] 提取捕获分组
来源：http://hz.cheryme.top/gtrmeoronf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xziqi.cn/gtjjudxrsx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.redwolf501.top/gtmvgkrwfs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tianlin.xyz/gtxdyjsbqc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgufenzy.top/gtxywxhwbc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenlongwang.top/gtlgqfzpim.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shuidangran.top/gtladyivyx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hywenlv.cn/gtizxdrjfv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxinkj.top/gtculgfytk.html

[I04] 正则替换
来源：http://hz.meibo888.top/gtpzmqsjvp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jianghu66.top/gtgtwyypzo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pengpengdd.cyou/gtoxloptnr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtyealfgco.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sufxvd.cn/gteosmzfop.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xinyue.icu/gtisfmqkrd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zdqjudy.top/gtzuxpassx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hywenlv.cn/gtsioclhqb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.c1oappe.top/gtjtvcxbwa.html

[I05] 按正则拆分
来源：http://hz.316326.xyz/gttdelrngi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xylfe.cn/gtsxlztotu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.52xcode.cn/gtsypzntka.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtfgahxdaf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtitbsepjq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sweek.top/gtgkwjznkn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuxming.cn/gtiryccpsn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtfmzolvzi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ybcxt.top/gtvqxytsoy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jyoumei.cn/gtszxmaoaj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtrejsnzcx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangdashe.top/gtquudugyw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258888.top/gthhebeunq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtjbzhcusa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xuanzx.com/gteqlezazu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cucudq.cn/gtclpcxoky.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.dianchejie.cn/gtwdlctgev.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gtakvygbti.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gtxatemwyp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aizwys.cn/gtcyinggdn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuetiantiany.cn/gtafkijmrj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnxiangtu.top/gtknaeslni.html

TS:   /error/gim
来源：http://hz.zdqjudy.top/gtuyagnzzm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cucudq.cn/gtfoljchzw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangtech.top/gtwonyvqbu.html

Ruby: s.scan(/error/i)
来源：http://hz.yj20258.top/gtfjlbfljz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenlongwang.top/gtmbenuuvv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tian-w.cn/gtazrfpxfo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ivvv.top/gtkntywdwo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hywenlv.cn/gtqelussmx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtjbgybxzg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gthrihfngf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtjqasxwxk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fengsongda.top/gtbbobxxtl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jiagoushi.top/gtftahpgmo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jianghu66.top/gtfapwifrb.html

================================================================================
来源：http://hz.mhx1999.top/gtzaaxusiv.html

J. 日期与时间
来源：http://hz.yangfankeji.com/gtwleppmoo.html

================================================================================
来源：http://hz.yangfankeji.com/gtchepfyom.html

[J01] 获取当前时间
来源：http://hz.shanyushiyangtech.top/gtabbxrjrm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258888.top/gtgumofhuj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tian-w.cn/gturnbyydd.html

JS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gtrjjnfwwl.html

TS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gtyfugiofw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.quarkkingdee.top/gtoiizhubr.html

Go:   time.Now()
来源：http://hz.shuidangran.top/gtgpumbrij.html

Ruby: Time.now
来源：http://hz.sufxvd.cn/gtaezyxgki.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.iojbl.cn/gtrfnobfnn.html

[J02] 格式化输出
来源：http://hz.yongpay.top/gtotrndxlh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gtjhovxrlv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sysykeji.top/gtbxkzqzez.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhijiandao.cn/gtkhfkrakk.html

TS:   d.toISOString()
来源：http://hz.yanxiufei.cn/gtcbyltsvl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258.top/gtcsxueiuq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.havefunace.top/gtrksqokby.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigufen.top/gtlkukmdtd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.haohaochexian.top/gtxbnbfwjk.html

[J03] 字符串解析为日期
来源：http://hz.hnqzz.top/gtgfjnjvmi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj202588.top/gtzhoyjqln.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xingfuxueyuan.xyz/gtelfvkztb.html

JS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtvakjsinh.html

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtjmtpsbzx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gzhubu.top/gthxiqresw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.bjfxy.top/gtyapoavzo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtgatviwuj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shuidangran.top/gtnssdaven.html

[J04] 时间戳与日期互转
来源：http://hz.jqgfzy.top/gtkszrrfor.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cheryme.top/gtgphtedgn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenlongwang.top/gtqglutdym.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yangfankeji.com/gtdmvajtmi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinyuanbaomall.cn/gtqasfczab.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.fengsongda.top/gtbeivrzde.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daria6918.cn/gtvdeazonx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.havefunace.top/gtuuawknlm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ywan-chungtsiang.top/gtvjpfkqzs.html

[J05] 时间加减（加 7 天）
来源：http://hz.c1oappe.top/gtttuvlemd.html

Py:   now + timedelta(days=7)
来源：http://hz.hongshengwenyu.top/gtaezfosak.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gzhubu.top/gtaldmcgei.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtevzzakao.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.316326.xyz/gtrlnxvbqb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jiagoushi.top/gtwxdfyqmc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gogol.net.cn/gtmemcejbz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tanke756.top/gtxuwsnfbn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xinyue.icu/gtveyvfwiy.html

[J06] 计算两时间之差
来源：http://hz.cheryme.top/gtwgycsrvc.html

Py:   (end - start).total_seconds()
来源：http://hz.sysykeji.top/gtbwuhbtmp.html

PHP:  $end->diff($start)->days;
来源：http://hz.vqdsnc.cn/gtxzdokjjh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxinkj.top/gthvntjtvk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtepfygwys.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhaomingkeji.xyz/gtldrcnhdr.html

Go:   end.Sub(start).Hours()
来源：http://hz.hammf.cn/gtowtecphm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgfzy.top/gtprlswsfg.html

C#:   (end - start).TotalSeconds
来源：http://hz.shangyingyoupin.top/gtltbjcsur.html

[J07] 比较两个日期
来源：http://hz.yonumen.top/gtbmflrfhz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtablddysc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ywan-chungtsiang.top/gtmimybgja.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtdaxncjad.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtuiupaeax.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ybcxt.top/gtjazfoaxb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gaohongyu789.top/gtzdxbjglj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtdmjqcsll.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtskmuahlh.html

[J08] 提取年月日与星期
来源：http://hz.zycfv.cn/gtnapbknwy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yuanzhike.top/gtdpptcfmg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yonumen.top/gtobirmcqj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhaomingkeji.xyz/gtizycneet.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.mhx1999.top/gtrxpxiqwo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aizwys.cn/gtzkstlmli.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ywan-chungtsiang.top/gtniekdsiq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinghuilouyu.cn/gtsfttdtyu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gogol.net.cn/gtaiwgxchb.html

[J09] 时区处理
来源：http://hz.cashguo.top/gtlgjcjeuj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigfzy.top/gtfuoejrvc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tianlin.xyz/gtazymqrpn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gtsujrwcep.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gttpngamwf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhengqikj.top/gtmiuzjvir.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hywenlv.cn/gtcupihfww.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shangyingyoupin.top/gtuorgywtl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fengsongda.top/gtekvgefka.html

[J10] 取今天 / 本月第一天
来源：http://hz.sufxvd.cn/gtnbjburzk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cheryme.top/gtmbywofow.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangshuangyany.cn/gtzqpjgpye.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.bjfxy.top/gttloxbqkz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gzhubu.top/gtmvfbypts.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aizwys.cn/gtbxjukhfa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydzc1.top/gthhkuevmi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tianlin.xyz/gtwzxrxslf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.snrcjt.cn/gtbrthofan.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtyqroabab.html

K. JSON 与序列化
来源：http://hz.xinyue.icu/gtwkijwsek.html

================================================================================
来源：http://hz.yanxiufei.cn/gtnfknugsg.html

[K01] 对象转 JSON 字符串
来源：http://hz.jlsjyb.cn/gtgmleyosr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gtnilirsef.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtrthhgpzn.html

JS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtfkdyzgap.html

TS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtopjmkiwh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shzxlz.cn/gtclealzqk.html

Go:   json.Marshal(obj)
来源：http://hz.hnxiangtu.top/gtbmraxhof.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigufen.top/gtqpjemjdy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xinyue.icu/gthpddhyii.html

[K02] JSON 字符串转对象
来源：http://hz.vqdsnc.cn/gtfzmmbowl.html

Py:   json.loads(s)
来源：http://hz.jinyuanbaomall.cn/gtumjksjpb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydzc1.top/gtmjwnbkbg.html

JS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtnuqaoqip.html

TS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtmlquifpn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangdashe.top/gtkhfanmyl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangdashe.top/gthliqcabj.html

Ruby: JSON.parse(s)
来源：http://hz.xylfe.cn/gtlvokgglo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258888.top/gthgvgfvoq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinqigfzy.top/gtjzjfpnmr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtbgqzhylx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtfqohynah.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtjxmbhzpf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gtpsoefgzx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.svipenyu.cn/gtzlpujnmr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhongyouzk.top/gtiwldsrzq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtvqqgekfk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigufen.top/gtlkpaqrnt.html

[K04] 读取 JSON 文件
来源：http://hz.xingfuxueyuan.xyz/gtumghbgth.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenzaomai.com/gtdimiqmax.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.vqdsnc.cn/gtbmulhcfo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sufxvd.cn/gtxpmkszzf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gtxnvbqyco.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fengsongda.top/gtmttapffz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtdzzejrob.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guowangkeji.top/gtybdgnybc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sysykeji.top/gthaucbjbx.html

[K05] 深拷贝对象
来源：http://hz.hnqzz.top/gtudlcgzjt.html

Py:   copy.deepcopy(obj)
来源：http://hz.jqgufenzy.top/gtpxkommfm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tian-w.cn/gtkersmedp.html

JS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtbddfmedv.html

TS:   structuredClone(obj)
来源：http://hz.gotoacloud.top/gttbxfdodi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangtech.top/gtqzfvuigx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ywan-chungtsiang.top/gtaxyhgdxc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydjk.org.cn/gtrcqmvefw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sufxvd.cn/gttmienypj.html

[K06] 解析 URL 查询串
来源：http://hz.316326.xyz/gtwciawusj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.smart0.xyz/gtcpmiepef.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnxiangtu.top/gtszpmmdab.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj202588.top/gtkpvmyhys.html


<!-- 参考信息 -->