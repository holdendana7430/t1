代发 wailian999

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dvbucsgj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2fefzxtyp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2enjivppg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vjwvpbwz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sqhhshmu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2outgwsxn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytgfvywn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zzzgrcgw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zfxvlnbh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kmqayeul.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rmgirogv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ktgknyrk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2naonbbgf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwccvpfl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2symwwfzz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mewjxmlo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yjmgruvw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bppzjwoz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mzhzljlo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkgohbxp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2sljrzzju.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mdbwhqkd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mlkwivhs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxexjvrv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2exiemtgv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwtyryst.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ridpafxp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2arhroxmr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mwcnpbxi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bdsizwky.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xwejmozq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2icpeucrf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kviuzixg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zhbekvow.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2reywaape.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2waiebzou.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ermdrest.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2czvcrebg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ixmaystw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mqnhzudi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gbokxhox.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2frzxjqfq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ricdsdtw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwrxduve.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qqwmdklf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ujgbkvaj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2uuvtaywr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2uqxfyvwn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vzkqwltf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2anwnrkms.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2icsnrkep.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mskmhhts.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wriqmopz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ovmptxkv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yfgpkkkk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2iddsfybv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ajwxpeyl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qwzlzxjl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bglmiqyy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2aeivwcvx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uayfbclf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hfoneoii.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jemaimxe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pndctyzx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2egifjhql.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2yanhrkor.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ogsvbrwy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2clscbnrc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewtrltxk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2luchyekl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxzdyocx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2avraefdx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lupuzdcq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2wipqbqgk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tpppwenh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nfybkshs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktiavdln.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pqbcbbit.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayoeuwse.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lexqlvsz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ubnbwgyw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fyjhceyp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ofpfckac.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ptiahjsc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2fuvlpptv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zfdckfrp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jrhajrhj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fyweokul.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pkqdhzxf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mbuwqjxe.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2aasgnijz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rshdspas.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2kikregzw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pjkuoksl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2yppzzcxd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kwlsqgsw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2jvrxwylj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bdbgppyv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tsvkfexh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2souepzou.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2mmsswsnh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ulammaox.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uxhjxiiw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhuhygzt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2sjziptwf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ecoljkho.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2zunwphbv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2kcdnkxsg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2fxqgldxf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bvcehiyb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2eihkdgke.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kaxjxwbz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2qyujrklb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qwbvhixo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vetpqlix.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2deolujix.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ngbmvsfb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2bnevqjjm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tvmwpdam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzpktscw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2yskhnvve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnyapmbq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vbchuiby.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2eufhemna.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wangsbpo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykrjmvdc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwqamcne.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2epqxwjsb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2khbxaeri.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2iveaicok.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2nngqpdrc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2limscagf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2gqijjeke.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qeezvnkm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxbplwdz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdxsxfhj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cvjrtblp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pfozcfls.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2dhsdbubs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbgjquky.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tauuqglr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2hfhnqguu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pqklodfs.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dthjdxos.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hswqmbpe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ubqoihsh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xarbogiv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2edogvtyw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qvwvzhba.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2vodafgvy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kagkdmig.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tevtoljg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vejqstwg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wazmgxpg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ifebnsnc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2oczpxmei.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2hqynpasy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fzavvubd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2roqtrfgb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2wgjcrlxu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jwjvmoqj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rmjinmgo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yisdjrff.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2onxhzhlz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2jdypjttb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2bmrzvdez.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykjraekf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ogtujgut.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2izmxwjsf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hhvwipso.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2flijolfb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hbtnzesa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ucciaygh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2gxtwjvfz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2nrdyerue.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ucivgxll.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2egbbthnz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2cmvkagxj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wqskommp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jnqwfeua.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rwjlfbth.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2pgspznbz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xgurisek.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2thuunarz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zjsynjwv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2gqlyxodr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2sareoicp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2lmqgfyiv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2axyhnjax.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rtomwjjn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2zbzokczo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2lpsbgnqp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bgxcdhlp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2hglhrtgw.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2qvszyrou.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2frcqapcp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2kbyiciga.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2csynwkbx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zcylpeim.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2opmbaevn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ewejnrml.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2uyijveqn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2qnxeesgn.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2easmreyg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2wjynuujk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2hixycwjg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mzdjjqow.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bdkzdkhq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2olumkqrn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2rizrltkw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2fwangxju.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2clylyjok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dejkctbo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sbpsowqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfbzqtdg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2afiupzmo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2watalacw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2llflandw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2bogaksrd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2svagghlq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2qagbhknc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofzkdtmf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2grrdkmzu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zvpnjfex.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pgkwmnrw.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ffgqfjxb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tdeotodl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2rdcdbxcz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2esqaiagr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2xbrqnwkd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yostombv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qicxvyxj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qgbjdvog.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2wpjsrnwj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrxmjcvx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hzplpuyo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2uhlsblxc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hourbggn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2oporbrsf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2uwiwtdzq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dubsdudp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2fdoyxmak.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pooblgih.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2gsxpfsgk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2emqcyouj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tvzrcdsh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2srmkmwwe.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mabewexe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fchpfnha.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2fdpcljkw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2epgbatii.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2vvenfoio.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdbptaqh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fpsckviq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ijnukrtn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yhcorylz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2rbqbdenv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kquimbxv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yfuznstj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2fpltjrqc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2qkksulrh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zfomwidc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2thsnsroe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hoadffhe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vomhucza.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2btwcmmny.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2zxskdpxp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2snplrwtt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2epdknlpa.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2vrvomgyu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2adzgsfgz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vjdfbhfw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2lxeqizct.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2hsqdajqz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ibexgdrz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2fyrzixud.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2pupfgzbw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2gnplpgie.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2isrsauzh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2nvsgmvry.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2aiidupbv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jsegbbqd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rczlaimq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2mmzpucio.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2osbwfbmg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2dmjdluig.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2spktnezh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imbyahyt.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2otvnnmyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwfmudkh.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2mvnbafhl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2rmjyhweg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xxllgnte.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xoxtmsin.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2nousrpxx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gdkpmarg.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2zzjzyoon.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2npeulvgr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2xljzdevl.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2obkarpwi.html


<!-- 参考信息 -->