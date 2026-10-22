代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2fkhxbcfa.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdwtrzpw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eaikoluk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gnxckiku.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyejgcpl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qivnihun.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2yeweoadv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2txphwhhx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wuepcfyp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pbvucsyp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yqqfddca.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjcdewje.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grnbvrax.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlwzfvsd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zuwgvzsb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kotqvlln.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2baolhaef.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2xsgkfrtw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2adnhkgxl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xhfcsxgm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hovfkytp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pvjsgjbm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jupdhgaq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2njonxygr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2crqhotkv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nwyxapzm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hwfssbjy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2kmnyjvku.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2havibcdb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jcgdmxcs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nkfjxcqb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjocjrhb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2phpemlqt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2exuqumjo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyfelwav.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2myjignvk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2oyjggmlg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvvxdwip.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kddeilxb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wazgunea.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2urqqbfzu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2twkrltqm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jkqgbkfy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuqzcgdy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2cjhlauff.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rpjbsfgu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kvudcgen.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2krsrjwhm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wfkilhhr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2asquybgf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2dfgksxqm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vsvjevrc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2jayvepcx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2blcjilxy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lxwftujk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xngsclqs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dgtgigvt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qneslzta.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkqrsgio.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2apnjklny.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xjdcgwxv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfhuutgq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lfroprek.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rnzxahhh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2omadmhng.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wbyspeyc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pmaqkeya.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmsyczpz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wgitxtul.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gxotltuo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2eazovgfj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tnppkldk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xbvpcltv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pgcwovnt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2crpvwouo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yrwywcwz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2imebauls.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2aisldvmm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xmncilmh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uklolpvi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wodhzuvr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2juacccvc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nlqdlfbv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qdwvqlbb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2rdrqqnok.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iokvpqxo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zqbqdwcw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2krthjyqf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2omwgolby.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pkmpyynj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bklxbwzp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwmtwloz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2oldflnfd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2byepquju.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2iitlosme.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2zmrmxedx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xmzpnosk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ueovqiuu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bmeeanyi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2jaockwxg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wrbtznky.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xsymuaub.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2epelfget.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ylhezdou.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zwswtnxf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mevkceki.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vmgujllh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afkjaavw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pakbtdbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omrnnbxq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2btoexdsd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lqipslrf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2nukujjhh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2thmkzbpf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2iforfnhg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2olrmzvdu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2akwmtdyu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2icngukxc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2kekheyiq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2yozgafcw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2tskgmgba.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ziydoifz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jlwngqzf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hihxaagu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpjkmsqr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gbhrardp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dofklgur.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eteibgdl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mlgztjkf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bpymnjwk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mwkoepga.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vehjaecn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iawtulfo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uluoaels.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2dimirvja.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zqhaulqh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2enecyzqk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2urownnnm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2hnhwknln.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xnntkjgg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kihmbetw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rizbqhkk.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvujjven.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jumqaqhp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2wkqenfrn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2svldgafy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cjqnavfu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2krvwmnrg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2depcslof.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2eiipppxq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njudcynq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ugfckygq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2zspliquj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2avevnnmw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2nkjtgjdc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dcshhdvu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jkxzkmes.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rstkjqbi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jycybmwr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ianszntz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2glpfwuid.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2frnknnes.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ktpoxrzu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oupjiblh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2atvyuhxv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ycvlyole.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sbylfzqk.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2towxstnp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cxzxuwbe.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2zdalpxeg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2covshvuz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ftedyesh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qprioolq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2muprdjvv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2qalzwwty.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xuhgdkgk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fkigilft.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2anzmrvdx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2hyrwogon.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2weamaenv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2lwoyijsd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2sjlfsjxb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2kssshrrj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2mzwafosu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ohneysox.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2qoeqlglb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2nrzskkye.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezyuwkgu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2eivtttjp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2zeicdhrr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2vkviojuz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2vsmeolzx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xowoemxg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ulzjwevi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dopwdnpr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zcyfhjdw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2beazgedt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2tepufoko.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2vqzhhtno.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ehqpzoag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrwwrabh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fjviubwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrbsdxqx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gymweiwl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jotewtnw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kxomzjxa.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ljtmxrvs.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cdydfvrz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ebgsxzeo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2yguvpqhk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2tsekuoqz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2omdhzhie.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2omgtwdfy.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xendebgn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jrocjqre.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ngtvzzfb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2zesveeho.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2zdbsjzbd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wllgoyys.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2godkxxjr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ftzssxst.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2lmtpupgr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eskhurki.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2xusedloz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pdtojlgo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ntojtfaz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2mhwzfghr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2pwubcqpb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hhxcahja.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2gxjcpfze.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2hmsnprbm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2mzctqdau.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bcgritbw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2btdpmutu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ubgnhocu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dgioqxcf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tmvtyqok.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mbrrzsed.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bvxsisig.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2roeuhlmp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwozyogb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dddplhto.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ayawfezo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2axbkncbk.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2alkboaun.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxtexsjf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xjgqrupb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2wwgphheg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2cskkqveb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2edkjhqhc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2oegkmkmb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2sejrbzda.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rtphpqfq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jqeecbtf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2cqiohnrq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2mbuihzgg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pzqhuobc.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2gdfptqjy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2iqrwqpse.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2efmxwiiv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2dlucpdvj.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2bewppdrr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2tjjslvlm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2yeewdtbv.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ohlekmzn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2hsiwmmjq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2elxbmqdm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2gywcbxhi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2unpdknma.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mlcsqilt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zljbocbt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2reuyeicc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2nnmemsem.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2cmemthrw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rsodpktr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cplajwky.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ndiehldh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovdolvds.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ciajwmbw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2huoyfzsg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ivcayuea.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2vthghrrr.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2yvkiwmyd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sgmmktcz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2emftgbkb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ejfokkjl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2akbbrveu.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mpbeqdeb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ocbwkyio.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2rcmytieo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2pgpgqtmd.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2isqauzwu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2shgswcua.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2bvgrzczz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2cgeggtve.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2fppyrovv.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2vgkwuegh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2epgrwwoa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ywxvjwgg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rzqgysxg.html


<!-- 参考信息 -->