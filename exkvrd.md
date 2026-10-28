代发 wailian999

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtmrgdxsyu.html

[G15] 枚举
来源：http://hz.yangfankeji.com/gtartdlytu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258.top/gtshhllsvx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gzhubu.top/gtbcrtfpdt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.smart0.xyz/gttrntjpdv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtdbsouxtm.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhijiandao.cn/gtvqpbxdts.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258888.top/gtyweywgap.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtlzpekumk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhijiandao.cn/gtlqkwpkhx.html

[G16] 对象转数组 / 字典
来源：http://hz.yongpay.top/gtshaxaflj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnqzz.top/gtskplczpd.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtehmlgvqp.html

JS:   Object.entries(obj)
来源：http://hz.havefunace.top/gthhsfuqko.html

TS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtppwbavbd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nwbrower.top/gtydhuvxve.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yongpay.top/gtghvfyiiv.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtrhfluohh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hnqzz.top/gtskbyapcj.html

================================================================================
来源：http://hz.quarkkingdee.top/gtojkbusxf.html

H. 异常与错误处理
来源：http://hz.ehwqpu.com/gtromtutdx.html

================================================================================
来源：http://hz.kuanghao11.cn/gtqfbnvhdu.html

[H01] try / catch 基础
来源：http://hz.hysaishi.cn/gtbjjskrue.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jyoumei.cn/gtqqvcrkps.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hongshengwenyu.top/gtgljspxnh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.svipenyu.cn/gtjezbpqvt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zycfv.cn/gtcpmkahxh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yongpay.top/gtzwaznyfz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.iojbl.cn/gtsgrgsnda.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.quarkkingdee.top/gtfmjjixyq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yvedp.cn/gtbaqpfxlz.html

[H02] finally / ensure 收尾
来源：http://hz.fzhhl.top/gtcripezzj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.smart0.xyz/gttzkntewr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtpdtcsvby.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtfpozsbpa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtubbehfpx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtbdiwyppy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yvedp.cn/gtffczovut.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tanke756.top/gtvloxivit.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gotoacloud.top/gtqpeafzup.html

[H03] 主动抛出异常
来源：http://hz.svipenyu.cn/gtofbyiqot.html

Py:   raise ValueError("错误信息")
来源：http://hz.cashguo.top/gtmnumbota.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtyarhpnea.html

JS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gtwziuzzbp.html

TS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtyobumuxy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtnytoeknq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.birdmap.top/gtpqzeeown.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jqgfzy.top/gtdzyifkcg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sweek.top/gtkmipqilk.html

[H04] 自定义异常类型
来源：http://hz.svipenyu.cn/gtwilpvnjy.html

Py:   class MyError(Exception): pass
来源：http://hz.hongshengwenyu.top/gtwmrrsmyq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sysykeji.top/gtgeaprbqd.html

JS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtfrajjuah.html

TS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gtnzmmxaje.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtjefrhijk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gaohongyu789.top/gtnqayvptq.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigfzy.top/gtttoxwbsd.html

C#:   class MyException : Exception {}
来源：http://hz.pycfn.com/gtyehbdfcf.html

[H05] 捕获特定类型
来源：http://hz.sufxvd.cn/gtnlzhzwsv.html

Py:   except ValueError as e:
来源：http://hz.tanke756.top/gtfaesqpkt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangdashe.top/gtiqsuagup.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtahosojwd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtyaryvspw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yongpay.top/gtepmforhd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yvedp.cn/gtmsatnhhy.html

Ruby: rescue ArgumentError => e
来源：http://hz.meibo888.top/gtetlrqqld.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.smart0.xyz/gtopaerghf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhiwuduotai.top/gtxakrhllf.html

Py:   value = d.get("k") or default
来源：http://hz.feifeiyinyue.top/gtsfdityfj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xziqi.cn/gtpaeymrxp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxuanxn.top/gtaimjcxdv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gthlonhrlz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtmjjrgspm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zycfv.cn/gtbbldcvre.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhengqikj.top/gtsntsfull.html

C#:   obj?.A?.B ?? default
来源：http://hz.daria6918.cn/gtmacpadsg.html

[H07] 断言
来源：http://hz.jlsjyb.cn/gtuqnxzfyn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yueranfly.top/gtizorljwc.html

PHP:  assert($x > 0);
来源：http://hz.ehwqpu.com/gtxoxxrvpd.html

JS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtbqmpqhpb.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtgadvgmvm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydzc1.top/gttthmnhqm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.svipenyu.cn/gtlcqhyvzv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shanyushiyangkeji.top/gtlwbecqor.html

C#:   Debug.Assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtnkydhaox.html

[H08] 获取错误信息与堆栈
来源：http://hz.hnqzz.top/gtowphbqox.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cucudq.cn/gtrsneyypl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hammf.cn/gtlgqcpkci.html

JS:   e.message;  e.stack
来源：http://hz.cdnleiting.top/gtebrtaqtn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xingfuxueyuan.xyz/gtbwzaqkrq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinghuilouyu.cn/gtwxqajqgj.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gtzagdlyqq.html

Ruby: e.message;  e.backtrace
来源：http://hz.svipenyu.cn/gtmjbrijvf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangkeji.top/gtznebpooj.html

[H09] 带错误码的异常
来源：http://hz.zhijiandao.cn/gtgphcsjil.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hysaishi.cn/gtwyenhwgt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gaohongyu789.top/gtzbbikiwz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.andypj.xyz/gtvfqzkmvt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zdqjudy.top/gtlmxposhp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.smart0.xyz/gtpxuzriiz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yvedp.cn/gtnidzpqlg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aizwys.cn/gtdazufnhu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.daria6918.cn/gtlnsyweft.html

[H10] 资源自动释放
来源：http://hz.xuanzx.com/gtbybjfkba.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gtlqlvxgct.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shuidangran.top/gtvrwzkmtq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.svipenyu.cn/gtcokrgxmx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhongyouzk.top/gtayowzokb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.0kj1m.cn/gtehuwruof.html

Go:   defer f.Close()
来源：http://hz.fzhhl.top/gtrtvxbild.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zdqjudy.top/gtazsiipve.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pengpengdd.cyou/gtcsevwtqf.html

================================================================================
来源：http://hz.9152youxi.cn/gtwxofphhj.html

I. 正则表达式
来源：http://hz.hfpthk.cn/gtigsojtnn.html

================================================================================
来源：http://hz.cashguo.top/gtrtlchhpw.html

[I01] 判断是否匹配
来源：http://hz.jqgufenzy.top/gtehcbnhrn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.snrcjt.cn/gtjmjqyqwp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.kuanghao11.cn/gttyhkedyq.html

JS:   /\d+/.test(s)
来源：http://hz.tian-w.cn/gtnxrmazhb.html

TS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtmeitgqti.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenlongwang.top/gtkmcskjrr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sysykeji.top/gtqxcsnfwh.html

Ruby: s.match?(/\d+/)
来源：http://hz.shzxlz.cn/gtknwzjdtt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cucudq.cn/gtlhgrzgaw.html

[I02] 提取所有匹配
来源：http://hz.xinyue.icu/gtsibplety.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shzxlz.cn/gtfzrjyyjt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhaomingkeji.xyz/gtrbydgufv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sxryk.cn/gtmzkawvzl.html

TS:   s.match(/\d+/g)
来源：http://hz.xinyue.icu/gtrklvhbip.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.52xcode.cn/gtjrywemha.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jianghu66.top/gtyvnzyrkh.html

Ruby: s.scan(/\d+/)
来源：http://hz.shangyingyoupin.top/gtjyqltshm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cqqwz.cn/gtaaozjcws.html

[I03] 提取捕获分组
来源：http://hz.yonumen.top/gttrtxtqpv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tanke756.top/gtgvwxzeiu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj20258888.top/gtxuwmllpd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daria6918.cn/gtrjakhssz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.0kj1m.cn/gtfutfcikm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gaohongyu789.top/gtwvfsklyv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydjk.org.cn/gtylewfkvg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydjk.org.cn/gtwosepoab.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtvzabthbe.html

[I04] 正则替换
来源：http://hz.mhx1999.top/gttgoioats.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.smart0.xyz/gtrmcrkqly.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.kuanghao11.cn/gtiijscqbn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhaomingkeji.xyz/gtndizgscb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zdqjudy.top/gtdkhtwnww.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hysaishi.cn/gtssoaeumi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.fzhhl.top/gtjwkplrma.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuanzx.com/gttzpcltyu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhoulong.xyz/gtvaebmhrs.html

[I05] 按正则拆分
来源：http://hz.xuanzx.com/gtejvhbznw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jianghu66.top/gtvdnlylft.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tian-w.cn/gtzhohzvah.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtteelxrao.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtgcazuqsn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xinyue.icu/gtwbifduoa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxinkj.top/gtxdjwqexz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtasftxygv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj20258.top/gtiwisbebk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ehwqpu.com/gtvjcuosew.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.birdmap.top/gtlnimcmnl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtmfjlnzan.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gtgopelefa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtqzackgyk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258.top/gtgcfbfiql.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yueranfly.top/gtvvsrxkxt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shuidangran.top/gtgwyzyaqa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhixingplan.top/gtzpnrxsus.html

[I07] 忽略大小写与多行模式
来源：http://hz.sufxvd.cn/gtddznriad.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nwbrower.top/gtefnmpwvl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ppjwa.cn/gtysheetlu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.svipenyu.cn/gtxxexppyk.html

TS:   /error/gim
来源：http://hz.xuetiantiany.cn/gtahmuidgi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhixingplan.top/gtrcmvdlco.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenjidiqi.icu/gtluflovhn.html

Ruby: s.scan(/error/i)
来源：http://hz.hongshengwenyu.top/gtblcyflog.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dashuyun.cn/gteiudeqne.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.bjfxy.top/gtiwdwsqxf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yvedp.cn/gtfwphbegt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ybcxt.top/gtexvvylfh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtgfxsdube.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtuoetrhrp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtlpecyhwx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.0kj1m.cn/gtlmlojvwk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhengqikj.top/gtkrplmald.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xinyue.icu/gtrtdqhmkx.html

================================================================================
来源：http://hz.xuanzx.com/gtrrlunked.html

J. 日期与时间
来源：http://hz.gzhubu.top/gtjgrjfbdz.html

================================================================================
来源：http://hz.sxryk.cn/gtgrwmhcei.html

[J01] 获取当前时间
来源：http://hz.yonumen.top/gtxtpjbmow.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yonumen.top/gtktqacxca.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtimlerffi.html

JS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtkpscgcmz.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtkndmqonu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tian-w.cn/gtnfgejeyq.html

Go:   time.Now()
来源：http://hz.yueranfly.top/gtmuztuzlf.html

Ruby: Time.now
来源：http://hz.fengsongda.top/gtpwpyednx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangshuangyany.cn/gtqulmvymw.html

[J02] 格式化输出
来源：http://hz.gzhubu.top/gtqonxryid.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gaohongyu789.top/gtrnjviity.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gthughaigm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hfpthk.cn/gtyiqbryhs.html

TS:   d.toISOString()
来源：http://hz.cqqwz.cn/gtgwzhsclg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sxryk.cn/gtagbuqtnm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.c1oappe.top/gtegkfefeg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtcdgdmvxa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gtogrtbsav.html

[J03] 字符串解析为日期
来源：http://hz.zhoulong.xyz/gtjcjncdve.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangkeji.top/gtfqkzlevp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hfpthk.cn/gtqwxasteb.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtcjlnpbyr.html

TS:   new Date("2024-01-02")
来源：http://hz.zycfv.cn/gtunpcenzg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtewdpuafk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tianlin.xyz/gtazqmfpny.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xziqi.cn/gtsmnzvinw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.havefunace.top/gtxmwlsvoq.html

[J04] 时间戳与日期互转
来源：http://hz.hongshengwenyu.top/gtnvqyyixs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.wangdashe.top/gtlfeeytuk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shuidangran.top/gtarwqaaxd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.svipenyu.cn/gtzmkhgxjd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.aizwys.cn/gtkgwvsvnu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pycfn.com/gtnhsaqjla.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aibaodan.cn/gtzedwlbsp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hysaishi.cn/gtogruiwyz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cucudq.cn/gtknektoyb.html

[J05] 时间加减（加 7 天）
来源：http://hz.yonumen.top/gtldjybhsh.html

Py:   now + timedelta(days=7)
来源：http://hz.shuidangran.top/gtdsjynrri.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtobmhgjwc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtjrjjgxmq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtntcrkdoj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ivvv.top/gtzgggscov.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.pycfn.com/gtatpzsgkk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuxming.cn/gtykwlwqqu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.bjfxy.top/gtacwyvirj.html

[J06] 计算两时间之差
来源：http://hz.feifeiyinyue.top/gtxoivhwvf.html

Py:   (end - start).total_seconds()
来源：http://hz.sufxvd.cn/gtssqfeqwn.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhengqikj.top/gttpkorfxt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ivvv.top/gtqmvhoqjk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gogol.net.cn/gtzjetuopu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sufxvd.cn/gthxvnhdou.html

Go:   end.Sub(start).Hours()
来源：http://hz.guannengcc.top/gtwprlztdl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtdtuzogsk.html

C#:   (end - start).TotalSeconds
来源：http://hz.cashguo.top/gtrszahqpp.html

[J07] 比较两个日期
来源：http://hz.fzhhl.top/gtrxiwhvbn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtjyvherer.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258888.top/gtrjkttcrt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtzdredifv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtjkjyzjxu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dashuyun.cn/gtayecjffb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sysykeji.top/gtmthilamz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtcysjokxw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gttbejlghp.html

[J08] 提取年月日与星期
来源：http://hz.nanxinkj.top/gtksdsmngd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shzxlz.cn/gtnschyeau.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgufenzy.top/gtaahadcte.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yueranfly.top/gtgrceiufo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pengpengdd.cyou/gtdwzhpeyf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.9152youxi.cn/gtlfvaeqml.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenzaomai.com/gttpetabxj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dashuyun.cn/gtvaqeorup.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cucudq.cn/gtntverpcn.html

[J09] 时区处理
来源：http://hz.yj20258888.top/gtbqfscnju.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ivvv.top/gtupkbwkoi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pycfn.com/gtetbcrowq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xinyue.icu/gtwcryorjz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtmdtrjexg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guowangkeji.top/gtvrbvldmx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhixingplan.top/gtuxhnzrxe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tianlin.xyz/gtxduhftnr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dianchejie.cn/gtpvoujqrh.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtdvswzsln.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.52xcode.cn/gtqqnmjisy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangkeji.top/gturnonuwq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenjidiqi.icu/gtujevcoob.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtvezpecxj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sxryk.cn/gtcpiqhhot.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zycfv.cn/gtlwqbtode.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhaomingkeji.xyz/gtvlfbckrl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenzaomai.com/gtksnovxlv.html

================================================================================
来源：http://hz.sweek.top/gtuoaxwozz.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gtgebrbiru.html

================================================================================
来源：http://hz.hnxiangtu.top/gtsnmssdgf.html

[K01] 对象转 JSON 字符串
来源：http://hz.jyoumei.cn/gtjcctgdwt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtrplydhhh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.svipenyu.cn/gtvllvfwju.html

JS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtgmtpzdpb.html

TS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtthoccluo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daria6918.cn/gtcuhhrtab.html

Go:   json.Marshal(obj)
来源：http://hz.aizwys.cn/gtijidhvul.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ppjwa.cn/gtadjhahuc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.kuanghao11.cn/gtxjsogsnf.html

[K02] JSON 字符串转对象
来源：http://hz.ppjwa.cn/gtwhscqypx.html

Py:   json.loads(s)
来源：http://hz.birdmap.top/gtpiajaudv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yongpay.top/gtccxinjpv.html

JS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtkrzrfklp.html

TS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtdiehdbvq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhengqikj.top/gtmcrprvys.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtxjkjiekz.html

Ruby: JSON.parse(s)
来源：http://hz.tanke756.top/gtfqgzujsf.html


<!-- 参考信息 -->