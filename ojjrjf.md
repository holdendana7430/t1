代发 wailian999

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gtttbahaug.html

JS:   static f() {}
来源：http://hz.pengpengdd.cyou/gtugdawyhg.html

TS:   static f(): void {}
来源：http://hz.nwbrower.top/gtrthobtvd.html

Java: static void f() {}
来源：http://hz.svipenyu.cn/gtebqdxleb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jqgfzy.top/gtsougjjfw.html

Ruby: def self.f; end
来源：http://hz.sweek.top/gtioqnqmfn.html

C#:   public static void F() {}
来源：http://hz.zhijiandao.cn/gttumiiibz.html

[G09] 接口 / 抽象类
来源：http://hz.fengsongda.top/gtgtxsbxch.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.kuanghao11.cn/gtxfubooic.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhixingplan.top/gtyzhpbran.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gaohongyu789.top/gtslgleqvb.html

TS:   interface Shape { area(): number; }
来源：http://hz.ivvv.top/gthkvltjgn.html

Java: interface Shape { double area(); }
来源：http://hz.ehwqpu.com/gtndhjgktk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hywenlv.cn/gtezjwrngf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhijiandao.cn/gtrqtobclu.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuxming.cn/gtjxfquvys.html

[G10] 访问控制
来源：http://hz.zycfv.cn/gtwurmzylj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tian-w.cn/gteivdbmxz.html

PHP:  public / protected / private
来源：http://hz.yj20258888.top/gthnvjlgdm.html

JS:   #private 字段；其余公开
来源：http://hz.jqgfzy.top/gtodaebjun.html

TS:   public / protected / private
来源：http://hz.xuetiantiany.cn/gtcnbwaxil.html

Java: public / protected / private / 默认包级
来源：http://hz.yj202588.top/gtfhkwytei.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jqgfzy.top/gtwdzutqoa.html

Ruby: public / protected / private
来源：http://hz.gzhubu.top/gtpqhrlfrb.html

C#:   public / protected / private / internal
来源：http://hz.sxryk.cn/gteczuwity.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtjxamntyu.html

Py:   @property 与 @x.setter
来源：http://hz.jlsjyb.cn/gtcjcwecxm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtqirrjdfx.html

JS:   get name() { return this._name; }
来源：http://hz.52xcode.cn/gtzmjpzmwy.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtgescafyr.html

Java: public String getName() { return name; }
来源：http://hz.aibaodan.cn/gtkixfajnn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtzwntgffm.html

Ruby: attr_accessor :name
来源：http://hz.xylfe.cn/gtmyamahzw.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtyvtxzmjo.html

[G12] 对象转字符串
来源：http://hz.jinqigfzy.top/gtazliixki.html

Py:   def __str__(self): return self.name
来源：http://hz.zhixingplan.top/gtnnvvunws.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yongpay.top/gtrsdqpqtl.html

JS:   toString() { return this.name; }
来源：http://hz.aizwys.cn/gtaqbtitvg.html

TS:   toString(): string { return this.name; }
来源：http://hz.daria6918.cn/gtzqbrtlrf.html

Java: @Override public String toString() { return name; }
来源：http://hz.cdnleiting.top/gtjprmrvgw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tianlin.xyz/gtolupevgv.html

Ruby: def to_s; @name; end
来源：http://hz.hnxiangtu.top/gtdnbpliqj.html

C#:   public override string ToString() => Name;
来源：http://hz.cdnleiting.top/gtnrvepkps.html

[G13] 判断对象类型
来源：http://hz.hongshengwenyu.top/gteuufxszr.html

Py:   isinstance(u, User)
来源：http://hz.chenzaomai.com/gtxwpfpwxk.html

PHP:  $u instanceof User
来源：http://hz.xinyue.icu/gtltukaopd.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtingjelzn.html

TS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtrgdhlfhb.html

Java: u instanceof User
来源：http://hz.jiagoushi.top/gtrffrlpbq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jyoumei.cn/gtfhuruzet.html

Ruby: u.is_a?(User)
来源：http://hz.fengsongda.top/gtkeaezcgr.html

C#:   u is User
来源：http://hz.ivvv.top/gtowfkutue.html

[G14] 数据类 / record
来源：http://hz.zycfv.cn/gtdkijskyd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.birdmap.top/gtfopgsaqz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gogol.net.cn/gteggsyguf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fengsongda.top/gtbgdpmfbx.html

TS:   type User = { name: string; age: number };
来源：http://hz.0kj1m.cn/gtmxbxsfcb.html

Java: record User(String name, int age) {}
来源：http://hz.zhengqikj.top/gtcnryeoki.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenlongwang.top/gttpedgjgg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jianghu66.top/gthlloafun.html

C#:   record User(string Name, int Age);
来源：http://hz.kuanghao11.cn/gthoeqlsnh.html

[G15] 枚举
来源：http://hz.jyoumei.cn/gttetpauoz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fzhhl.top/gthllqhbyn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuetiantiany.cn/gtljygrunr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgfzy.top/gtlqvwpbdy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtekjadpyu.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenjidiqi.icu/gtkiplzkkq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.c1oappe.top/gtvmviupwb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258888.top/gtyxoydiqb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gtlvddtbpe.html

[G16] 对象转数组 / 字典
来源：http://hz.xziqi.cn/gtzxfrgyqg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxuanxn.top/gtvjadwhbz.html

PHP:  get_object_vars($obj);
来源：http://hz.gogol.net.cn/gtaoynkyle.html

JS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtjqlbeoku.html

TS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtfnlzpewc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cdnleiting.top/gtiifkqvqa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.havefunace.top/gtycrltnyp.html

Ruby: obj.instance_variables
来源：http://hz.zycfv.cn/gtnfqufdzp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258888.top/gtixujslqy.html

================================================================================
来源：http://hz.9152youxi.cn/gttcxbvywe.html

H. 异常与错误处理
来源：http://hz.pengpengdd.cyou/gtuzphxiwn.html

================================================================================
来源：http://hz.yanxiufei.cn/gteyjqoyyv.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtrvwtmdpx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shangyingyoupin.top/gtkvuyibat.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.feifeiyinyue.top/gttyjmeqbq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.316326.xyz/gtymejivtg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sysykeji.top/gtzdejqeng.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gttnqwloih.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hongshengwenyu.top/gtppgoetbp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zdqjudy.top/gtupjlynrp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xziqi.cn/gtvxdmudct.html

[H02] finally / ensure 收尾
来源：http://hz.nanxuanxn.top/gtjirriquh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ybcxt.top/gtxfvrikeg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtxowzeosc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtqhcfwveh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtuorgtwhs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtcxhpqdso.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jyoumei.cn/gtdczniwkn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtncktduyh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydzc1.top/gtmqhujmez.html

[H03] 主动抛出异常
来源：http://hz.aizwys.cn/gtyywtrmyg.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuanzhike.top/gtocyrfttn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtypgqfbox.html

JS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtygronrlx.html

TS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtndpeouhd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtytbktyoc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xziqi.cn/gtwchldxjd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jiagoushi.top/gtnrkdwfyz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtfgvsnrmb.html

[H04] 自定义异常类型
来源：http://hz.jinqigufen.top/gtijhrgfmy.html

Py:   class MyError(Exception): pass
来源：http://hz.mhx1999.top/gtztvlpief.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtfheznogp.html

JS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtbugqexpp.html

TS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtjsgteowi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.redwolf501.top/gtlsdugxtn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cucudq.cn/gtsjwoztyc.html

Ruby: class MyError < StandardError; end
来源：http://hz.ywan-chungtsiang.top/gtnngkecoa.html

C#:   class MyException : Exception {}
来源：http://hz.zhongyouzk.top/gtohasyufl.html

[H05] 捕获特定类型
来源：http://hz.daria6918.cn/gtjqdkzwix.html

Py:   except ValueError as e:
来源：http://hz.yvedp.cn/gtoqnaljia.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.redwolf501.top/gtiyebuwqt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtmdkalywz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtarrqsjrh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258.top/gtzcyieyoo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gzhubu.top/gtqxvtziyv.html

Ruby: rescue ArgumentError => e
来源：http://hz.haohaochexian.top/gtmbbpeuky.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sxryk.cn/gtfffaraia.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sxryk.cn/gtvmdmdjly.html

Py:   value = d.get("k") or default
来源：http://hz.hnqzz.top/gtwsseizcm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuetiantiany.cn/gtkqcqkpwt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gtlvmmrjkp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtuwsnsfjp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gtxenghvoz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.0kj1m.cn/gtlyjpsovh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinyuanbaomall.cn/gtfkfthpfr.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhijiandao.cn/gtcjvtrjrx.html

[H07] 断言
来源：http://hz.gogol.net.cn/gttepfatct.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuetiantiany.cn/gtvfffhbed.html

PHP:  assert($x > 0);
来源：http://hz.snrcjt.cn/gtpmkhtoio.html

JS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtwgommtxo.html

TS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtajbovbyd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinghuilouyu.cn/gtgbcmstrv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gogol.net.cn/gtsqqcdmgz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zycfv.cn/gtwjayfrve.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cdnleiting.top/gtwbrwyzfq.html

[H08] 获取错误信息与堆栈
来源：http://hz.havefunace.top/gtfgdqkatu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gaohongyu789.top/gttueaeovf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gtigceapaa.html

JS:   e.message;  e.stack
来源：http://hz.chenlongwang.top/gtkmvjairt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ywan-chungtsiang.top/gtcwinfija.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.52xcode.cn/gtovysjees.html

Go:   err.Error()
来源：http://hz.cqqwz.cn/gtvaubqnqo.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gtysmvhecd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tianlin.xyz/gtqdtrvyvk.html

[H09] 带错误码的异常
来源：http://hz.snrcjt.cn/gtrqsptcth.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xziqi.cn/gtremfrfum.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.havefunace.top/gtimubmewr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tanke756.top/gtkmyyxtbh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigfzy.top/gtcnbhgzzb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.havefunace.top/gtpakiybfk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ppjwa.cn/gtgidizqnk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangdashe.top/gtoleidwos.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj202588.top/gtfpnhjnin.html

[H10] 资源自动释放
来源：http://hz.cashguo.top/gtkscfjpus.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jiagoushi.top/gtsyhkmocx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhengqikj.top/gttsyacvnx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gtzmzxrski.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gthvczxwaw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangshuangyany.cn/gtziuxlcla.html

Go:   defer f.Close()
来源：http://hz.nwbrower.top/gtnngayybg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sysykeji.top/gtfvryaynp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtjuosihco.html

================================================================================
来源：http://hz.zdqjudy.top/gtjoiitcwn.html

I. 正则表达式
来源：http://hz.xuetiantiany.cn/gtoonlepze.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtshovytnn.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtkjssyncr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gogol.net.cn/gtrzptartc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtzoyzcwmg.html

JS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtmwoucryk.html

TS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtzhgqefbr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangkeji.top/gtuedbrfpw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sysykeji.top/gtrqumfsoi.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gtihmraxto.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yanxiufei.cn/gtylgtfigg.html

[I02] 提取所有匹配
来源：http://hz.ehwqpu.com/gtmambuvei.html

Py:   re.findall(r"\d+", s)
来源：http://hz.haohaochexian.top/gtestnhqxo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gtkesrsrlo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhoulong.xyz/gtxbjriubu.html

TS:   s.match(/\d+/g)
来源：http://hz.zhaomingkeji.xyz/gtdjipgzso.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hongshengwenyu.top/gtualakadn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shangyingyoupin.top/gtnvhkuwon.html

Ruby: s.scan(/\d+/)
来源：http://hz.hammf.cn/gtwldysdph.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.smart0.xyz/gtibaujoxu.html

[I03] 提取捕获分组
来源：http://hz.316326.xyz/gtvhqpxzxm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxinkj.top/gtqeanzomr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangdashe.top/gtcspxupqn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gtuwlugtwe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gtiywymoyz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guannengcc.top/gtefjpboxf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guowangkeji.top/gtekfzdvnk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zdqjudy.top/gtbgeinzsy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.9152youxi.cn/gtarrmfnkj.html

[I04] 正则替换
来源：http://hz.hfpthk.cn/gtkevkgmir.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.aizwys.cn/gtlkyotgza.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtlymujtoq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtmvpecjvx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtomtymqly.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jlsjyb.cn/gtqsxxsqge.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aizwys.cn/gtskgupmud.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jiagoushi.top/gtkjjcvnkq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daxiang520.top/gtgauogfln.html

[I05] 按正则拆分
来源：http://hz.birdmap.top/gtlhaalgrl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fengsongda.top/gtqksxavfx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ppjwa.cn/gtypdvdtjn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtbngueihy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gttijhlwbp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.9152youxi.cn/gtjcykahyu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhongyouzk.top/gtpqdsyfyd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtaiyoyuxk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cdnleiting.top/gthafjeocg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jlsjyb.cn/gtffokhelv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gthxsijjjn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yvedp.cn/gtngcetqlv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtyaqovykw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtqpjizjjo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnqzz.top/gttqezlhzj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxinkj.top/gtuwurtghi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gaohongyu789.top/gtazbjoyhd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtgvmbkbvy.html

[I07] 忽略大小写与多行模式
来源：http://hz.sweek.top/gttejimquz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jianghu66.top/gtigwxaazg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.guowangkeji.top/gtojofoqjw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuetiantiany.cn/gtlekbumbo.html

TS:   /error/gim
来源：http://hz.redwolf501.top/gtdzcgqvca.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yongpay.top/gtplzoezxy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinghuilouyu.cn/gtqvhviyjg.html

Ruby: s.scan(/error/i)
来源：http://hz.snrcjt.cn/gtrwbggqit.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.vqdsnc.cn/gtxsefhklg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ehwqpu.com/gtwtrtwcbo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yuanzhike.top/gtbhczedwc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jianghu66.top/gtkgexgjvb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtbgarsqpa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtwkkskpfw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.mhx1999.top/gtocnilujh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fengsongda.top/gtlenbpogx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ywan-chungtsiang.top/gtxeibyznn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xziqi.cn/gttnguryyd.html

================================================================================
来源：http://hz.nwbrower.top/gtfwhieuct.html

J. 日期与时间
来源：http://hz.ppjwa.cn/gtjqvsurnp.html

================================================================================
来源：http://hz.daxiang520.top/gtghadxfdo.html

[J01] 获取当前时间
来源：http://hz.cashguo.top/gtuyqhygqi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sweek.top/gtllhgehdt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gtigiaqhxv.html

JS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtmehudpen.html

TS:   new Date();  Date.now()
来源：http://hz.yanxiufei.cn/gtkcjodjiv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangkeji.top/gtbwrcwtwh.html

Go:   time.Now()
来源：http://hz.xylfe.cn/gtxxszijti.html

Ruby: Time.now
来源：http://hz.tianlin.xyz/gtvndsuhdz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.feifeiyinyue.top/gtjgzwkipe.html

[J02] 格式化输出
来源：http://hz.chenlongwang.top/gtrtdnoljn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtdugbbekr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtmcuvjnbw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xylfe.cn/gtpinerbiu.html

TS:   d.toISOString()
来源：http://hz.vqdsnc.cn/gthnarlggj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtarvfdqht.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gtzaqrqyev.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtdqcnzhqq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jlsjyb.cn/gtdizllpne.html

[J03] 字符串解析为日期
来源：http://hz.dianchejie.cn/gtugzvylbk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhoulong.xyz/gtslvuarbx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cashguo.top/gthavpfsat.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxuanxn.top/gtrfssaxob.html

TS:   new Date("2024-01-02")
来源：http://hz.yvedp.cn/gtkmqiwooc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtczmzwpzh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxinkj.top/gtzzzzlmbh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtxrqehnql.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhengqikj.top/gtpfqkcurb.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangtech.top/gtkrecepus.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258888.top/gtftxkahkt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yanxiufei.cn/gtqxphvipb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sxryk.cn/gtcexvsewy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ppjwa.cn/gtuzukapaf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nwbrower.top/gtsjvocymo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xingfuxueyuan.xyz/gtxfdtorvp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtrdguajde.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.aizwys.cn/gtxcmkwddh.html

[J05] 时间加减（加 7 天）
来源：http://hz.yvedp.cn/gtxpfzvwot.html

Py:   now + timedelta(days=7)
来源：http://hz.zycfv.cn/gtmqpieahr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hysaishi.cn/gtimamincv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gttmnztxjl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258.top/gtgpvosbpb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xylfe.cn/gttirkmnoe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gogol.net.cn/gttdmuwflg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xinyue.icu/gtozksfbob.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.havefunace.top/gtmaqxhshi.html

[J06] 计算两时间之差
来源：http://hz.zycfv.cn/gtpelcxixf.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtbpvpugep.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuetiantiany.cn/gtnfgxfhzv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.pycfn.com/gtpgehhdmm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtptudqcgq.html


<!-- 参考信息 -->