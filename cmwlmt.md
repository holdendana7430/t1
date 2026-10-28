代发 wailian999

[G14] 数据类 / record
来源：http://hz.fzhhl.top/gtrqpffhrt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangdashe.top/gtnslrdmcm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhixingplan.top/gtnefecniw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tian-w.cn/gtxnjfifyo.html

TS:   type User = { name: string; age: number };
来源：http://hz.0kj1m.cn/gtbkraxdsh.html

Java: record User(String name, int age) {}
来源：http://hz.ydzc1.top/gtwbjltwhr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.bjfxy.top/gtwhithvid.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhijiandao.cn/gteijznigw.html

C#:   record User(string Name, int Age);
来源：http://hz.zhoulong.xyz/gtjupwidfm.html

[G15] 枚举
来源：http://hz.zdqjudy.top/gtgidfchwk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.vqdsnc.cn/gtvvugiofp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.mhx1999.top/gtdbkwihvn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.haohaochexian.top/gtqfhtoanz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtqbefzabs.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gthhpsjqan.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zycfv.cn/gthjlypbgw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.meibo888.top/gtflfazfjt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtxrclchhy.html

[G16] 对象转数组 / 字典
来源：http://hz.andypj.xyz/gturafbnmo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xylfe.cn/gtbktkochf.html

PHP:  get_object_vars($obj);
来源：http://hz.jinyuanbaomall.cn/gtojnpocbu.html

JS:   Object.entries(obj)
来源：http://hz.ybcxt.top/gtoxjjkjrk.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtcnkhhumt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangtech.top/gtkgoautbc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinyuanbaomall.cn/gtuanilaiv.html

Ruby: obj.instance_variables
来源：http://hz.hnqzz.top/gtmbcmjogq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigfzy.top/gtklrhozsg.html

================================================================================
来源：http://hz.sweek.top/gtyewopxov.html

H. 异常与错误处理
来源：http://hz.ydzc1.top/gtydcxtbot.html

================================================================================
来源：http://hz.dianchejie.cn/gtaqudiviu.html

[H01] try / catch 基础
来源：http://hz.cashguo.top/gtjzuwistt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.havefunace.top/gtcjfpxtcb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daxiang520.top/gtehzufwfs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtgaienrcf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtpdibncpf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gtqjyrwsvf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.bjfxy.top/gtsqxvifdd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xinyue.icu/gteqaemgmr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgfzy.top/gtuelfhuyc.html

[H02] finally / ensure 收尾
来源：http://hz.zycfv.cn/gtkfucypai.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtpkhgmbvw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtiphgkawn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtqchycylk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtvhyhvrwi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtbivljpwu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhengqikj.top/gtmdnermrs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.birdmap.top/gtyneatacb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.fzhhl.top/gtrhzwkngv.html

[H03] 主动抛出异常
来源：http://hz.yj202588.top/gtikdkngpc.html

Py:   raise ValueError("错误信息")
来源：http://hz.redwolf501.top/gtmkbqhtam.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtiigxwncv.html

JS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtldkayotf.html

TS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtxnvabnvs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtwwjkfjaw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinyuanbaomall.cn/gtqftvrvvf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yanxiufei.cn/gtboquakos.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtocawicck.html

[H04] 自定义异常类型
来源：http://hz.bjfxy.top/gtokvtymfu.html

Py:   class MyError(Exception): pass
来源：http://hz.xinyue.icu/gtgpvnrlkv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtklfugysd.html

JS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gtzkhhdvex.html

TS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtbxmqxert.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtmhxqafav.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dianchejie.cn/gtgscysorf.html

Ruby: class MyError < StandardError; end
来源：http://hz.cheryme.top/gtbrxkaxey.html

C#:   class MyException : Exception {}
来源：http://hz.gzhubu.top/gtzgejhsqn.html

[H05] 捕获特定类型
来源：http://hz.cashguo.top/gtovpujqvj.html

Py:   except ValueError as e:
来源：http://hz.yueranfly.top/gtcltyjntk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fengsongda.top/gtkkxzqjcn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangdashe.top/gtcztqpudj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtvrhagroa.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxuanxn.top/gtxfgpnqoq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhaomingkeji.xyz/gtbikvkmbz.html

Ruby: rescue ArgumentError => e
来源：http://hz.jlsjyb.cn/gtmgbybghc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hysaishi.cn/gtmesrsgyu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.316326.xyz/gtlizvojxc.html

Py:   value = d.get("k") or default
来源：http://hz.ehwqpu.com/gtuihpslsw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtuokhwswk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtxjmvprih.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtedvbjabv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yongpay.top/gtwoathagr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sxryk.cn/gtaaervfcx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtviuyzrvl.html

C#:   obj?.A?.B ?? default
来源：http://hz.pengpengdd.cyou/gtpnjllcyl.html

[H07] 断言
来源：http://hz.jinqigfzy.top/gtcixfpnbn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.andypj.xyz/gtdjsmfuto.html

PHP:  assert($x > 0);
来源：http://hz.dashuyun.cn/gteypsdviq.html

JS:   console.assert(x > 0);
来源：http://hz.9152youxi.cn/gtwnoebwmm.html

TS:   console.assert(x > 0);
来源：http://hz.svipenyu.cn/gtdhsvgqcy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgfzy.top/gtervpiffv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.vqdsnc.cn/gtrpuyqzpj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xinyue.icu/gtjlevzrhx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shuidangran.top/gtjodftfjr.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangtech.top/gtujyyvgeg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenjidiqi.icu/gtigcuyuhg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxinkj.top/gtwxlyukjs.html

JS:   e.message;  e.stack
来源：http://hz.316326.xyz/gtbbmpglul.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ivvv.top/gtoaattzhn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gotoacloud.top/gtjdthblqh.html

Go:   err.Error()
来源：http://hz.zhengqikj.top/gtbsrvaede.html

Ruby: e.message;  e.backtrace
来源：http://hz.hfpthk.cn/gtpxtduejp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tianlin.xyz/gtfzjezcnu.html

[H09] 带错误码的异常
来源：http://hz.yuxming.cn/gtfzjsartn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tanke756.top/gtvloiecny.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pengpengdd.cyou/gtjlscyjgm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aizwys.cn/gtiqjhvtmi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.0kj1m.cn/gtsnzmcvoy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenlongwang.top/gtstufwkdh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenzaomai.com/gthlgoqdzi.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinyuanbaomall.cn/gtoudgvenj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj20258.top/gtuqiooafi.html

[H10] 资源自动释放
来源：http://hz.pycfn.com/gtzcwvzmbt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shuidangran.top/gtkhjxqgms.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dashuyun.cn/gtsxlsrccz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gthgsigttw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtzvvqyibd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.haohaochexian.top/gttkcinrlw.html

Go:   defer f.Close()
来源：http://hz.c1oappe.top/gttkvqcqfw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hfpthk.cn/gtagtrxbas.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinghuilouyu.cn/gtmsqkofqs.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpokfgzqp.html

I. 正则表达式
来源：http://hz.snrcjt.cn/gtmnirkwwm.html

================================================================================
来源：http://hz.fzhhl.top/gtledlsnvx.html

[I01] 判断是否匹配
来源：http://hz.fengsongda.top/gtldppsotj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gogol.net.cn/gtvubnnkmc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aibaodan.cn/gtqfpztadn.html

JS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtlzoeqgut.html

TS:   /\d+/.test(s)
来源：http://hz.kuanghao11.cn/gtpghmealf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tian-w.cn/gtabiedczg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhoulong.xyz/gtogqdhvji.html

Ruby: s.match?(/\d+/)
来源：http://hz.yvedp.cn/gtwcasiddo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nanxuanxn.top/gtphekhjci.html

[I02] 提取所有匹配
来源：http://hz.hammf.cn/gtkfzsokhj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigufen.top/gthrqlwzsl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hywenlv.cn/gtkzcaqdfm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tian-w.cn/gthmehxfsm.html

TS:   s.match(/\d+/g)
来源：http://hz.gzhubu.top/gtsuycazby.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.bjfxy.top/gtjkbijwgi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtmgdhpucr.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gtdsqlaxkp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zycfv.cn/gtuwzcdbup.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gticgmievr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hysaishi.cn/gtugitmldj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.quarkkingdee.top/gtesimvate.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhiwuduotai.top/gtgyaqqnot.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gaohongyu789.top/gtnkjvuusc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gtmvcrgxti.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.bjfxy.top/gtjsuoaxjw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zycfv.cn/gtgliapnaf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gzhubu.top/gtnsnqwnwd.html

[I04] 正则替换
来源：http://hz.vqdsnc.cn/gtugikpooe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jianghu66.top/gtbaatovcu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.haohaochexian.top/gtstotwokk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtzikgfxae.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtfgcmgxbw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jiagoushi.top/gthocatlzj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgufenzy.top/gtjjnmodib.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgfzy.top/gtqsobkmnq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nwbrower.top/gtjzphjuxm.html

[I05] 按正则拆分
来源：http://hz.hywenlv.cn/gtvdzscors.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.kuanghao11.cn/gtjoudibto.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ydjk.org.cn/gtijgftear.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtiygrdvcb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtfkijfkvb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zycfv.cn/gtelynectl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtramryacb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtacyrrodk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gogol.net.cn/gtzzmtpsth.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nwbrower.top/gtqgihakua.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtcahfccey.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenlongwang.top/gtktnzzvmi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtvkzrkghf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gtyqdbrfqp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shuidangran.top/gttcswkwwk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxinkj.top/gtscdtrado.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hywenlv.cn/gthyvwcusp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtqxcynezo.html

[I07] 忽略大小写与多行模式
来源：http://hz.ywan-chungtsiang.top/gtsrzrndgh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gtelfwpbbe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ydjk.org.cn/gtuosrkecj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xylfe.cn/gtrsvsuicl.html

TS:   /error/gim
来源：http://hz.ybcxt.top/gtexgzxqig.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guowangkeji.top/gtfzvgublw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hammf.cn/gtxrhwbkgs.html

Ruby: s.scan(/error/i)
来源：http://hz.zycfv.cn/gtrwdvujxy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhaomingkeji.xyz/gtsgyjixip.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sweek.top/gtpqdxftuj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangdashe.top/gtvyhjgkna.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gthzwgmkzq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtmynrvklo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gtrabnnyti.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gotoacloud.top/gtsqfihtex.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigfzy.top/gtpjbbfinv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ybcxt.top/gtcezkosbv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.mhx1999.top/gtbkyuhkwu.html

================================================================================
来源：http://hz.shuidangran.top/gtjhyyuggd.html

J. 日期与时间
来源：http://hz.sufxvd.cn/gtrgniwijs.html

================================================================================
来源：http://hz.shuidangran.top/gtmuezfbxu.html

[J01] 获取当前时间
来源：http://hz.mhx1999.top/gtrwpxsosg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.iojbl.cn/gtehvuegly.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtsvtabjfz.html

JS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtglatmyhk.html

TS:   new Date();  Date.now()
来源：http://hz.hywenlv.cn/gtrfaxomcw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cashguo.top/gtblkpiate.html

Go:   time.Now()
来源：http://hz.yanxiufei.cn/gtgopfelxk.html

Ruby: Time.now
来源：http://hz.yongpay.top/gteqjktiyq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangdashe.top/gtzpjvqotj.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtbwzlvdev.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtjklzipus.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jiagoushi.top/gtoykrqpns.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtkvqvadgx.html

TS:   d.toISOString()
来源：http://hz.tianlin.xyz/gtilrkavom.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.svipenyu.cn/gttufumtay.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.haohaochexian.top/gtpiwdsflo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtwjjllnht.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xziqi.cn/gtqhpdueuz.html

[J03] 字符串解析为日期
来源：http://hz.yonumen.top/gtsnymrdsm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nwbrower.top/gtkseamfrp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gthhuvioth.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtnwlxodbz.html

TS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtqgtaernw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtitdyyyrx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.aibaodan.cn/gtqsteukpk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtsaikubmh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gtksbpdkpg.html

[J04] 时间戳与日期互转
来源：http://hz.ydjk.org.cn/gtxrmxloau.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.meibo888.top/gtgwwhgfhc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aizwys.cn/gtaeodbgss.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gotoacloud.top/gtelagfikk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yongpay.top/gtsuvwmrjh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shuidangran.top/gtxnsmtvbq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gotoacloud.top/gttggmnaic.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fengsongda.top/gtjrfihzam.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yvedp.cn/gtkclkiliu.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangshuangyany.cn/gtdsdxsxex.html

Py:   now + timedelta(days=7)
来源：http://hz.tian-w.cn/gtwagkwjsz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tanke756.top/gtxuafapid.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtnbuxwzsh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtlpoboafi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hywenlv.cn/gtjibnlbjs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gzhubu.top/gtidynfbuz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenzaomai.com/gttiuhlfxz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnqzz.top/gtxugtftha.html

[J06] 计算两时间之差
来源：http://hz.bjfxy.top/gtpbgbpncz.html

Py:   (end - start).total_seconds()
来源：http://hz.yuxming.cn/gtudpvaplk.html

PHP:  $end->diff($start)->days;
来源：http://hz.9152youxi.cn/gtuubmbnwj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hysaishi.cn/gtrriztruu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgfzy.top/gthgsyjbsf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guannengcc.top/gtebkznehr.html

Go:   end.Sub(start).Hours()
来源：http://hz.meibo888.top/gtozpncyiw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shanyushiyangkeji.top/gtadjnryni.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigfzy.top/gtkuyksnpw.html

[J07] 比较两个日期
来源：http://hz.jyoumei.cn/gtxlncsqfl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtppgnuqrq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sufxvd.cn/gtdwqptotr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtudsntyqz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtmbykrjui.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.meibo888.top/gtmwcayghm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj202588.top/gtafmfvwwr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtlbfvprph.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtfmowfbhs.html

[J08] 提取年月日与星期
来源：http://hz.jinghuilouyu.cn/gttlfgkpwx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yangfankeji.com/gthjtycoxj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigufen.top/gtbqqdxbdf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ybcxt.top/gttitwjjnh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.316326.xyz/gtcvelgszv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zdqjudy.top/gthjbdvobw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gtkgvlquis.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ehwqpu.com/gtzkmaubog.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zycfv.cn/gthltechza.html

[J09] 时区处理
来源：http://hz.316326.xyz/gtpfcnpaoi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xylfe.cn/gtpblteegh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yongpay.top/gtqfbmrhql.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtxsmrofgj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtjakzazfi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxinkj.top/gtrwpxegvr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnxiangtu.top/gtqxlcxnmn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gtnswjurdf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cdnleiting.top/gtrqqlvltq.html

[J10] 取今天 / 本月第一天
来源：http://hz.daxiang520.top/gtwrhjgqwm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gaohongyu789.top/gtycnhatph.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.andypj.xyz/gthptwtnlh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jyoumei.cn/gtlmmvwodi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtqqmruojo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenlongwang.top/gtvncpsskw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.snrcjt.cn/gtcrmccapy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gotoacloud.top/gtcmhqolsv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gtrgnalrbu.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtvratkezi.html

K. JSON 与序列化
来源：http://hz.jlsjyb.cn/gtbupakuua.html

================================================================================
来源：http://hz.ehwqpu.com/gtkdgmkfje.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenzaomai.com/gtuzndiicf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtaocojina.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtqonbqdpn.html

JS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtbbjhyjqv.html

TS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gttsnbttel.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.kuanghao11.cn/gttootwxwl.html

Go:   json.Marshal(obj)
来源：http://hz.haohaochexian.top/gtgxfatyjy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cashguo.top/gtixmiuyhj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shangyingyoupin.top/gtjnxwgtxj.html


<!-- 参考信息 -->