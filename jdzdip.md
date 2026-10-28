代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.smart0.xyz/gtzhquecrv.html

Ruby: def self.f; end
来源：http://hz.smart0.xyz/gtbirhowrj.html

C#:   public static void F() {}
来源：http://hz.jinyuanbaomall.cn/gtxwvgubae.html

[G09] 接口 / 抽象类
来源：http://hz.snrcjt.cn/gtjxqcewlh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj202588.top/gtbvqsklxd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ivvv.top/gtjvxvqnnh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.wangdashe.top/gtyuyatphw.html

TS:   interface Shape { area(): number; }
来源：http://hz.xylfe.cn/gtvedrzbbw.html

Java: interface Shape { double area(); }
来源：http://hz.jlsjyb.cn/gtnbmyimud.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aibaodan.cn/gttyvscjvv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guannengcc.top/gtatcuvmyz.html

C#:   interface IShape { double Area(); }
来源：http://hz.guowangkeji.top/gtjrqhijvg.html

[G10] 访问控制
来源：http://hz.cucudq.cn/gtjsrdycuu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gaohongyu789.top/gtesnfwpdq.html

PHP:  public / protected / private
来源：http://hz.vqdsnc.cn/gtgvpzrtxa.html

JS:   #private 字段；其余公开
来源：http://hz.chenzaomai.com/gtigyrsftn.html

TS:   public / protected / private
来源：http://hz.cashguo.top/gtdxzubmjq.html

Java: public / protected / private / 默认包级
来源：http://hz.fzhhl.top/gtzobsspyn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jlsjyb.cn/gtlysfuogh.html

Ruby: public / protected / private
来源：http://hz.zhongyouzk.top/gtkmhdkntz.html

C#:   public / protected / private / internal
来源：http://hz.xziqi.cn/gtlzjinlsf.html

[G11] getter / setter
来源：http://hz.shuidangran.top/gtubkqodno.html

Py:   @property 与 @x.setter
来源：http://hz.xingfuxueyuan.xyz/gtjqmlpois.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtrnoexbml.html

JS:   get name() { return this._name; }
来源：http://hz.jianghu66.top/gtglmdryty.html

TS:   get name(): string { return this._name; }
来源：http://hz.gogol.net.cn/gtbhtazcpt.html

Java: public String getName() { return name; }
来源：http://hz.dashuyun.cn/gtkisjzlei.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.0kj1m.cn/gtzawwcbfy.html

Ruby: attr_accessor :name
来源：http://hz.yj20258.top/gtrrdasaey.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtrmkdjroo.html

[G12] 对象转字符串
来源：http://hz.hnqzz.top/gtqpwaakhb.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxuanxn.top/gthpkflcju.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.havefunace.top/gtlpqgusoj.html

JS:   toString() { return this.name; }
来源：http://hz.andypj.xyz/gtmarlwlij.html

TS:   toString(): string { return this.name; }
来源：http://hz.jianghu66.top/gtxzkxczna.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gtqcdhtruu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dianchejie.cn/gtzhjwqlzf.html

Ruby: def to_s; @name; end
来源：http://hz.jinghuilouyu.cn/gtwzorlmmq.html

C#:   public override string ToString() => Name;
来源：http://hz.ywan-chungtsiang.top/gtgikgtwmz.html

[G13] 判断对象类型
来源：http://hz.xinyue.icu/gtcnjtjktm.html

Py:   isinstance(u, User)
来源：http://hz.52xcode.cn/gtwfvepadc.html

PHP:  $u instanceof User
来源：http://hz.yueranfly.top/gtzzuidywn.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtaqjjfscv.html

TS:   u instanceof User
来源：http://hz.jiagoushi.top/gtrjhboxld.html

Java: u instanceof User
来源：http://hz.jyoumei.cn/gtdxwbjhkb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sysykeji.top/gtxveghsmx.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gtxusdscwc.html

C#:   u is User
来源：http://hz.gzhubu.top/gtyhwrlqpb.html

[G14] 数据类 / record
来源：http://hz.wangdashe.top/gtbxesrtle.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gotoacloud.top/gtoesupudu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.daxiang520.top/gtznncltiq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shzxlz.cn/gtepklbzsx.html

TS:   type User = { name: string; age: number };
来源：http://hz.ywan-chungtsiang.top/gtzsgemevt.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtswdhycja.html

Go:   type User struct { Name string; Age int }
来源：http://hz.0kj1m.cn/gtaycoztel.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.snrcjt.cn/gtefmpsuvn.html

C#:   record User(string Name, int Age);
来源：http://hz.chenzaomai.com/gtzaadotww.html

[G15] 枚举
来源：http://hz.hysaishi.cn/gthqocianv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cdnleiting.top/gtdebxfzih.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yangfankeji.com/gtravcmlaa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.redwolf501.top/gtjwsxpjtf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtqmljlrdz.html

Java: enum Color { RED, GREEN }
来源：http://hz.havefunace.top/gttwshtefn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yonumen.top/gtssjnkgfj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenzaomai.com/gtdpdvpggh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtxsszlqta.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gtudmqglgi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydjk.org.cn/gtpxhlxnqz.html

PHP:  get_object_vars($obj);
来源：http://hz.yvedp.cn/gtvbpfbvek.html

JS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gtupyjbsvj.html

TS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtmgsgkryq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.svipenyu.cn/gtppjfmzjc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guannengcc.top/gtespfaeoo.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gtznqcoyuy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.svipenyu.cn/gtohhwspje.html

================================================================================
来源：http://hz.quarkkingdee.top/gthibvoxvj.html

H. 异常与错误处理
来源：http://hz.gotoacloud.top/gtchyeysdy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gthduoccbk.html

[H01] try / catch 基础
来源：http://hz.wangdashe.top/gtftlmrvpx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.0kj1m.cn/gtozgpydmv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aizwys.cn/gtbjqazfmb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cheryme.top/gtduhpbrgj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daria6918.cn/gthtcxvppy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hammf.cn/gteuxfhdro.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgufenzy.top/gtftkfvugw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gthqbbuozl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xingfuxueyuan.xyz/gtawaydwrt.html

[H02] finally / ensure 收尾
来源：http://hz.jiagoushi.top/gtskxeaqro.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aibaodan.cn/gttzijrjat.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtfzjkncqc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtemrikngh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtkthsnwxu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtwtrbsdsz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.guannengcc.top/gtxcjnebxz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.redwolf501.top/gtyzyfmumt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guannengcc.top/gtjngixusa.html

[H03] 主动抛出异常
来源：http://hz.xuanzx.com/gtzpqgyteb.html

Py:   raise ValueError("错误信息")
来源：http://hz.hywenlv.cn/gtnibpvrpp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtyliqpwmx.html

JS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtbixpxxwy.html

TS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtyepfzlmp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gteoilovqx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtrtakpstz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.iojbl.cn/gtzslvksfn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtaxisfzss.html

[H04] 自定义异常类型
来源：http://hz.9152youxi.cn/gtjukwpnck.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gtimsccrea.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shuidangran.top/gtljlnrrzm.html

JS:   class MyError extends Error {}
来源：http://hz.kuanghao11.cn/gtzyjvtfas.html

TS:   class MyError extends Error {}
来源：http://hz.shzxlz.cn/gtjncsljgm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj202588.top/gtdcvfyyvh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhengqikj.top/gtycmkfqyt.html

Ruby: class MyError < StandardError; end
来源：http://hz.gogol.net.cn/gtsqxvjkva.html

C#:   class MyException : Exception {}
来源：http://hz.iojbl.cn/gtaztdsuhw.html

[H05] 捕获特定类型
来源：http://hz.yanxiufei.cn/gtdulqjstv.html

Py:   except ValueError as e:
来源：http://hz.jqgfzy.top/gtxdgdtdsf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhixingplan.top/gtxklzudtz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtdxnmmsov.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtpdgnbryl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.mhx1999.top/gtlwjfcipb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dashuyun.cn/gtixrhimzj.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhoulong.xyz/gtmzyssxrw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hysaishi.cn/gtkgnpygqy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pengpengdd.cyou/gtopjhuiae.html

Py:   value = d.get("k") or default
来源：http://hz.hfpthk.cn/gtalrrxqee.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cdnleiting.top/gtqpywcynm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtercfiaub.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtzdmifhwq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinghuilouyu.cn/gtynqtgbwi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.mhx1999.top/gteyilwkye.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangkeji.top/gtbhduvseb.html

C#:   obj?.A?.B ?? default
来源：http://hz.smart0.xyz/gtznonrldi.html

[H07] 断言
来源：http://hz.hnqzz.top/gtiatpmdbr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gotoacloud.top/gtpspzsbtm.html

PHP:  assert($x > 0);
来源：http://hz.hfpthk.cn/gtxxmsghuf.html

JS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtdflydjjn.html

TS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtfiaebbiy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinyuanbaomall.cn/gtzkukwgiv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zycfv.cn/gtlqsiuyuk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.redwolf501.top/gtpqyrjyxy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gtprsbfgys.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenzaomai.com/gtwkuhgrlj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gtwbaztyxh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nwbrower.top/gtzkbbjcco.html

JS:   e.message;  e.stack
来源：http://hz.daxiang520.top/gteyfmeiga.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.quarkkingdee.top/gtjhkimizo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xinyue.icu/gtifnexizs.html

Go:   err.Error()
来源：http://hz.zdqjudy.top/gtjqwzybuf.html

Ruby: e.message;  e.backtrace
来源：http://hz.hysaishi.cn/gtdmjtzjvm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ivvv.top/gtwigwtxur.html

[H09] 带错误码的异常
来源：http://hz.meibo888.top/gthkigffhm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shuidangran.top/gtynfawscc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.snrcjt.cn/gtavjzltpm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jianghu66.top/gtkylxlqhv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sxryk.cn/gtxbunavnl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ybcxt.top/gtebjpeevu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yongpay.top/gtkzpaiycs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangkeji.top/gtkayxgjor.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nwbrower.top/gtjqrndckx.html

[H10] 资源自动释放
来源：http://hz.yongpay.top/gtajcglxvb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.pengpengdd.cyou/gtgsegvmmg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.9152youxi.cn/gtpatxakon.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtcnbijldl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gtfrjdwlyl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhengqikj.top/gtzqnvgrvj.html

Go:   defer f.Close()
来源：http://hz.ydzc1.top/gtfyphuwza.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtmvzfbugl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daxiang520.top/gtiipxkspl.html

================================================================================
来源：http://hz.jinqigufen.top/gtwvhguwot.html

I. 正则表达式
来源：http://hz.nanxinkj.top/gtilyjhvlp.html

================================================================================
来源：http://hz.tianlin.xyz/gtbthrsowl.html

[I01] 判断是否匹配
来源：http://hz.sysykeji.top/gtawrvjyfy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zdqjudy.top/gtpadoweup.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zycfv.cn/gtlfzsxzxt.html

JS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtcgayidtl.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtpizpinil.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenlongwang.top/gtohfyxkkg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cucudq.cn/gtdholrqsb.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenzaomai.com/gtvjpibsxq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258.top/gtjozenope.html

[I02] 提取所有匹配
来源：http://hz.wangdashe.top/gtzwkstpbj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhengqikj.top/gtjrvloueg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fengsongda.top/gtvssswuua.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj202588.top/gtidufzjke.html

TS:   s.match(/\d+/g)
来源：http://hz.ehwqpu.com/gtzgzzhpgb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydzc1.top/gtfufvsikv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gttiaixesg.html

Ruby: s.scan(/\d+/)
来源：http://hz.zdqjudy.top/gthfynmkyr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.c1oappe.top/gtuskgrjet.html

[I03] 提取捕获分组
来源：http://hz.nanxinkj.top/gtqkqoinca.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhoulong.xyz/gtfacrqmrn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daxiang520.top/gtvqwdzuaq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxinkj.top/gtbvkbzomv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigufen.top/gtcprohuen.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinqigfzy.top/gtgdccprmc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinyuanbaomall.cn/gtqyyewxcv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtkaajnvqu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gotoacloud.top/gtxkfqgxmi.html

[I04] 正则替换
来源：http://hz.aizwys.cn/gtjkdtcufr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sysykeji.top/gtkjqtjjyo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gtwyrwwnlk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtebxnkoir.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.wangdashe.top/gtodlybusr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ydjk.org.cn/gtowwvprno.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydzc1.top/gtihinypmh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.0kj1m.cn/gtiyyuvsdo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuanzhike.top/gtmqqjfoxw.html

[I05] 按正则拆分
来源：http://hz.jiagoushi.top/gtpftnxxah.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ivvv.top/gtxkrairsj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxinkj.top/gtmctmxkcs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gteuswugqc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtskqedxsg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hysaishi.cn/gtlvbaeubg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhiwuduotai.top/gtzbrplsza.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gthrkewwxn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.kuanghao11.cn/gtlcobevcg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgufenzy.top/gtnnnlgjye.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtrihlcbko.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuxming.cn/gtniryreoy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gtxpjkbaja.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.52xcode.cn/gtvlthvgwz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.kuanghao11.cn/gtigcvxhcp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.feifeiyinyue.top/gtcrklpsuy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.andypj.xyz/gtqbfaorwe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtefrlxiux.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258888.top/gtnhqvcrya.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cashguo.top/gtowqbszwk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258888.top/gthudupkjl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shuidangran.top/gtrnkpregk.html

TS:   /error/gim
来源：http://hz.xinyue.icu/gtwnyeisec.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnxiangtu.top/gtpblngdjd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zycfv.cn/gtqlqljmaz.html

Ruby: s.scan(/error/i)
来源：http://hz.aizwys.cn/gtqmgazzpb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yangfankeji.com/gtdlggznzx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shzxlz.cn/gtypegbtuo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuanzx.com/gtwuxaxunf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenzaomai.com/gtqetndyky.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtwnmmqjrm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtvdxntmnv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.mhx1999.top/gtueoeqbbb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.meibo888.top/gtkwwnyepb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.pengpengdd.cyou/gthjhyxakt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtjiwyowfo.html

================================================================================
来源：http://hz.fzhhl.top/gtefvhhxss.html

J. 日期与时间
来源：http://hz.jqgufenzy.top/gtkrubstpk.html

================================================================================
来源：http://hz.gogol.net.cn/gtjrikoyao.html

[J01] 获取当前时间
来源：http://hz.zhoulong.xyz/gtnoiydswk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gttxxgjcis.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtkyqikjzu.html

JS:   new Date();  Date.now()
来源：http://hz.jqgfzy.top/gtwyudaijy.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtthnuiguo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258.top/gteiwqjzsp.html

Go:   time.Now()
来源：http://hz.xylfe.cn/gtkjdwebdz.html

Ruby: Time.now
来源：http://hz.quarkkingdee.top/gtnmeizyms.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgfzy.top/gtmncprwjs.html

[J02] 格式化输出
来源：http://hz.hfpthk.cn/gthionwbve.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtahcxspeq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dianchejie.cn/gtzmcxghxg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hammf.cn/gtqgduktyb.html

TS:   d.toISOString()
来源：http://hz.guowangkeji.top/gtejsxxskb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhaomingkeji.xyz/gttfdtvvnf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gaohongyu789.top/gterecikle.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yueranfly.top/gtxikkeabv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinghuilouyu.cn/gthdfmbfsk.html

[J03] 字符串解析为日期
来源：http://hz.snrcjt.cn/gtxguaquaq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.smart0.xyz/gtyvfyredc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.vqdsnc.cn/gtwmztaoou.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtknysptxg.html

TS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gtrvoiylvu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuxming.cn/gtmubwuscq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guannengcc.top/gtzapnjwwf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gthdsoalwh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guowangkeji.top/gtcywgqszs.html

[J04] 时间戳与日期互转
来源：http://hz.ppjwa.cn/gtylyqqdyg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.wangshuangyany.cn/gtkavlocil.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tianlin.xyz/gtppxlgkhu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gtaerqcxse.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangshuangyany.cn/gthrtrpzgg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gtfiaomfwr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aizwys.cn/gthxgzfruf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258888.top/gtsrtyqxsd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ivvv.top/gtzfuxfgra.html

[J05] 时间加减（加 7 天）
来源：http://hz.nwbrower.top/gtrhpbveph.html

Py:   now + timedelta(days=7)
来源：http://hz.haohaochexian.top/gtrlfwxvvy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cdnleiting.top/gtucifzhjc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtikxkncwb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtgclobqwr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gthilgjmdz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yuxming.cn/gthanjbbav.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pengpengdd.cyou/gtilmhvcms.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhoulong.xyz/gtkuheqomh.html

[J06] 计算两时间之差
来源：http://hz.zhaomingkeji.xyz/gtepvhilbj.html

Py:   (end - start).total_seconds()
来源：http://hz.wangdashe.top/gtunkhqxes.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtpuziqept.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtyvxeywjp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gtzzpiwpdz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgfzy.top/gtugsatrzf.html

Go:   end.Sub(start).Hours()
来源：http://hz.hammf.cn/gtxivcgaps.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gzhubu.top/gtymlxhvuy.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydjk.org.cn/gtuilecsks.html


<!-- 参考信息 -->