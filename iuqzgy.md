代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ywan-chungtsiang.top/gtlkuwshsx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gtmfzqsonu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gtosfxpgez.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yongpay.top/gtlpmdbejm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgufenzy.top/gtjpajxffv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigufen.top/gtpddqkdrm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cashguo.top/gtrppvlhog.html

[H02] finally / ensure 收尾
来源：http://hz.chenjidiqi.icu/gtilucgdly.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.tianlin.xyz/gtoeskxjpd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtwtacfytm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtiqldhypi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtrlucbhde.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtaecgtjns.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hongshengwenyu.top/gttyagolea.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhoulong.xyz/gtpekjjwin.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnxiangtu.top/gtguzamqgr.html

[H03] 主动抛出异常
来源：http://hz.hywenlv.cn/gtectqyfxq.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtdrybjpas.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtgmsseqmv.html

JS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gttdxfivmq.html

TS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtatgxapkw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtmsctqgqh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jyoumei.cn/gtkazhxbqn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pengpengdd.cyou/gtkhubcriw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtrjjtsram.html

[H04] 自定义异常类型
来源：http://hz.yongpay.top/gtjcnflecn.html

Py:   class MyError(Exception): pass
来源：http://hz.shangyingyoupin.top/gthiaphybm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtawwopvru.html

JS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtnjegkjvf.html

TS:   class MyError extends Error {}
来源：http://hz.aizwys.cn/gtivxxdgcw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yongpay.top/gtrctqfcfb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yuxming.cn/gtwlahrawa.html

Ruby: class MyError < StandardError; end
来源：http://hz.redwolf501.top/gteilxoysj.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigfzy.top/gtffzwbqfx.html

[H05] 捕获特定类型
来源：http://hz.jinqigfzy.top/gtzgxpxamz.html

Py:   except ValueError as e:
来源：http://hz.jinqigfzy.top/gtwaofpdib.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yvedp.cn/gtxvammoxt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtipwksktt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtsxhhfcoj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhongyouzk.top/gtpgtxqqza.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xziqi.cn/gtmacuyvmw.html

Ruby: rescue ArgumentError => e
来源：http://hz.52xcode.cn/gtjkvfobbn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hongshengwenyu.top/gtzrupnsbw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhengqikj.top/gtxedumkmp.html

Py:   value = d.get("k") or default
来源：http://hz.ydjk.org.cn/gtlxssakpb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hywenlv.cn/gtqhmyuksd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shangyingyoupin.top/gtyflxetki.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtsvdfyfbo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.svipenyu.cn/gtxkmkxyun.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gogol.net.cn/gtpodklbyn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fengsongda.top/gtvbwhrtyk.html

C#:   obj?.A?.B ?? default
来源：http://hz.daria6918.cn/gtbnrlpzah.html

[H07] 断言
来源：http://hz.gzhubu.top/gtaclqeoja.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhongyouzk.top/gtbibzxqgt.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gtyxzztsoe.html

JS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtshpxwsgg.html

TS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtxhulztud.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daxiang520.top/gtaxadpply.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ywan-chungtsiang.top/gthzrwyivi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgufenzy.top/gtzedwxqga.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aibaodan.cn/gtpowpepow.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtaxzlbjsb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sxryk.cn/gtgzkfujqc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenjidiqi.icu/gtfeeftweg.html

JS:   e.message;  e.stack
来源：http://hz.iojbl.cn/gtbegnhadu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258.top/gtwhegwbuv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guannengcc.top/gtnkbvkdzh.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gteaeshluy.html

Ruby: e.message;  e.backtrace
来源：http://hz.nwbrower.top/gtnmfjdavp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guowangkeji.top/gttloliwye.html

[H09] 带错误码的异常
来源：http://hz.jianghu66.top/gtjrdbgmoq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tian-w.cn/gtaylcxnlc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.9152youxi.cn/gthigibjad.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenjidiqi.icu/gtzvnolwla.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenzaomai.com/gtdhywlckx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenlongwang.top/gtyghvpksg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gzhubu.top/gttsknpgak.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yanxiufei.cn/gttbarxdxn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jlsjyb.cn/gtagjixqpc.html

[H10] 资源自动释放
来源：http://hz.ehwqpu.com/gtyyrujbkq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.vqdsnc.cn/gtqmqaxrjh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xylfe.cn/gtklgmwdlc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtallzkvaa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtrdpzxizy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtmuvmqrgq.html

Go:   defer f.Close()
来源：http://hz.bjfxy.top/gtxewvtisg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yvedp.cn/gtgvvodsbh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fzhhl.top/gtcwsudadu.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtelqxrqes.html

I. 正则表达式
来源：http://hz.yvedp.cn/gtjhaibpem.html

================================================================================
来源：http://hz.sweek.top/gtgfypobkd.html

[I01] 判断是否匹配
来源：http://hz.zhixingplan.top/gtbtyjclvh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtfpyakfyb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.52xcode.cn/gtnddjfxjc.html

JS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtqvlweyqk.html

TS:   /\d+/.test(s)
来源：http://hz.cqqwz.cn/gtqgvpahzv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yj202588.top/gtlrstuqkl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtuvhamixy.html

Ruby: s.match?(/\d+/)
来源：http://hz.c1oappe.top/gtjygsveaz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.andypj.xyz/gtqgzcxhro.html

[I02] 提取所有匹配
来源：http://hz.svipenyu.cn/gtbzgmupyi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigfzy.top/gtloiwmlln.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuanzhike.top/gtwafkkkos.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.meibo888.top/gtbdnlusen.html

TS:   s.match(/\d+/g)
来源：http://hz.ppjwa.cn/gtqwnobsaq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.quarkkingdee.top/gtpbkdvfns.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cheryme.top/gtmezdwnel.html

Ruby: s.scan(/\d+/)
来源：http://hz.snrcjt.cn/gtyppkzsiy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.quarkkingdee.top/gtpynxlnln.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gtdsqtfwkq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tianlin.xyz/gtxymtbocr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtewxxdoen.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ivvv.top/gtckacunhl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.52xcode.cn/gtuexecxhb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.c1oappe.top/gthnzbetxq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtqshixwpn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gotoacloud.top/gtkvsytxwf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhaomingkeji.xyz/gtrshlhtoe.html

[I04] 正则替换
来源：http://hz.cqqwz.cn/gtavfwkedx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daxiang520.top/gtvnvsucsc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ehwqpu.com/gtnhazpjax.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtmacppycm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtjknyhdmg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258888.top/gtoapenmlm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.birdmap.top/gthfuchbfi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ppjwa.cn/gtkrehkmsk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtzivapdzi.html

[I05] 按正则拆分
来源：http://hz.hysaishi.cn/gtmhscaawl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.redwolf501.top/gtypovrsxu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hfpthk.cn/gtdioktyrv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtggmlrsov.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtwtmuxnnl.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuetiantiany.cn/gtqxyznkok.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuanzx.com/gtpnrwqeom.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gttpqsspzh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jqgufenzy.top/gtfdholrzx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhijiandao.cn/gteeojxvoq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.vqdsnc.cn/gtifykjwic.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dianchejie.cn/gtolysiqyt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtmzrmsrto.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtupwrnion.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dashuyun.cn/gtpvyogujg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.birdmap.top/gtnxwlzfhl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xinyue.icu/gtknudfcuy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gttumjymap.html

[I07] 忽略大小写与多行模式
来源：http://hz.fengsongda.top/gtrvwlgvry.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenzaomai.com/gtxgkgdxfz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cucudq.cn/gtktphgmjc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuanzhike.top/gtulnymxmi.html

TS:   /error/gim
来源：http://hz.jinyuanbaomall.cn/gtechbmitt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxuanxn.top/gtwmlwtwks.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hammf.cn/gtpxktgwax.html

Ruby: s.scan(/error/i)
来源：http://hz.daxiang520.top/gtzkjxyeeh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj202588.top/gtqgeymlzh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ppjwa.cn/gthuhaosjz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinghuilouyu.cn/gtacipstet.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhengqikj.top/gtdxadbtrl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhoulong.xyz/gtglntbuhv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtjoapjiyk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.meibo888.top/gtabmenmnq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.c1oappe.top/gtoahkmgot.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hywenlv.cn/gtfktnotuy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gtpnauqkck.html

================================================================================
来源：http://hz.fengsongda.top/gtrcijfmev.html

J. 日期与时间
来源：http://hz.bjfxy.top/gtsmqltrnd.html

================================================================================
来源：http://hz.sweek.top/gtngtgbeyn.html

[J01] 获取当前时间
来源：http://hz.guannengcc.top/gtassznxlw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydjk.org.cn/gtwlwpueyn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtlzadokru.html

JS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gtjcwoamxv.html

TS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtkkcwbrqp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ehwqpu.com/gtpjsydqmz.html

Go:   time.Now()
来源：http://hz.nanxuanxn.top/gtfhmpxazv.html

Ruby: Time.now
来源：http://hz.ppjwa.cn/gtupwyfcxk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgufenzy.top/gtbjfokrer.html

[J02] 格式化输出
来源：http://hz.zhijiandao.cn/gtnfjvavsu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gtmakvrekf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtalslvieq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yvedp.cn/gtoknwisim.html

TS:   d.toISOString()
来源：http://hz.yongpay.top/gthtgcsejl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangdashe.top/gtzgiwwwtz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhaomingkeji.xyz/gtndiufoos.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gaohongyu789.top/gtyovhteok.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ivvv.top/gtkimombha.html

[J03] 字符串解析为日期
来源：http://hz.meibo888.top/gtdlcnfeny.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gtutwtxhto.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gogol.net.cn/gtgxmrculj.html

JS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtwdgovlrw.html

TS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtmcmrsjri.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtknwlqkfp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tianlin.xyz/gtkdzadlik.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtdmfhlvqg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.52xcode.cn/gtgerfndth.html

[J04] 时间戳与日期互转
来源：http://hz.jiagoushi.top/gtgqtgboix.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zycfv.cn/gthmplhijs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xinyue.icu/gtmesuhucf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhijiandao.cn/gtxfijcqvq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxuanxn.top/gtzkxhcmvp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shuidangran.top/gtgdacueit.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.iojbl.cn/gtnboegvfi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhengqikj.top/gtrccldxtu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xylfe.cn/gtmvwuqurz.html

[J05] 时间加减（加 7 天）
来源：http://hz.yueranfly.top/gtuuxpkqiz.html

Py:   now + timedelta(days=7)
来源：http://hz.tian-w.cn/gtzpovekpv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jiagoushi.top/gtozsdddnb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtpwpfmdit.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtuaqjhyus.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.andypj.xyz/gtrjwvvrej.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhiwuduotai.top/gtirvvbslt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gzhubu.top/gtkmjuhenx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtlttspimy.html

[J06] 计算两时间之差
来源：http://hz.meibo888.top/gtezfwfaxy.html

Py:   (end - start).total_seconds()
来源：http://hz.cheryme.top/gtlppisolp.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhixingplan.top/gtohekhkij.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinghuilouyu.cn/gtsskolqbc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxinkj.top/gtmchuqsxi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gtqppsdkfo.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangshuangyany.cn/gtpsxqckmk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fengsongda.top/gtxllhazvk.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinyuanbaomall.cn/gtjortbtnw.html

[J07] 比较两个日期
来源：http://hz.jianghu66.top/gtajqrgejj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtnfegouqy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.birdmap.top/gtccnjnutd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hywenlv.cn/gtnxqogsau.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cashguo.top/gtueiumtbq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yonumen.top/gtqdktwbge.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgfzy.top/gtojpwiylb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtpywrnlfi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gttuomjyuf.html

[J08] 提取年月日与星期
来源：http://hz.wangshuangyany.cn/gtorfstrxp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj202588.top/gtkysmqgye.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgufenzy.top/gtwilowzix.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yueranfly.top/gtohzvppck.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tianlin.xyz/gthqaswmmp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnqzz.top/gtlvuncnmd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jiagoushi.top/gtusqyuiwl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtjomcwnhs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydjk.org.cn/gthwtynxhh.html

[J09] 时区处理
来源：http://hz.cheryme.top/gtgsffehev.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hongshengwenyu.top/gtkzejlevz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuetiantiany.cn/gtcudjjplc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tianlin.xyz/gttkzkxfpw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gthzocbevv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtfvqpwkxh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangkeji.top/gtfxuhphje.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhixingplan.top/gtsktaycti.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtdqtvxnil.html

[J10] 取今天 / 本月第一天
来源：http://hz.andypj.xyz/gtcvurviqs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nanxuanxn.top/gtnzsfivqa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnqzz.top/gtpzxermtq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cheryme.top/gtzcswyueo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shangyingyoupin.top/gtrrjmxxdz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.bjfxy.top/gteieyedza.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cqqwz.cn/gtmovuehsp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aizwys.cn/gtyaykjxkp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hysaishi.cn/gtzpcgqmcr.html

================================================================================
来源：http://hz.9152youxi.cn/gtspmjhqgi.html

K. JSON 与序列化
来源：http://hz.tianlin.xyz/gtdprhjldh.html

================================================================================
来源：http://hz.yvedp.cn/gtzsjkbzfi.html

[K01] 对象转 JSON 字符串
来源：http://hz.ybcxt.top/gtjcvkkvtv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gtrcniwrjt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gthnhjnfeg.html

JS:   JSON.stringify(obj)
来源：http://hz.hfpthk.cn/gtyicjojqa.html

TS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gthowulzpi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.c1oappe.top/gtcsrqlxil.html

Go:   json.Marshal(obj)
来源：http://hz.zhiwuduotai.top/gtxcrhjsik.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.quarkkingdee.top/gtzzdzfouj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtxwiqzeep.html

[K02] JSON 字符串转对象
来源：http://hz.zhijiandao.cn/gtwngzvhbw.html

Py:   json.loads(s)
来源：http://hz.cdnleiting.top/gtkhoxajsz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jyoumei.cn/gtwskgthxe.html

JS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtqkmlhwbo.html

TS:   JSON.parse(s)
来源：http://hz.wangdashe.top/gtorkgveky.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtiwuzslwc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtuyupymou.html

Ruby: JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtesapvpgx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.kuanghao11.cn/gtrgzptgfw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xylfe.cn/gtuizqalyr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtalwrdeir.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtauoujwke.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtpjqqcuys.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtqccslyez.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gteyernsin.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangtech.top/gtvagmpdxw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.smart0.xyz/gtyexqvaai.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gotoacloud.top/gthqejdoqi.html

[K04] 读取 JSON 文件
来源：http://hz.xziqi.cn/gtokeenczo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenjidiqi.icu/gtmkyfxkdt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guannengcc.top/gtjswevxlb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtnpjohezi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigufen.top/gtamzmxdxh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.meibo888.top/gtqvsyswhc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtcdfhpgjy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cqqwz.cn/gtskbwhejn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yueranfly.top/gtcfpewvlc.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtcrwewkvr.html

Py:   copy.deepcopy(obj)
来源：http://hz.iojbl.cn/gtxswluhth.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenzaomai.com/gtxgkvxvzw.html

JS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtzqiavxfu.html

TS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtdwwebpnd.html


<!-- 参考信息 -->