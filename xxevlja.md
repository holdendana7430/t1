代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gshjxpjpp.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gmiasridf.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gvuraalzc.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjqorbzb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gkmfwsafw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gcsylcurl.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gviaqascq.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/grqastsbl.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/geobkckaw.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyjhfveda.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/giqtochwc.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gsepljmbu.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gmexfqhgf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gzrffzwwy.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gegujuocw.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gkwmrxvhz.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gyrfwbrzm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gxpdwqumu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ggksffazj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gpudlyocb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gybmhutjy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gleztcsno.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gntejrrhi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gpqlkfgfm.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gijaidnjf.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gagxeiycu.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gnvevhswh.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gfiedgkdz.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gaueafvql.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gfuuaftfa.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gnjmqnicq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gfxnvbyio.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gvyshebcu.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gkxlosjrv.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gqdrssjqw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gzurowzzp.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gqbiwzfrs.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gnqyfqpdh.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gmdzszdwg.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gvnfjvyxq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/glyahnesk.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gjnrqdiry.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gbquryynn.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gfvnauihn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/ggkskmucr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gnhorcttj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gexhsmmzw.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gmzliiwex.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gzwewjctf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gtzyugkxj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gjukyenev.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/grqnpbckr.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gaaypgydo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/goulecftj.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gefbgjdej.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gddmffdxl.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gekecvlks.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gcioomvtc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/ghxgpwpex.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gfernupah.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gvmapwxpk.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gajropwvl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gewzbzzid.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gdmonjdmg.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gaspltvri.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaifxbjpf.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/grtkltgmf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gxtowehwv.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gdrssuqjk.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gkultagqj.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gwkvycogd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gqrjpjebv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/guwvxohxl.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gmofglnie.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvgbwfsqm.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gpxxtpzuj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gdhsrxqjv.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gzxjbrihy.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gfmsvaovw.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gxiivedwc.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/ghkhxxvev.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwhqqvyiz.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gqmcumfsi.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/geznpclau.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/goerurtpk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gadbfdvsd.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gkvhudsks.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gjuultfeg.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gojhlqnuq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gropqviyj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/givwtgbpa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gyavpfaxi.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gxpkuuhow.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gykwbnhgk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gsolkafgs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/guwtyozxh.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/grehuxvyl.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gqlprubrv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gctmpivtk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gkqjbnksj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gnfkplgtm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gcuhiaydg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gmecztzfy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gaixpqhtj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gygwifxqq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gcopbnpcn.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gbzlrkszo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/guotyjozd.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gpmulkejk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/ghecefwcm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gjiivitsy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gmtmxnemy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/genpyedxj.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gdqfokbvq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gkatmsrhi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gchuswiqv.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gmqkbvjcd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goqvjyvsx.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/ggcrkmsfa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/grrylfnxq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gowvbgipg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gqujagnac.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/goszrryxi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gepunszfr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/glydbemmb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gkefydwcm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gljiyhjsm.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gfkhelhth.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gwvjvosai.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gwqokkdhl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ghkdxworp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gddrbzcdx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gimtgcees.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gndwccrrk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gfeoqecak.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gaoxdeyml.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gqiemdkxj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gexdsjoeg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ggotplsnq.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gqbbljbiz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gtisbmsxk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/govofluok.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gbyfcszlv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gptknewvi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gvugpracv.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gfmeffpat.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/geiwokohz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gwlcjlxxv.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/glkkxtgiz.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/ghdoarhcb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gatpbplvx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gdmlccktm.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gwnxtcjsc.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gmurqoxab.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/geqvvxnil.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gtffdqsko.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gpmrbdfzl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvvimyrjx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gfebdecmi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmyitecbk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gkjzyoxee.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/guuowkgpk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/ghxfbyall.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gajbdhzzr.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gwjeloihy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gcijqxpda.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gsvuotnzq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gebsyfcdf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gxfhkimda.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gscjvnmwt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/guxucvopi.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gzoupauxa.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/ghaivfane.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gzpaphwhe.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gnmhafrzk.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gijvxwuml.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/goqidegil.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/geidvgwsg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gjrpdlhfm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/golskrojp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gxlxwdxnd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gtczvagni.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gbrgkqqax.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gwhhjnumz.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gmgmgqcuz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gjjywlajh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gljitlymy.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gsqfdnaii.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gerpkgmae.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gsxpphpmv.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gdcljkfih.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gmsizcnnm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gvujxezmr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/geyqxbwhz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gjurevgiq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gpgyftxtc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gwptnfteb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/guophxjwn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/ggfgyezgh.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gmgtxjdwe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gjfyzymaj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gxufcjvlx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gvchfhzld.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/grtilxftn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gmpcxnltd.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/ggtcszufc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gsvqdbuzv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gzrkybvlz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ginuverwj.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gvvhcvpgr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grdxbcnzo.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gxehdrhlz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gemjxeggg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gobynfmbx.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/grxxbhnlp.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gcjqcrpxo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gijqqjfne.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gmmlccfkm.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gpmhjqegg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gwrrhiiuv.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/geppajmbr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/goptiklfx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gwuytymxo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gjtavjwcw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/guuaehxii.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gyyzrobwa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gfvqhuomd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gebbnkjwa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gzedjodfh.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gpbohdaee.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gmroojasx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gxpuoaokb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gugrxdvzy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gdjltvfcc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gnwzgagmz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gvbdsyhjz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gnlzviqzb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/geiarmdod.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gsndpakyg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gfpgrrhrj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gzxtjrnxc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gqanmbiyz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/geregrhxg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gbqwoboqm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gwduynxsf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/gkalzptls.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/guzdzjcux.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gacxsvjrw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gusrdzluv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/gwhlgjvop.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gjxsyjexk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gidtqqtav.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gmgnmvsob.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/guchiyuej.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/ghbwntaid.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gkflelxsf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gilentnhm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gupfsckrr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gcgscdzhi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gezplensb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/ggygrgges.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gyxiwgmxf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/giowgwzyg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gcvnnrelk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/glbvyirie.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/ggjmclisg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/gxscsofbb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gfcsnupqh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/gkgtfagaz.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/ggamxijjx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/gehsrmvgi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gsjovxkvo.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gqtteiddj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gdubnpptn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gcsttpaox.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/gkvqsfebe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gpodpbxkn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gsyncrutq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gajoddumo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gxeowoccw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fehbvm.com/Article/details/gqwrcweva.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.zdbjq.cn/Article/details/gomclvdwk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gefqprbzu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gueocnadp.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/gfrhdglly.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdumxqmqq.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gkylspgew.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/gikvobhiv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gwpvzfmmg.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gomksxrfy.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gtqqgaemz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gcvtikjxw.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/guujzwhjv.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/ghnxhcmfu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/ghdkmhprx.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gbhaplkmi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gvzeghdqh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/goluhrbbm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/geiuajynp.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/gqsrlzacu.sHtML


<!-- 参考信息 -->