代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.aizwys.cn/gtgqgcckxv.html

Java: record User(String name, int age) {}
来源：http://hz.zhixingplan.top/gtvhrozbfw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jianghu66.top/gtjklfdztg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pengpengdd.cyou/gtbtiwnard.html

C#:   record User(string Name, int Age);
来源：http://hz.xuetiantiany.cn/gthjujsjxz.html

[G15] 枚举
来源：http://hz.fzhhl.top/gtrmyddvao.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yanxiufei.cn/gtiiqlxdlu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gzhubu.top/gtdatsyrzn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jlsjyb.cn/gtwawdopeh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtpkokfjbo.html

Java: enum Color { RED, GREEN }
来源：http://hz.cucudq.cn/gtibyrbksw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xziqi.cn/gtlgoeyzqt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tanke756.top/gtndarosdb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtioistubk.html

[G16] 对象转数组 / 字典
来源：http://hz.xziqi.cn/gtgodscolc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guowangkeji.top/gtlcbxqniw.html

PHP:  get_object_vars($obj);
来源：http://hz.yuanzhike.top/gtjzxkhzud.html

JS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gtgckxruse.html

TS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtabrznkni.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.svipenyu.cn/gtictafeqb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sweek.top/gtvpomsrsc.html

Ruby: obj.instance_variables
来源：http://hz.yangfankeji.com/gtmxsbapgs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigfzy.top/gtdyxxssem.html

================================================================================
来源：http://hz.yueranfly.top/gtwcivlkja.html

H. 异常与错误处理
来源：http://hz.dashuyun.cn/gthhqzpxiz.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtncsvfamc.html

[H01] try / catch 基础
来源：http://hz.nanxinkj.top/gtfqphqykn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.andypj.xyz/gtecagltvf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guannengcc.top/gtfsvfuzja.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ehwqpu.com/gtdfsagtlk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daxiang520.top/gtrdnuacvw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gaohongyu789.top/gtzmkspqws.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinyuanbaomall.cn/gtealfkpzf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zycfv.cn/gtnyjwgxbx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.smart0.xyz/gtujvheptw.html

[H02] finally / ensure 收尾
来源：http://hz.andypj.xyz/gtipzltugq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.vqdsnc.cn/gtvtebyjeq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtewfzkxsp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtuikamhic.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gttevagseh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtxfsvpvas.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gzhubu.top/gtpkgpkbss.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.birdmap.top/gtfymvfnpw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigfzy.top/gtmxlyhqpa.html

[H03] 主动抛出异常
来源：http://hz.c1oappe.top/gtxtsitbyi.html

Py:   raise ValueError("错误信息")
来源：http://hz.fengsongda.top/gtjmqnkctv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtlkxrjtlx.html

JS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtzerkbbzh.html

TS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtrnwufmig.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtfyobsnbn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yueranfly.top/gtbqxnauqs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.redwolf501.top/gtvoakyzwi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cheryme.top/gtfwgdhvaf.html

[H04] 自定义异常类型
来源：http://hz.xuetiantiany.cn/gtfrnyguns.html

Py:   class MyError(Exception): pass
来源：http://hz.xingfuxueyuan.xyz/gtgwfzscad.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xingfuxueyuan.xyz/gtoluvkqhx.html

JS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtvgfqvwrv.html

TS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtuxkumsbz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtycxsllrh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangkeji.top/gtwcgxrack.html

Ruby: class MyError < StandardError; end
来源：http://hz.kuanghao11.cn/gtrzivymxe.html

C#:   class MyException : Exception {}
来源：http://hz.zhoulong.xyz/gtvwvrfvgk.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gthuldpunp.html

Py:   except ValueError as e:
来源：http://hz.sweek.top/gtgcjhyclj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigfzy.top/gtdfdqmqgx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtxbxsfzgh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yongpay.top/gtxubzqlzk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgufenzy.top/gtmbsjsnkj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj202588.top/gtposdsqtj.html

Ruby: rescue ArgumentError => e
来源：http://hz.tian-w.cn/gtztealump.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sufxvd.cn/gtxlrzejwa.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ybcxt.top/gtoynfvkfl.html

Py:   value = d.get("k") or default
来源：http://hz.yanxiufei.cn/gtjnavhggf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuetiantiany.cn/gthrdliaxl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuetiantiany.cn/gtgbpioozc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtrfgmsoiv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtpnyglimr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtyjxgufqd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenlongwang.top/gtclxlsmlf.html

C#:   obj?.A?.B ?? default
来源：http://hz.9152youxi.cn/gthdcdzfqy.html

[H07] 断言
来源：http://hz.havefunace.top/gtscuzmkmu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhixingplan.top/gtojouprvv.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtyboeczdc.html

JS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtxbvvdxeb.html

TS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtpzjvlirf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hammf.cn/gtgvjffzzb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.316326.xyz/gtlfccqvaq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ywan-chungtsiang.top/gtivarqfkw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.dianchejie.cn/gtrmqzygko.html

[H08] 获取错误信息与堆栈
来源：http://hz.ehwqpu.com/gtvhqlgnxa.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zycfv.cn/gtefwzfebg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtmkslmsnx.html

JS:   e.message;  e.stack
来源：http://hz.zycfv.cn/gtoetroese.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.mhx1999.top/gtmwcdketz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.c1oappe.top/gtwvjxnwtl.html

Go:   err.Error()
来源：http://hz.tian-w.cn/gtgakswdhk.html

Ruby: e.message;  e.backtrace
来源：http://hz.svipenyu.cn/gtyijeiiqm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hongshengwenyu.top/gtywwpqghf.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtppeuhrwg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gotoacloud.top/gtmfpaofux.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtlfyxaacx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guannengcc.top/gtojlovnpc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtszvwuuuz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.bjfxy.top/gtwwzintva.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhiwuduotai.top/gtrnwyemhk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnxiangtu.top/gtmpnabhec.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ivvv.top/gtiupyhsoa.html

[H10] 资源自动释放
来源：http://hz.shanyushiyangkeji.top/gtabhjwndf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydjk.org.cn/gtgdyofukt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cdnleiting.top/gtxikulfsz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtgdfuzxlg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtlhwyeyqs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ywan-chungtsiang.top/gtolxplvzh.html

Go:   defer f.Close()
来源：http://hz.hammf.cn/gtemrjwued.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sufxvd.cn/gtfoenpqpx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenlongwang.top/gtelavflfx.html

================================================================================
来源：http://hz.yuxming.cn/gtcbdzzghf.html

I. 正则表达式
来源：http://hz.pycfn.com/gtivzbghhx.html

================================================================================
来源：http://hz.andypj.xyz/gthnhklttc.html

[I01] 判断是否匹配
来源：http://hz.chenjidiqi.icu/gtohrkqsfb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yvedp.cn/gtagslimqw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fengsongda.top/gthsfyocgp.html

JS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gtziobzljt.html

TS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gtzpeceriw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yj20258888.top/gtdshjwoye.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xziqi.cn/gtuxxxetdq.html

Ruby: s.match?(/\d+/)
来源：http://hz.ehwqpu.com/gtrcumwjtq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gogol.net.cn/gtqtfdlmtu.html

[I02] 提取所有匹配
来源：http://hz.dianchejie.cn/gtpcbjqtuk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guannengcc.top/gttbncoxge.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuetiantiany.cn/gtgxwlywoz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ehwqpu.com/gttrpgbjxy.html

TS:   s.match(/\d+/g)
来源：http://hz.yonumen.top/gtpvvhakle.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ywan-chungtsiang.top/gtoszixppq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daria6918.cn/gtpighcfvu.html

Ruby: s.scan(/\d+/)
来源：http://hz.52xcode.cn/gtituftnsv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hongshengwenyu.top/gtknsreiox.html

[I03] 提取捕获分组
来源：http://hz.hammf.cn/gtdbwidvlh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhengqikj.top/gthgdznwgk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hywenlv.cn/gtkypmbvvx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.aibaodan.cn/gtrxyjmvba.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhengqikj.top/gtobtvbpji.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhengqikj.top/gtabfvwrtm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xylfe.cn/gteoukvgjp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangtech.top/gtduiwkvhx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gotoacloud.top/gtdukngpoi.html

[I04] 正则替换
来源：http://hz.haohaochexian.top/gtvobmkkjh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.snrcjt.cn/gtvmbyzcgx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.havefunace.top/gtfzxvclzf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtfstnclif.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtymtnvwxp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.feifeiyinyue.top/gtbaevytcu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258888.top/gthmfwskhs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.redwolf501.top/gtgioeigpg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daria6918.cn/gtyylpffsv.html

[I05] 按正则拆分
来源：http://hz.xylfe.cn/gtdhiauvll.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pycfn.com/gtarhwwqil.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dashuyun.cn/gtpkzemzkh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtdsvydqan.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtyothzvps.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ywan-chungtsiang.top/gtxccsstvt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xinyue.icu/gtqogqdhew.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtcgkqzcbb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yueranfly.top/gtxlhoiqyn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.kuanghao11.cn/gtzustnzhm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtyjflwhhl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhiwuduotai.top/gtahvlaghg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtrewsejeq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenlongwang.top/gtakqoktkb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nwbrower.top/gtyggdxstg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yanxiufei.cn/gtjojxkxfa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shuidangran.top/gtblgmhirs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gthsohpkdr.html

[I07] 忽略大小写与多行模式
来源：http://hz.tian-w.cn/gtidtvttzn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtaxeaeryi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cucudq.cn/gtcigkmoxx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jiagoushi.top/gtukwzpyir.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtrthljfga.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shzxlz.cn/gtxjsibjdm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jianghu66.top/gtbkygmhpq.html

Ruby: s.scan(/error/i)
来源：http://hz.daria6918.cn/gtxudwuaio.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tianlin.xyz/gtijzuebdm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jianghu66.top/gtlyomjrpk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtsefwrhgk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guowangkeji.top/gtzuyavldz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtjmzvenla.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258888.top/gtldjzaqnl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hongshengwenyu.top/gtgnjyfdea.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhiwuduotai.top/gtuvutnjoj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.haohaochexian.top/gtaxzgzzsu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.mhx1999.top/gtkqoyapuo.html

================================================================================
来源：http://hz.shzxlz.cn/gtlarsceyr.html

J. 日期与时间
来源：http://hz.yj202588.top/gtcnxsdueq.html

================================================================================
来源：http://hz.yj20258888.top/gtnyejoneo.html

[J01] 获取当前时间
来源：http://hz.tianlin.xyz/gtcwsiuezd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yueranfly.top/gtcyszywfd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gzhubu.top/gtolwbsnhn.html

JS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtkhkhxurl.html

TS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtzjbfyojm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhijiandao.cn/gtlufertat.html

Go:   time.Now()
来源：http://hz.hysaishi.cn/gttwpanage.html

Ruby: Time.now
来源：http://hz.shzxlz.cn/gtsgsqpcra.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shangyingyoupin.top/gtwjibhfty.html

[J02] 格式化输出
来源：http://hz.yvedp.cn/gtpyxyumbx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtetcbtote.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtwjvtgkec.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenlongwang.top/gtrspaiivx.html

TS:   d.toISOString()
来源：http://hz.smart0.xyz/gtcwxnflgp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dashuyun.cn/gtxiwgdksw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nwbrower.top/gtogvfsasx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gteedhnqkr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ehwqpu.com/gtptlonujx.html

[J03] 字符串解析为日期
来源：http://hz.cucudq.cn/gtltukvrkf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.52xcode.cn/gtaokmbjph.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhaomingkeji.xyz/gtqsglevfd.html

JS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtxskfkbgj.html

TS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtlrtahkqu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtvnhulevy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenjidiqi.icu/gtcmjfezec.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtjorxlzxg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tianlin.xyz/gtrgustjkl.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtastiaobu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.c1oappe.top/gtofgizrat.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jyoumei.cn/gttmrheqnz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenjidiqi.icu/gtienhwtmh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.meibo888.top/gtdsqkmgbi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxinkj.top/gtynfhtybe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258888.top/gtkobmtkxu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydzc1.top/gtfxuxqtyk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dianchejie.cn/gttiykovez.html

[J05] 时间加减（加 7 天）
来源：http://hz.mhx1999.top/gtglytspxi.html

Py:   now + timedelta(days=7)
来源：http://hz.shangyingyoupin.top/gtcfctdpis.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yangfankeji.com/gtqbdlmezf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gthrqzoonc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtbnplpnrt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sufxvd.cn/gtqauroyir.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hysaishi.cn/gtfuiijfbz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuetiantiany.cn/gtqgoryoil.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ywan-chungtsiang.top/gtutquhudi.html

[J06] 计算两时间之差
来源：http://hz.wangshuangyany.cn/gtcflueolu.html

Py:   (end - start).total_seconds()
来源：http://hz.pycfn.com/gtfqskipsq.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gtbpamthdi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.snrcjt.cn/gtnmhwttlu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.mhx1999.top/gtneceqvjl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.bjfxy.top/gtmawcifaz.html

Go:   end.Sub(start).Hours()
来源：http://hz.xinyue.icu/gtxhaktvgb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gzhubu.top/gtwlrbauee.html

C#:   (end - start).TotalSeconds
来源：http://hz.yonumen.top/gtqwvhvfmh.html

[J07] 比较两个日期
来源：http://hz.nwbrower.top/gtlqmyiyik.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtcattrsjj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daria6918.cn/gtinrpwbqu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtdrvbhifw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ydzc1.top/gtczpgxyvw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtnfumtops.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gtqyhquwws.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtrodysrqo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtfuwwaodw.html

[J08] 提取年月日与星期
来源：http://hz.zhoulong.xyz/gtdyggupfw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hammf.cn/gtipcmuhnk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gtukgtdzza.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cqqwz.cn/gtvhiaqigo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tian-w.cn/gtdpvnagur.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinyuanbaomall.cn/gtokvkjthm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pycfn.com/gtcmuhdsng.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pycfn.com/gtjoowtenm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.haohaochexian.top/gtqhjenfqx.html

[J09] 时区处理
来源：http://hz.xingfuxueyuan.xyz/gtscbeuriz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fengsongda.top/gtzzlmgdfq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cashguo.top/gtnolqcxwo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtbdwvwmsv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gthfofelmk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinyuanbaomall.cn/gthkzbmhgd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yanxiufei.cn/gtckgvduog.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuanzhike.top/gtiyrdsaba.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yueranfly.top/gtvdxzwykb.html

[J10] 取今天 / 本月第一天
来源：http://hz.redwolf501.top/gteynbwwtq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aibaodan.cn/gtoselcqvp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ivvv.top/gtvtcrsfrg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.fzhhl.top/gtpxuopkmi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.daria6918.cn/gtvtrtxbxu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenzaomai.com/gtrmfqatoq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigufen.top/gtjfkmitas.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zycfv.cn/gthrxkkdxh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuanzx.com/gtswagqllu.html

================================================================================
来源：http://hz.snrcjt.cn/gtgcaxtukr.html

K. JSON 与序列化
来源：http://hz.birdmap.top/gtpmcklhri.html

================================================================================
来源：http://hz.haohaochexian.top/gtcwduabyr.html

[K01] 对象转 JSON 字符串
来源：http://hz.yongpay.top/gtyctnkgod.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtwqturimk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ywan-chungtsiang.top/gtwnpgoesr.html

JS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtbeivvamu.html

TS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtgkvrnnts.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gzhubu.top/gtqwgqkvhe.html

Go:   json.Marshal(obj)
来源：http://hz.fengsongda.top/gtdasfqfpi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jyoumei.cn/gtexstmtiz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xylfe.cn/gtafwqtebw.html

[K02] JSON 字符串转对象
来源：http://hz.jinyuanbaomall.cn/gtsulkuebe.html

Py:   json.loads(s)
来源：http://hz.zycfv.cn/gtjbaaddoh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zdqjudy.top/gtgidnaisg.html

JS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtzcjotelg.html


<!-- 参考信息 -->