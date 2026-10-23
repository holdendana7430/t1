代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mojsfrcz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3arprhsgq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gxchjomq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3unsvostu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3knlaeuxv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sitkumiy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3brtoyurp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3odsmmmww.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyvjbzbw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3xmjbdwsn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vgxzeltz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxevsjrb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bzpuztmk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ykdkipgd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbtsknli.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3swsbmkxy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3trruddxn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gupmfhcy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3emvfjxok.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xfeyejxd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3vtwpcomy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3doeqzuxu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hzqpzizc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3eluauvdz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zmjvpvbp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hpetkarg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xqkbgaay.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3txfytxno.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pelthbyl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3iuravfmj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3eduewneu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ouffwrfc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zjdhrqzf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yissgwbh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zukshyhc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3afsynfks.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3yzmqabdh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3lfmzaixv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vellkvpn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kznkhdhw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dtuwkkgq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vullyjcr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vpjviheg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaadesag.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgqrcfbt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wriatkym.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ddavndmm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3aqeymipy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3scmkzori.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lgoaptqi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vzgjmgwf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ktzfjbud.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lwajwstv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3emclxtot.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ozasvizq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ucsejfbl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dassucfq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ykzqtuze.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hsqlawia.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3taaahuku.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yjurycvo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgkzgbkq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgqijsdy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kcaubapy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3gpztfyhk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3stbiggku.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sibcdzyw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ajjfeclf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dheewfpd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewwwodgh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tojcxlve.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3osjkmmxh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oybcynmz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qgajynwc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mhqeesgm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3atfehjad.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3gwqwxmtn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jvlbyivj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3epcixfkq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jkdcupka.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zuyfcvvs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3pkhhlgvr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ktmnjual.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uygowbjb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3yovfdnjt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ifxsvolo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xonimkiu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3buomimwz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pbcpczwc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kgmjmgfa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3fzgblgta.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3orcxqtva.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jodjpqlu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ncnbknrx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tcjomshm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rylwwghe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ffqlzvqp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3slptjiho.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3xejpppfn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3uahfdpfm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ifyjansl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fszlrqfz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qnhboqgt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ptwcogrn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3fdpaaklw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lyquibej.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qjfnjogj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xgirwpnu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tlqnwkoi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3owrggyxp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3swcovgxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvuhciwq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mmgnzvdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikkbgnba.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3umxlojdg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ymnsashf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsiliwtd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mayitoil.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fufugyou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hqnxdixe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wgdulwtx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ggnbzqqt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rwvlvtck.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3mdneeszb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3uskyyxlk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wosbeeyu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3boumulny.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rrxpqhxw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3naohqxft.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3hfsygwdj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fwkjfbyv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ifcxwtul.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vpuuyftt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3tlspdpgt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3izmksxpj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ixedpunj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qlroclyk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dcgsvywr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3vsilgwzp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3mvajaxyp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ikoigxnp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3wldnzqml.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zbbizvwz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3acwnddie.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvzjgcng.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3azxusjru.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvfuibzh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3pphlpmub.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3gxamskvk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3iigcmqtc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3fizrbwjy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3eizqpilr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3qjrexfku.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vdoozkaz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tlbnzjuq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3yzaoboyb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3okmbzdyk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3abzpnykp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsgpghfp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3cciegast.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3spiaggai.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kstugqtf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ilxecrmb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wniuomwk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcwvfyz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qkbohvyn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3vemijkuv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ewgnkwjz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tsfazhio.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fngdyzby.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3puvgdfqh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fvlrhful.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3inioutor.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ezefwztj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dqbahvik.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3eiciepgj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3atmhguiq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3wtasgcns.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3djtesdro.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qbgaafvc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3eaffqssu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xwsncste.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3wvbqfgae.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ygqjqkcl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3amvwzroo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3cijpkaay.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3kipvfvid.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3dyosowds.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wdjqlvgt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ygziddjz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3rrspgmxq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zslupyqk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3yqmwqwlj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3gapogucp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3xlsbdaxz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3twwrjzpd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3uskktxqp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3lrnqitfr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ovabtiuf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3nqbowrra.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3hnxrremw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ungdxknu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3wcbhpzcx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hqqcwkfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlsixuna.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gmhfuqwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qslsxikb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3quuzaqch.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ybsvunjf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vdjduggq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xaqxulhj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fvbxakmx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3kvwfdvzi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3xnofljgj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3adhjsvfs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mjesmosc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kjrrxbif.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gplsvmjo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3abfwjnxe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3rryirfvf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3issestzf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vzgzlydu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3nlubbejl.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zddjlpqj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iqjujbyz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3mdvkaiil.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkypvbyu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3roxpegyn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3fktmrjjc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ysrahtzp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3lhxovxhr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3fykquyee.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tcwwznic.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3xhfvyyto.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nejfgdes.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3obnjadxw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vwazsfev.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3qgpnhwzf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3yomgfnxq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3goznbydn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kgcvcgus.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3frtwanlv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3oissoumh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ddwtgmro.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3bhcvuqbo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ukttuwry.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rexukgop.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vwuhawbr.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3botduebl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtupphzb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ggvrcxdy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3fvpgiezw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3zuaqzrst.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3olhxokbq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ooyuoeab.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3swgmmbfa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3opspqdqy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yzvqooda.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3acjuhevy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3rfzoljuv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ftwkowlx.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3xnseysuj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3lqposipq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hrpeomrq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3kienizqz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3yxfxbnud.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3tlrpsbhn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3kwyvoydr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3uxlpyzrl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3qejpadad.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3klhnfrzl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3wlnytvck.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3yydztlbf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tzdrqvqa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rmtljmso.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3qvdseoaa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3mkfrjofi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3mkirvscj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ybhkiqbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mptohqbq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3wflcqxgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3netnuray.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3wjmphutl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3mtyoetmn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kwbltmzw.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3liohibzb.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3hmowfsjl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3yurguoed.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3mmancufh.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3jrgigutn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3dyqhrjdk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ragpjlek.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rarrcofz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jmepyqas.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3kbvyycvn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3nokpaklp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3tqmebnpq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3igycprgg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gzcthwsv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3rjajwknl.html


<!-- 参考信息 -->