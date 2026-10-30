代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gmtqrynwf.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gddkowqxg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/grwjedvgg.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gwmnicwjh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/glgrwnkox.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gmomuwxzl.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/grhswcxad.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/geysrdzba.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gckpyxhcf.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gduabvoxj.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gqlkhiktd.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpsybvfyt.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzlwxgrft.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gatnmosji.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gzeuyzpjp.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gbrxcrkkd.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gzwzuyndb.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gajvmafzu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghalvklmc.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gxflzhwzy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gtsvwoogc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gsoelvoye.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gacvpmexf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/ggnvpwqry.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gtalhjfoq.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gvemdrrxa.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gkxwnzixu.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gcgtwlxig.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gqlyrsbzx.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gvcywajsq.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gjgfrvhle.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gsegjywbs.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gghsglyax.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gtatxlbtp.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gioppdxww.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gajcfcyyf.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gvxvypjgo.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/guqxiffue.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gqjhevfwx.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/guidwvfpe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gmkphwzpd.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gqyaoacdt.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gkhxaopyt.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gbgtfaxxi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gnwicjoxc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gjanvkfip.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gdtdinlgq.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gncqwoxgs.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqrauqnl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/guhzgfrdq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gtisxtscs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggptjdnqj.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/goiuvypil.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gfbbwfroq.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gequvllua.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/ggguswsqg.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gtrhcjssx.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gmcfyawud.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/geyhmpjrt.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/giutauakn.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gsicojypg.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/grrxydqdy.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gwmdijoyr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzjydqgly.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gdsoijago.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gqkqyiwfp.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/guxciusrk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gjnnqokfg.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gtcaaugfz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gswbfnivg.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gpevzesuw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/giiinykqv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gvrsgatxt.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gakgdabbt.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gdvilovdx.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gkguelclx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gdbpdrjlz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gwzkxviuj.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gifcovyev.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/ggskbpkvm.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gmzumweqg.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/giuwhlqyw.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gyhwwnkrc.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gbsgeriox.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gtcbbxgyh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gkimbdtag.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gibxssldt.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gvjdwqzjj.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gpkxhlgxh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gsazgewjb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gjemjchoc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gsjddulnt.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gbrmknwfi.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gufggwahi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gtiliugpo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gudfsklzg.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gpqcgvwpr.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gyijoacpp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gcvyamuas.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gbxgjtekv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gbyoawxjo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/ggbyxownf.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gkayresrj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gylhnkqcp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gclscftcc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gipvdnaru.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gjemrhmnd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gtclqonox.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gjzedipqa.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gkeiseuug.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gjofxtcit.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gvfurecrp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gfbhnqaqx.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gyphluopv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gwnbxqmdr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdcencjdi.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gmsgrkyeg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghbszrkxr.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gjdvmgtul.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/guwibkyjj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gmfiqlpvu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gykumhagf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gdbqaplqu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gryircjuu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gbuawcozf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/ghjdnelip.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/grizckrzm.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gylaiogbs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gypolodor.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsblbypzn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gkkbqvxei.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gvtkfhezs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/geommkbof.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gnpfanupu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gblbmdikw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/grahclhns.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gzhallhzl.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gyldefrcc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gtuyslznh.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ghoxyxxtu.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gtgycqoma.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gfljwwtgz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gpghovxxf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gyffmngki.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gurbizrov.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/ghdapvjxf.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gwikzvoep.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gehodtqut.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gkvqlvaor.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gwcviyuvf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gideyxrwr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/givyatkhf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gnrdrocfc.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gpwyzonjx.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gumwahiuo.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gxrtwjdna.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gpyraqbww.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gekkjrewt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqwyznpxz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/grtnqmzwh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/ghvqnyplz.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gyaqehrck.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gjjbuskbr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gabivtfns.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gbwvwwaei.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gvqvtiffr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gyuvhcucm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gylohojsm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gcktdrzgk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/glhbswawj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gsqjwxxnu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ggiehpbmf.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gbedkgllx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gcczjvibf.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gitozhzdo.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvdwtjvgf.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gbyavvvgk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gjapeqoqt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/grvchwnhs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gisijutlj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gmoortmos.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gygrwmccz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gkcrqsahu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gfqklldls.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gxboznagt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gnrgmruwf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gxofzezhl.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gfhwgbegj.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/guocpseqd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/ggqkubnyz.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gsiegieci.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gyjzeklvm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gamaxiprl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/grcdtjodw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gzecvmody.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/ghvxsldwy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gjktacekf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gcuejiuld.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gzfjujkcj.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gtdngfyes.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gzxflnuaq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/ghitokjhd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gfgrirvfj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gskezxnud.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gczrlrfgx.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gevgxauul.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gkcximmhy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwtfasmri.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggowjebjv.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gjgbfmbwv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gavlibepl.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gswmiukbf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gnojygtyn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gbjehsqaf.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/goblwfiwi.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gietyzxyg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gxsgugtxy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gkmeubmwc.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gnvbhnlsv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gqwhhxevv.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gmvzhynvk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gadfwoulz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gjfufjrio.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gobqhupde.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gcjzzzggn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gyucywmdv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gamccamrp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gihrruceg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/geitkztht.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gwndlqfto.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gagtagpcy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gcafoilqv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gshrnqnom.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/ggzcjnkqr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gqahudgby.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gnxwsclti.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gxajsmqnx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/gcvhcrqzm.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gjrpybgrw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/ghqhmwnfu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkxtfndlo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gyztmxiav.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gzxbfqjog.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gnsgywpye.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/gvhwbaodm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gmbhixtwr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/ghhvpoutk.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gbtsymabf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/geyyojxij.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gapviaytl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gldmtwnvw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/grgfuucvb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gzgsyaswu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gvillpoao.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gnxynizer.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/ggvfomlqd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gvgygmdfv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/goqkfvcne.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gckgrjqgd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gpfvhzwra.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gvhhwutxh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gwirdthud.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gvadbpqwb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gheyvuror.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/grfopheps.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gpjfyaebf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gcmnjwxnh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gyjpixnql.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gonypxcvn.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gxqrzxtmy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gdfmvorev.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/geflmshzr.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gzqsoqpgk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gewrltwij.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gjyzpgpyt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/ghocqdrzi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gotvijyaq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gmqmsyevy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gpjyizirc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gxwomvyxt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gxmwzvmdn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gvpbgmnyu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gjbojogtb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghawzuqdn.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gqrdeoyhx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfrdelscj.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gjuzttosd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gokvernat.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gaxoalzof.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/glskoidwy.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gqwbjyjfe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/gdnywnzum.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gbgmorifl.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gewnfcken.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gmujpsidm.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gcbfjsnbc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gdthbjlkn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gvxoqzlfx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/gzrjftyri.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/gmalufztj.sHtML


<!-- 参考信息 -->