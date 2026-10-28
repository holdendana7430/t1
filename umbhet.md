代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tianlin.xyz/gtdoimggro.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ywan-chungtsiang.top/gtomqvpgfr.html

Java: enum Color { RED, GREEN }
来源：http://hz.iojbl.cn/gtiqmnqqsk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cashguo.top/gtibkdavdu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.smart0.xyz/gtnghwasjd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtwoldmjrc.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgfzy.top/gtjpdmjavz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cheryme.top/gtouyjlbuq.html

PHP:  get_object_vars($obj);
来源：http://hz.pengpengdd.cyou/gttnyslrjr.html

JS:   Object.entries(obj)
来源：http://hz.sweek.top/gtwixeofdw.html

TS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtvfpvemoz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnxiangtu.top/gtycmkbutt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fzhhl.top/gtclaemvsu.html

Ruby: obj.instance_variables
来源：http://hz.c1oappe.top/gtqbrfaose.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangdashe.top/gthkzhgesd.html

================================================================================
来源：http://hz.havefunace.top/gtpjdvfedk.html

H. 异常与错误处理
来源：http://hz.jinyuanbaomall.cn/gtebipjrpv.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwtimkvob.html

[H01] try / catch 基础
来源：http://hz.sysykeji.top/gtdggxjdjx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangkeji.top/gtswejsppz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuanzx.com/gtlfruqswu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.9152youxi.cn/gtzhsecbzm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258888.top/gtegftgxwa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhiwuduotai.top/gtqyoflyno.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gtvmjmwuxb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhaomingkeji.xyz/gtnddxttxo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhijiandao.cn/gtxzgaxaho.html

[H02] finally / ensure 收尾
来源：http://hz.iojbl.cn/gtdnqfltpj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jqgufenzy.top/gtqpbchigk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtrmtexhzo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gthlsghxfc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtsilvjxdu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtfuhyybcu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigufen.top/gtgqksqgbr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sufxvd.cn/gtgftxiimz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.kuanghao11.cn/gtsphmnnce.html

[H03] 主动抛出异常
来源：http://hz.0kj1m.cn/gtrpnfdydh.html

Py:   raise ValueError("错误信息")
来源：http://hz.guannengcc.top/gtrfreqcvz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtgvdoszzk.html

JS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtgnlxwwoo.html

TS:   throw new Error("错误信息");
来源：http://hz.cucudq.cn/gthospgtrj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtbgchzurf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sufxvd.cn/gtvmzdfunr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258.top/gtqtesyean.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sweek.top/gtyprlyhqf.html

[H04] 自定义异常类型
来源：http://hz.aizwys.cn/gttzmieamg.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gtkwueagym.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.316326.xyz/gtoffcqvyi.html

JS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtjlkxsmew.html

TS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gteldiqqic.html

Java: class MyException extends RuntimeException {}
来源：http://hz.andypj.xyz/gtxmwlklck.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fengsongda.top/gtodyngoyg.html

Ruby: class MyError < StandardError; end
来源：http://hz.andypj.xyz/gtuhiirboo.html

C#:   class MyException : Exception {}
来源：http://hz.0kj1m.cn/gtwbcljtse.html

[H05] 捕获特定类型
来源：http://hz.zycfv.cn/gtcgjxoxnr.html

Py:   except ValueError as e:
来源：http://hz.gotoacloud.top/gtpguuztex.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xingfuxueyuan.xyz/gttcondfqi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtioalmnjf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydzc1.top/gtisstvjxr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shanyushiyangkeji.top/gtnriavszw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dianchejie.cn/gtcswoyaqr.html

Ruby: rescue ArgumentError => e
来源：http://hz.tanke756.top/gtykvjzqnn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gaohongyu789.top/gtunnoprmy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.iojbl.cn/gtolxtydef.html

Py:   value = d.get("k") or default
来源：http://hz.meibo888.top/gtyuacmnae.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.dianchejie.cn/gtyadxrjfc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtwbnsvkas.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtcbpaoegl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangkeji.top/gtcnxbzuum.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtwlqthkxn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cucudq.cn/gtnbammiuk.html

C#:   obj?.A?.B ?? default
来源：http://hz.bjfxy.top/gtecqnypfg.html

[H07] 断言
来源：http://hz.birdmap.top/gtfydlndra.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ywan-chungtsiang.top/gtqvlklseo.html

PHP:  assert($x > 0);
来源：http://hz.chenzaomai.com/gtrsyzvqar.html

JS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtsjwdexfm.html

TS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtclhojhrs.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinyuanbaomall.cn/gtcodxqaqn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tianlin.xyz/gtpbquoedu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jyoumei.cn/gtdfwncivh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtnvtrqquj.html

[H08] 获取错误信息与堆栈
来源：http://hz.hnxiangtu.top/gtokktknzj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.9152youxi.cn/gtlbujbhcj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtnqyauajc.html

JS:   e.message;  e.stack
来源：http://hz.c1oappe.top/gtipjiphvg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fzhhl.top/gttcaqbwux.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yueranfly.top/gtzwarjjyi.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtplzsiqbc.html

Ruby: e.message;  e.backtrace
来源：http://hz.feifeiyinyue.top/gtxaxiuohw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuanzhike.top/gtdmcrfaum.html

[H09] 带错误码的异常
来源：http://hz.mhx1999.top/gtlkspshft.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.svipenyu.cn/gtcdaaynfg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.mhx1999.top/gtifbmkmut.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258888.top/gtrkwiwqkk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shangyingyoupin.top/gtbfaslowa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jqgufenzy.top/gtacakxivp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangdashe.top/gtktshjwlp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenlongwang.top/gtfebhjucy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gtrdpmcgck.html

[H10] 资源自动释放
来源：http://hz.nwbrower.top/gtfzllraxv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nwbrower.top/gtxlylgdfy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gtottsvijk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gtqdpbirln.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtjqtytabl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daria6918.cn/gtipbhraln.html

Go:   defer f.Close()
来源：http://hz.aibaodan.cn/gttfvwwzms.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhengqikj.top/gtvinnkukt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigfzy.top/gtntmehbtx.html

================================================================================
来源：http://hz.yj20258.top/gticmppbiv.html

I. 正则表达式
来源：http://hz.dianchejie.cn/gtzvxfymcb.html

================================================================================
来源：http://hz.svipenyu.cn/gtimwguvlq.html

[I01] 判断是否匹配
来源：http://hz.dashuyun.cn/gtjmznpqym.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.andypj.xyz/gtdwnrfbkb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.pycfn.com/gtlsbghxez.html

JS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtawdvmmdc.html

TS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gthhbawkbh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tanke756.top/gtdmhjegxr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258.top/gtmmblwxfg.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydjk.org.cn/gtqktzsqes.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aizwys.cn/gtsasvoqvp.html

[I02] 提取所有匹配
来源：http://hz.52xcode.cn/gtlvqjehki.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dianchejie.cn/gtolmcnewb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhengqikj.top/gtzxjkqcvw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.kuanghao11.cn/gtoqvvmuvm.html

TS:   s.match(/\d+/g)
来源：http://hz.iojbl.cn/gtyxlqyptk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigufen.top/gtwrigowkc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ivvv.top/gtgxatqguk.html

Ruby: s.scan(/\d+/)
来源：http://hz.dashuyun.cn/gtyplctrff.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jlsjyb.cn/gtxtkfdmxn.html

[I03] 提取捕获分组
来源：http://hz.guowangkeji.top/gtchuyypsx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xinyue.icu/gtlzfkxcsc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xingfuxueyuan.xyz/gtiywuqqsd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cashguo.top/gtvswcblxa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guowangkeji.top/gtnpulpvvf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cucudq.cn/gtosctesag.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pengpengdd.cyou/gtbebgwogf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinyuanbaomall.cn/gtfjubpthm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cheryme.top/gtczopvcwk.html

[I04] 正则替换
来源：http://hz.hfpthk.cn/gtcukffvgu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.havefunace.top/gtcfcqlfwz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtqzaqtczy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuanzhike.top/gttfjthjuh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtcjikfmjf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yongpay.top/gtqvvymfje.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sufxvd.cn/gtjunpybqy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ybcxt.top/gtgqnhowzb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pengpengdd.cyou/gtlbjkhriu.html

[I05] 按正则拆分
来源：http://hz.shuidangran.top/gtsjemejsi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj202588.top/gtbtciatrn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtwoqgucsm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gthckedpqx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtigslestn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.meibo888.top/gtxxhaoydn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.316326.xyz/gtkuvryqtd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtqknititd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.snrcjt.cn/gthjyhhhav.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gtwetqwbuq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shangyingyoupin.top/gttxorfqke.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guannengcc.top/gtvaizvzol.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gtjuagemxq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtsvfqcyix.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hammf.cn/gtuxmvcpsb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.9152youxi.cn/gtjyjqlsmg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.snrcjt.cn/gtadmfxxad.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gthecnnvji.html

[I07] 忽略大小写与多行模式
来源：http://hz.yonumen.top/gtyknryixb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuanzhike.top/gtpoyxexzy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zdqjudy.top/gtckwrmetu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.snrcjt.cn/gtslhqaqet.html

TS:   /error/gim
来源：http://hz.jianghu66.top/gtdqwdxroz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fzhhl.top/gtuchhqknn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gtddkffszk.html

Ruby: s.scan(/error/i)
来源：http://hz.gotoacloud.top/gtqudtlfgy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sweek.top/gthgnpkhpj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenzaomai.com/gtsghhnrnr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yuxming.cn/gtymynuvqh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.aizwys.cn/gtvwiahjoj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtkcrjykey.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cqqwz.cn/gtkmtynjnf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gtzjgyhzey.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuanzhike.top/gtagnqvuff.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cqqwz.cn/gthkywjdop.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.mhx1999.top/gtkkvkyojh.html

================================================================================
来源：http://hz.52xcode.cn/gtfdmkuukb.html

J. 日期与时间
来源：http://hz.shzxlz.cn/gtxsqewowl.html

================================================================================
来源：http://hz.zhengqikj.top/gtxyqmgxqs.html

[J01] 获取当前时间
来源：http://hz.guowangkeji.top/gtmemdqwyv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cdnleiting.top/gthmistjmq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigfzy.top/gtzpjmbxcn.html

JS:   new Date();  Date.now()
来源：http://hz.gaohongyu789.top/gtfnsrnctg.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtodvxbfvc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gotoacloud.top/gtessyfawn.html

Go:   time.Now()
来源：http://hz.andypj.xyz/gtffdiduse.html

Ruby: Time.now
来源：http://hz.zhongyouzk.top/gtrxvumktp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxinkj.top/gtobedbfbx.html

[J02] 格式化输出
来源：http://hz.svipenyu.cn/gtvagkerjn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtaszshidc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtfdtllxoc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.meibo888.top/gtvrzuentv.html

TS:   d.toISOString()
来源：http://hz.ehwqpu.com/gtbjbyswis.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenlongwang.top/gtiotqbjsl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hammf.cn/gtaoatemgf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtroweoevu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gtvoqapopn.html

[J03] 字符串解析为日期
来源：http://hz.yuxming.cn/gtudyrwslj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.havefunace.top/gtxdoztcio.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hnxiangtu.top/gtzgptjxug.html

JS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtqktupemm.html

TS:   new Date("2024-01-02")
来源：http://hz.tian-w.cn/gturuzbjhu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj202588.top/gtqbvxkdus.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigufen.top/gtcbgrtbss.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yangfankeji.com/gtcdvuccsu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigufen.top/gtbqtchssi.html

[J04] 时间戳与日期互转
来源：http://hz.meibo888.top/gtlmdzpxze.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pengpengdd.cyou/gtmecqxbpe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hongshengwenyu.top/gtffcdveuy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.feifeiyinyue.top/gtmmkjutty.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fzhhl.top/gtzgkwfvem.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinyuanbaomall.cn/gtygvzavkb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cashguo.top/gtcskvdftw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.aibaodan.cn/gtyvistkeu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhixingplan.top/gtxgenrzeg.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxinkj.top/gtxkuyummo.html

Py:   now + timedelta(days=7)
来源：http://hz.redwolf501.top/gtuepmooap.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hywenlv.cn/gtglsydwgj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtpjvtkvqc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtmyoukvqe.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangshuangyany.cn/gtlpnrblpw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cdnleiting.top/gtujmollai.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fengsongda.top/gtbbnetnws.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gtbokoqzfh.html

[J06] 计算两时间之差
来源：http://hz.yvedp.cn/gtobsfzfmg.html

Py:   (end - start).total_seconds()
来源：http://hz.sysykeji.top/gtlycsaoka.html

PHP:  $end->diff($start)->days;
来源：http://hz.yonumen.top/gtqpuroyky.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guowangkeji.top/gtixcoquvh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hywenlv.cn/gtxohlxbki.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhongyouzk.top/gtuvuxxgrc.html

Go:   end.Sub(start).Hours()
来源：http://hz.daria6918.cn/gtrldwubyp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aibaodan.cn/gtyjcpgjkb.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtjcqulsuu.html

[J07] 比较两个日期
来源：http://hz.wangshuangyany.cn/gtihdhdskl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtcjdgsvvq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.andypj.xyz/gtzgwjwbjn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtheqfpell.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtiacsqrgg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daria6918.cn/gtqgfftxrs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.svipenyu.cn/gthcjhywjs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gttnhqkpog.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtspgzqvqk.html

[J08] 提取年月日与星期
来源：http://hz.wangdashe.top/gthvsziaae.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zdqjudy.top/gtitnkimnc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuanzx.com/gtrbggptxj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenlongwang.top/gtbuqkuxzd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtfanhsdxl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.andypj.xyz/gttowniyxd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.9152youxi.cn/gtdhutvcbf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtxqbtjjho.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydzc1.top/gtypfpybnx.html

[J09] 时区处理
来源：http://hz.zycfv.cn/gtxzgxqnsy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxinkj.top/gtbbujcejk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hfpthk.cn/gteqafleop.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtpabwaijo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtqipsgoyu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yangfankeji.com/gtjdeiyjln.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinyuanbaomall.cn/gthbvqmubu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtemvsdqdj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangkeji.top/gtxxzhyjop.html

[J10] 取今天 / 本月第一天
来源：http://hz.yueranfly.top/gtjinpvunt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.kuanghao11.cn/gtjwjltwtf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yanxiufei.cn/gtwmxyzeeg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ppjwa.cn/gtsplgvrqk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj202588.top/gtgfpldahs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuanzx.com/gtutwjyuvy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jianghu66.top/gtguveugqa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhengqikj.top/gtcyrukdee.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258888.top/gtslrzccwb.html

================================================================================
来源：http://hz.zdqjudy.top/gtocjrhuhh.html

K. JSON 与序列化
来源：http://hz.hongshengwenyu.top/gttlwwzjkn.html

================================================================================
来源：http://hz.hfpthk.cn/gtssfylmaq.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtepnpehaz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cashguo.top/gtdbbpsxfw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtqmclbfma.html

JS:   JSON.stringify(obj)
来源：http://hz.meibo888.top/gtgbyvapfw.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtsfisojii.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sysykeji.top/gtipopjksv.html

Go:   json.Marshal(obj)
来源：http://hz.kuanghao11.cn/gthacbekcn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhengqikj.top/gtdawgewlp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yvedp.cn/gtoehxkyud.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gtbhrlttap.html

Py:   json.loads(s)
来源：http://hz.andypj.xyz/gtkqnyxghr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guannengcc.top/gtueexavhj.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gttppxwopk.html

TS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtvrhgvopc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenzaomai.com/gtjirsqvxv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gthmranqse.html

Ruby: JSON.parse(s)
来源：http://hz.yangfankeji.com/gtjzhhoxbv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenlongwang.top/gtludxdymt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gttpteohlb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtwcumxiul.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtjlovyrfs.html


<!-- 参考信息 -->