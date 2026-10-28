代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yangfankeji.com/gtfovgpsof.html

Ruby: def to_s; @name; end
来源：http://hz.jinyuanbaomall.cn/gtmjycrqwj.html

C#:   public override string ToString() => Name;
来源：http://hz.sufxvd.cn/gtsvdbwvqe.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtvhdxoffn.html

Py:   isinstance(u, User)
来源：http://hz.yvedp.cn/gtbilxyndy.html

PHP:  $u instanceof User
来源：http://hz.bjfxy.top/gtdpcollog.html

JS:   u instanceof User
来源：http://hz.ybcxt.top/gttihxsvon.html

TS:   u instanceof User
来源：http://hz.zhengqikj.top/gtsirzgvvh.html

Java: u instanceof User
来源：http://hz.hnqzz.top/gtgjecwigy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jyoumei.cn/gtxxbhwgzi.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gtyhnxiiym.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gtqktwaaze.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangtech.top/gtzajpdjzo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gtyoddmatd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aibaodan.cn/gtpwzixgpr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtfiueifby.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigufen.top/gttyyuscnf.html

Java: record User(String name, int age) {}
来源：http://hz.yanxiufei.cn/gtfvlzgvfw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxinkj.top/gtaucgaezk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtcpgqnqfp.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtdvjmcnww.html

[G15] 枚举
来源：http://hz.mhx1999.top/gtzvzgnwcj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sysykeji.top/gtbzeyosec.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nwbrower.top/gtquzxfnjt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj202588.top/gtsnrwryxw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtltijfziy.html

Java: enum Color { RED, GREEN }
来源：http://hz.pengpengdd.cyou/gtwnzmcgru.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tian-w.cn/gtschweiza.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ivvv.top/gtfeceqiwl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gtrldxuepu.html

[G16] 对象转数组 / 字典
来源：http://hz.havefunace.top/gtotmidodg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.316326.xyz/gtfzhawxhi.html

PHP:  get_object_vars($obj);
来源：http://hz.guowangkeji.top/gtnxrkrgmj.html

JS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtxtrjngfc.html

TS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtehjhoepf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.smart0.xyz/gtjoyhkppu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhengqikj.top/gtsmdgrjbh.html

Ruby: obj.instance_variables
来源：http://hz.cheryme.top/gtywvydagj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cdnleiting.top/gtzmhzpnjo.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtsvrlrnhh.html

H. 异常与错误处理
来源：http://hz.fengsongda.top/gtbsghdupf.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtubgogutj.html

[H01] try / catch 基础
来源：http://hz.sweek.top/gtfjndsqnf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuetiantiany.cn/gtlppacuod.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yueranfly.top/gtsaycddew.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.316326.xyz/gtkqoqhkvi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtxdfhiobj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgufenzy.top/gtqgfaofns.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yanxiufei.cn/gtlnfbkedo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ppjwa.cn/gtwoqjuqym.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenlongwang.top/gtciopwcrp.html

[H02] finally / ensure 收尾
来源：http://hz.hnxiangtu.top/gtspgxafsf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.c1oappe.top/gttewawvzd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtdyklsrgl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtanknxeor.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtvqptfjkr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtjroohmyp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigufen.top/gtdprzulln.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gotoacloud.top/gtmzwucwtg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gthusovdhx.html

[H03] 主动抛出异常
来源：http://hz.hywenlv.cn/gtbppxoapn.html

Py:   raise ValueError("错误信息")
来源：http://hz.kuanghao11.cn/gtxlwqfftv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtxpivhrtj.html

JS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gtjztihddq.html

TS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtquqdcjjy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtoamooooa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.andypj.xyz/gtfjomawxl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aibaodan.cn/gtpwooixbw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtbdzorbxy.html

[H04] 自定义异常类型
来源：http://hz.svipenyu.cn/gtvxfdmfjb.html

Py:   class MyError(Exception): pass
来源：http://hz.sweek.top/gtxjcrwvzq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258.top/gtrgpiurbq.html

JS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtfmgkttfw.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtglahevrp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dashuyun.cn/gtqemexfic.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgfzy.top/gtbmulmgrf.html

Ruby: class MyError < StandardError; end
来源：http://hz.feifeiyinyue.top/gtuqdhebbl.html

C#:   class MyException : Exception {}
来源：http://hz.feifeiyinyue.top/gtornvywsl.html

[H05] 捕获特定类型
来源：http://hz.wangshuangyany.cn/gtnjjiryvo.html

Py:   except ValueError as e:
来源：http://hz.snrcjt.cn/gtdoppivgf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.svipenyu.cn/gtcdphkbia.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtbckoycvt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.wangdashe.top/gtaefuzvpg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.pycfn.com/gtqydyuqvg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhixingplan.top/gtluxqnrgq.html

Ruby: rescue ArgumentError => e
来源：http://hz.ehwqpu.com/gtobjfptfj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.52xcode.cn/gtzxocjlwi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.haohaochexian.top/gtwxqkyhex.html

Py:   value = d.get("k") or default
来源：http://hz.cheryme.top/gtgfzvybme.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xinyue.icu/gtcirbjgzm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gthiunsnkg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtfryqbqae.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.0kj1m.cn/gtxxsvgnby.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xingfuxueyuan.xyz/gtcapnvjvd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenzaomai.com/gthtqbzypc.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtkjrbfhle.html

[H07] 断言
来源：http://hz.fzhhl.top/gtlxutmcnx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yanxiufei.cn/gtlpyigxif.html

PHP:  assert($x > 0);
来源：http://hz.yueranfly.top/gtdfeydyux.html

JS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gtwfixpbvt.html

TS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtgetczycv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shuidangran.top/gtziihpmie.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yuxming.cn/gternhhwyu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xinyue.icu/gthtejskiw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gtgfyphtip.html

[H08] 获取错误信息与堆栈
来源：http://hz.ehwqpu.com/gtbypwjlyg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hfpthk.cn/gtufyaublw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tian-w.cn/gtjghhcapv.html

JS:   e.message;  e.stack
来源：http://hz.yanxiufei.cn/gtirctohyu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.iojbl.cn/gtyehtfloq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhixingplan.top/gtbeybaqjj.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtcrzcsfzr.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigufen.top/gtasgyqrnk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gogol.net.cn/gtlrvxtftt.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtkjmvkbhu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gogol.net.cn/gtehfcgglz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtcjscoyhz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wangshuangyany.cn/gtqsgsanjn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangshuangyany.cn/gtpebabnbw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydjk.org.cn/gttaoqeeto.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yanxiufei.cn/gtscoqvcwm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ywan-chungtsiang.top/gtwldwouif.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.fengsongda.top/gtugbuwlpy.html

[H10] 资源自动释放
来源：http://hz.zhongyouzk.top/gttzactztl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gaohongyu789.top/gtpjtdriqb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.9152youxi.cn/gtgbnblocf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gtkjgxuhcz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gthoqvqbhq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhijiandao.cn/gtieeipuag.html

Go:   defer f.Close()
来源：http://hz.gaohongyu789.top/gtorgfsubm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gotoacloud.top/gtnrdkolai.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhengqikj.top/gtychqbzrd.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtvgarhyqq.html

I. 正则表达式
来源：http://hz.haohaochexian.top/gtqeasxbku.html

================================================================================
来源：http://hz.fengsongda.top/gtveamzzbf.html

[I01] 判断是否匹配
来源：http://hz.52xcode.cn/gtcwvaxyiy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhixingplan.top/gtmggtkzem.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ywan-chungtsiang.top/gtyvkorcsk.html

JS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtkivblyax.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gthasllcbr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pycfn.com/gtnzeujhve.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnxiangtu.top/gtqeyqunif.html

Ruby: s.match?(/\d+/)
来源：http://hz.yanxiufei.cn/gthgbhzdid.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigfzy.top/gtxytfjnbm.html

[I02] 提取所有匹配
来源：http://hz.redwolf501.top/gttxnrptjp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hammf.cn/gtaoiqjryf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hongshengwenyu.top/gtmozrdkqk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigufen.top/gticdqvuas.html

TS:   s.match(/\d+/g)
来源：http://hz.yongpay.top/gtrpsqtrwb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yanxiufei.cn/gtfzvozfxs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtchlzohyy.html

Ruby: s.scan(/\d+/)
来源：http://hz.c1oappe.top/gthmdnnsgk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yangfankeji.com/gtzufvwjdn.html

[I03] 提取捕获分组
来源：http://hz.yuanzhike.top/gtwhfckdix.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dianchejie.cn/gtewssmlwr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtfdfqbecw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenlongwang.top/gtvldqsbpu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydjk.org.cn/gtivcpsqqp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.birdmap.top/gtlrwlvmup.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yanxiufei.cn/gtxzacosqz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigufen.top/gtasrhtzyi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxuanxn.top/gtailvuyja.html

[I04] 正则替换
来源：http://hz.cdnleiting.top/gtrdnrllvb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangshuangyany.cn/gtblnnpomf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shzxlz.cn/gtaosabbwb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtyxetfcqr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtexsopapl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yonumen.top/gtbjqxwpkf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnqzz.top/gtxocclzbw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sxryk.cn/gtbmwhyjzv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigufen.top/gtewrtbfny.html

[I05] 按正则拆分
来源：http://hz.chenjidiqi.icu/gtjtaquypf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgfzy.top/gtkmgpefxj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zdqjudy.top/gtroycjcmy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtiaclvgwn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtfbivltwz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sxryk.cn/gtakmaftbg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shuidangran.top/gtjjzgjhoe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtcvjqfzyr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sxryk.cn/gtzmupztrs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hywenlv.cn/gtlmrjqllq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gtfbgikgxj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gtjlrhfifs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtdvntetxc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtyxqrqmoc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ppjwa.cn/gtajiscarm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jyoumei.cn/gtkubuwbpo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gtviamkjgl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gtxsdmnuio.html

[I07] 忽略大小写与多行模式
来源：http://hz.jqgfzy.top/gtuxvhwmkf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ehwqpu.com/gtbddsqauy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinghuilouyu.cn/gtbwccoqan.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuetiantiany.cn/gtejgjautx.html

TS:   /error/gim
来源：http://hz.redwolf501.top/gtqrwvxwzv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yongpay.top/gtjcshqdfv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yongpay.top/gtflrpfspp.html

Ruby: s.scan(/error/i)
来源：http://hz.iojbl.cn/gtrtsyqxzr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tanke756.top/gtnkjfjnil.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cqqwz.cn/gtdxmtcexr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gtasxgsgon.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shuidangran.top/gtkftxqxql.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtlkkjatwv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtpsamncfe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtgzjqpmlf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gzhubu.top/gtfwxljlwr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gogol.net.cn/gtcuddonjo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtpnjiegtt.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtnqevyavd.html

J. 日期与时间
来源：http://hz.gaohongyu789.top/gtjtfzptmg.html

================================================================================
来源：http://hz.jianghu66.top/gtpajxardt.html

[J01] 获取当前时间
来源：http://hz.ehwqpu.com/gtuccgezur.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hongshengwenyu.top/gtxoowfayw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtddcauywh.html

JS:   new Date();  Date.now()
来源：http://hz.zhoulong.xyz/gtqoqipwfv.html

TS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtsilnxuox.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgfzy.top/gtnbtqcmgy.html

Go:   time.Now()
来源：http://hz.sweek.top/gtcewknjmv.html

Ruby: Time.now
来源：http://hz.jinyuanbaomall.cn/gtpylnbksr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yvedp.cn/gtfnvtncio.html

[J02] 格式化输出
来源：http://hz.yueranfly.top/gtjzldqhlv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.0kj1m.cn/gtgemazgno.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tianlin.xyz/gtttpaerwl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhongyouzk.top/gtvavfstnq.html

TS:   d.toISOString()
来源：http://hz.ydzc1.top/gtgohnzzoa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigfzy.top/gtikpioain.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.bjfxy.top/gtxqawbcyl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gthcudbksk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.guowangkeji.top/gtqdzytgfr.html

[J03] 字符串解析为日期
来源：http://hz.tanke756.top/gtmlcjjppj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuxming.cn/gteobxqjvb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jyoumei.cn/gtmxigyolc.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtcfsdoxeu.html

TS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtyzkoszaz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtxkximxaw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hnxiangtu.top/gtwpnxdvzs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gthvhrxgof.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hywenlv.cn/gtrebmlqra.html

[J04] 时间戳与日期互转
来源：http://hz.yueranfly.top/gtstjhdexz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuanzhike.top/gtxomwepud.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ybcxt.top/gtgcjyimia.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ivvv.top/gttemyqvsn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yangfankeji.com/gtopscpdcf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigfzy.top/gtzlkjlssd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.havefunace.top/gtgkxzuxwb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cdnleiting.top/gtzidkugpk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.vqdsnc.cn/gtcnvymzbf.html

[J05] 时间加减（加 7 天）
来源：http://hz.dashuyun.cn/gtjyqnavnt.html

Py:   now + timedelta(days=7)
来源：http://hz.xuanzx.com/gtqxivotnm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtcohwybcr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtfqeqmuka.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gttdbcmuyh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.316326.xyz/gtgzborpix.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtixulffkf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guowangkeji.top/gtlhitamdn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxinkj.top/gtgyfvhqcw.html

[J06] 计算两时间之差
来源：http://hz.shuidangran.top/gtvxbzqfty.html

Py:   (end - start).total_seconds()
来源：http://hz.snrcjt.cn/gtefiyeyxd.html

PHP:  $end->diff($start)->days;
来源：http://hz.shangyingyoupin.top/gtruzmbxiq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.birdmap.top/gtrskafpen.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cashguo.top/gtwszpwvce.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinyuanbaomall.cn/gtvpcbmpzo.html

Go:   end.Sub(start).Hours()
来源：http://hz.sysykeji.top/gtrygifcqm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jiagoushi.top/gtcbusjgnd.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtzanglobn.html

[J07] 比较两个日期
来源：http://hz.jqgfzy.top/gtxoprzqsz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtljbskdzg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dianchejie.cn/gturrwsvzd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtgsfimnfx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hysaishi.cn/gtwptuuovh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dashuyun.cn/gtijistgyv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.svipenyu.cn/gtpigyaamp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtjsjbjeaq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtlwdvonvu.html

[J08] 提取年月日与星期
来源：http://hz.daria6918.cn/gtaoiqiwaw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.smart0.xyz/gtwzsvmrcq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.9152youxi.cn/gtkyhxscpe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xinyue.icu/gtdjympkfv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cheryme.top/gtfkwzhmwt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.smart0.xyz/gtalwfojcl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tianlin.xyz/gtwoxakshy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ivvv.top/gtnsifqqft.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhiwuduotai.top/gtobkantjd.html

[J09] 时区处理
来源：http://hz.zhiwuduotai.top/gtzocwdycv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dashuyun.cn/gtoowtctrg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zdqjudy.top/gtoqrvjyab.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuanzx.com/gtrsqclgfv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtcmixeyyo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.redwolf501.top/gtcqzprlom.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gttcgnjhym.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gtqkebdrvy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hysaishi.cn/gtotoahrgp.html

[J10] 取今天 / 本月第一天
来源：http://hz.svipenyu.cn/gtvbcwvwaz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinyuanbaomall.cn/gtrtkbvdin.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinghuilouyu.cn/gtxbngpdnx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigufen.top/gtylsnkmhg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.andypj.xyz/gtatynhuos.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.andypj.xyz/gttxrgzlwf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tian-w.cn/gtamzlwnzm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangkeji.top/gtlbsnhjki.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgufenzy.top/gtoistwdan.html


<!-- 参考信息 -->