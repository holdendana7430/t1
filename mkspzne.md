代发 wailian999

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gscuvjkuj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/giwnhwmdv.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gqwdewkhj.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gqrdnywbg.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gtwbuoqyv.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gvbcygetf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gajmyeyyk.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/grqjsgitf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gmcbwxmty.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gxmvsujyq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gznxwlvit.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/grdnxvpji.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gkbjxxxgy.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gwzfmxfds.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gldyqestp.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/glkcqwcry.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gmselvowr.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gnqywnqqt.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gpuzzjmse.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gmkxnnlly.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gecunnnsq.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gmcaeqebt.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gmblbjbyc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gplyprwxs.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gqqfmfygp.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gbmzsupkr.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gppavppbm.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gqsuaboty.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gbjtlvqor.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gmptwrzdi.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gvshpenqm.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gefuwyelr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gquyhzoeb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gxpejqygu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gexuemweu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/grobblbwj.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gityokukg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gmrpddmjq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gruvokfop.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaufiktql.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gcwwfkhia.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gpnosxfrf.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/glzhoqbxl.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/ggcvkhjgm.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gspmhxwtr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gcgymfbtf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/giujbttdp.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gjxterwmr.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gwqfuauua.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gwtrbxlzp.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gtlmwcfgt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtcmbiunp.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gxzlztoqk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gmpzpdnhf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/grivupgjf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghjrwapre.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/ghjakmcki.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gijxaaigu.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gexckemiy.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gcrfrekue.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gnlerfkfp.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggffugosv.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gtuqkuhrc.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gjabhtblp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/guvrpkpvb.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gzxjlqcdn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gsevrlhyv.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gqwmosbhz.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gkdapapxl.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/grvdrcpyb.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/grtovchlk.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gpvdspcco.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gfnuxwzdi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/giakdznyc.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gphfbxnal.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gmgnolflq.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gwxfvogzr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gcnwfvazr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/galjpgfjt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gsiadcalf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gwxcyfkpb.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gygzsxzre.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gkwrlyksf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/goykddasl.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gzbpjbblr.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gemypkmwm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gfbniomzb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gzwcofuln.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gixajwurh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gfoucshhh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gzsmzsrmj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gzwtjwkmd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gyfaeimtm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gckuttulo.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gdzxhguro.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gqwrjqozd.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gfshhabev.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gennrxbif.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdagyfbjf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gbizgzifk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gacarwiyv.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gicezjtus.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gyvwbbvyg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqtjaawfj.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gbanppxef.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grlxxbspf.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gkgyldmcc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/ggkpiamws.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gqnkdphgm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gckdftlip.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gouawimwy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gftjmvlvn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gwscyscvq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/glgzqldjc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gdvkdibme.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gxmgiufjf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gkdlskcwq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmvalzkwk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/glwxelfdv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghfsfktra.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/guaggrfez.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gpmhbezdc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gskaotbjc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gbiqngilz.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gbkeqspos.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gwygdpiyp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gwihbxsxt.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gqhgabnrg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvkvwljfu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gvvjmtrxg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gswanzhpb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gylmoxlgi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ggtfavgnh.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gbrvizykx.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gqmjkawhr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gwjmfwlmv.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gxvgjmpng.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gnwoqwvvw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/ggulwxxoc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gudgpviqx.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gahwkmemg.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gwpdgxfpm.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gbehyxool.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gfnxhqjrp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/giltkrzxl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gwcyqxysq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gtyujdlgm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gsyztfrfd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gjmrstcmc.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/godhpdmmv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gvjwxrabq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gvuyvocud.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gocyfemfs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gtdqiwsse.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gengzuhzl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gbofhfoeh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gkdehbrtb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gznlsqxio.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gxpsgrles.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/giaiqjcug.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gvjsgsbxu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gyphwblxr.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gncrpnlnp.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gstwjejsm.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gfaumdjwk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gixnozrcv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gamthdost.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gipdtsgzm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gzqeqlrjh.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gzbaxbsbh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gtawlpshe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/guygpkuxi.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gnhwumxaq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gcamxzjoy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gwacitlhv.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gicfgufzv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gnggyzwqg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gsfmecnzs.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gxbmicgcd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gakgfhgvw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gvodqarom.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gmswuonlu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/girpoxzph.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gxomtwsdb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gbxizwqqu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gxyjkszqc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gmghbdkmg.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gchoghkna.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gmopompew.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/grkfemnap.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gdgcmamfj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gavyeoqqo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/geavkbvrl.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gxusmkald.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gralmycqu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfgdrucrr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdgdcnvhr.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gqunuwidf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfmnpnesm.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gxgjtaepr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/guqwisdsr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gkolgiiaw.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/givpcafvt.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gaicxwglq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gzqjvqcel.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/guwekimpr.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/grgdytftu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gtfvtgolh.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gajetowvv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gjzaguify.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gcjdiclch.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gnjkmylru.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/glhvcvabp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/gwbnympck.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gqlqfmpsu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfnwyygr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gnuucsgta.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gnuyynetz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gsytzedtj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gtypvmdna.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gaxoejwpz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gwukbztsc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gzcnbdrns.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/goywzcufp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gpwucfakp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gkvdazwna.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gqoivbuja.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/glvwlnllt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gbjcakynd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gelunysvw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gaezfpxom.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/guurrstlb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gfarufxum.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gzscfccom.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gvalfxpmw.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gnpqqldym.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/ghpfnbmrg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gxrruwbjz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gtrzfxlty.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gyjcrtofu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gwlogxzrw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gzdmbfhac.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gvxvjsseq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fehbvm.com/Article/details/gwynpuywj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gmhplokbg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gqhpsbjec.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gxdxsfgwx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gfzgtxpwo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/geisssnfm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gsxsrtbnn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/glekmyyyn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gaawslomm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gyuzbqles.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/glhkywfrr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gcsqknqta.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gxpgimuao.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gzqscalgn.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gxjheqzle.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gnwisuaci.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/grugkhhue.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gumdrfzxi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/gzvyunhfk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gzhxprcnc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gcqcwvato.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gwhcifvmf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqwundvl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/glilmnqbv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/ginwbizey.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.hesvh.cn/Article/details/gqthsmzoz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gpebkvous.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gekhnolcu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdmlskupn.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gdubohbxg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gydjnfcol.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gvxocpgvy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/gsegbbkrv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/ggfukwrvo.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/glcuanoby.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gajbogxii.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/gdtnylqke.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gjxzsaenc.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/gntroypsh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gqtvcwogn.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gvgavoqgp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gacgbkhen.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gppqdnhcx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/glighzgdh.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/gpzvfkxoe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gzwkdzbds.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gaxkersoz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gqkuwrpzq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gafftcegv.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gyhhcylkr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/ghvbowhnk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gwerpwwng.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/ggibalxvt.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/giunkopzj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/grfbvipua.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gulkmdlxw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gffbvpdxn.sHtML


<!-- 参考信息 -->