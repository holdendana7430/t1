代发 wailian999

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3thvnrktu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3thmdmmem.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vtgubzci.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dsthnfaz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lishkksg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmgegnlc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3akfuwkdf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuufcgye.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vyhkvnvm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hfdkwoxq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vrhrzdwt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3mstzsoai.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cutkvxyo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3remwzzdt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdkltvht.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vphiqdxq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrrfpffe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fdbwzfqt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hkqdgzbg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbqrqmwn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ehxicavw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fhuzmrev.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qmpcfhjb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iabtdqay.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hpbyqjwl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sozesqdn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jzpmrjsq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3cnbkbaun.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wywnuvah.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3oapgughy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ccngwsvz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ucfivsok.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iojtpngu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fxikklil.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3asroxeng.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3lnbheayk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ctqwgxci.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3rxszizja.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wravotca.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wlrwmfmw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3sqdywckj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kywssphf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3agzbeugn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilukhubt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tsvbkjdk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ynprpaew.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gismpsuw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ehgwzvce.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vectcmnr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3szmplbgq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tiokmkql.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3npxnidxh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrxbjggn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3eyhmmsea.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ktruhkae.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hofpktyd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3bswzcuhe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3tchzaqip.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nrvqlcwe.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3apxgjnxm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3teyxtqzd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lewoybxj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3nrzsmuzh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3phbvdfbf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3askycidt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ervrakhm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3iksoxump.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnnrijnh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3twsqenyg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hwivafoo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lzrtznxc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sumbggaa.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tcwphzza.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3prtyqpqm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3jerkfkia.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xrjmeaca.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kazkzdit.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfpxemqc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3poslokqw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kikhjtdh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jmszrfby.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ykmhxfaa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lkljufvi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jqrwynvv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ggqbgiwu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eswfzgil.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jnicglrx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hkuqugjp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pejwrrsc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3faucsttg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pfdlmmlj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xqcpocfj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3wqfgqnhy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3vzgiijuf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3uejpeqvs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3cezjdpog.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3hxzhnweg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwsbzvqj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dhyeqgzm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gxtkayla.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3czsnestu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jyhfzhso.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wlimgccx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zumhmkmd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3zuiiwhca.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gtxkdxhc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3joldgflc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3hitgddnt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3halgylgw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tqlnsifd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3syydlaxi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3vezzjabr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zaczuaeo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pyeuwypv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kvzusele.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vsrnyojq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fcgdyigm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qrihnczs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jtrqsngf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzgusbqn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oylmjjhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zymkjavf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3jfaxewkl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ebopnxqd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eungnyxj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xntvcxbo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkklzqrd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wiqfywwp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3atxoyrfx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3wncydnys.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3censljvj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3cnslmozo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3fxlkrpil.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zttucwyo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nvdwmzfs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrobgqhs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3drnzouwj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3baljudtc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vxqfkmva.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3idovegqa.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dyyvpwdi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3kythwvmy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yenrmkin.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3atnmkpzh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tvsvosdi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xthhpnpa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3krwjgevb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jsemntyb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ioeddnrw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3flicgqpi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3myvyyqde.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlhkmjni.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3phuztuqi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mljzohwp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cgfefpsu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3opipoanu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mzkjjhfa.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3efktbeuj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3gwzhzwkm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3cebjjpcl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3zqejqclu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3goxdgmwz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3areajvox.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ociscenx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3kjxlsxkf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3lkhjgqao.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfsedaox.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3prltdbvm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ynzpdldz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gccrwcgo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3knyaztwx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zfhmwulk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3dbfhukqo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3avtdmvjc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3vgvculzp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hzllwoab.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3lvavnqgb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3flokptmd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3otcpzdmz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rknvnmkl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ohcbuedo.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3qvchwjvn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3uccqenny.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3kyamlfox.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3amkxlvpc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3lzvxgtze.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3gpchsgoo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rnmvtgee.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3oehgxnym.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tlfjadhq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3bfcbwpmb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3qggmlydn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3gwxilszq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3mtwejiye.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3rpoudokr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ktladsrf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3iejixugq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3wfzbvluw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3pdtgicpb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylebeile.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bhmjokmf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3qfjsrvcn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3bcfjezdw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3vnwhzure.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3rebgqqzt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3jlisfawt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3uewnjzfo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rkxipzad.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ylpzwvur.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3zxesyjsh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3juniidwh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pdewgrgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unosmxgb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3euicdspw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxpbugkl.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3aggcybvm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3tzlhghpy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xmdmwkjx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kskkpzoc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxracvxq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3vetuayjl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gsdomets.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wyveyfaj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fywtqwuy.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lhldmaau.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jfhedfgr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3eezikyme.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3woyrcojk.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3xcukdjmx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3baqxohkk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3klsqmalv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3gcuuotxz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nkvlelin.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3rhjgqnco.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3byewescm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3syavqgge.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kymvlobg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3tzhfqzht.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jcdfaebw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3buzcpxwc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ojhanmia.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3otobixzs.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3lcbsempv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3awbzbbvl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zzutvwlk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3atssqyhj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xewuxjpx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uvxyshtk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hudgzyuj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3tkvneoqe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zviirkay.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nzumeorm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggxwrshs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fviszgmv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqvwukk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3eooakeij.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3uykwrsjv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3szawigkq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3briisggi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3tgtkfila.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3thabxtwa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3awyyrgec.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ppqpfcen.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3jvxqysrj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hlwahcsz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vssrinsc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3gybzibzi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3qsevpggr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gvgrzqrf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3pyjxyxbv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3wwheyfpp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3wenzvblj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3jmdqdcbc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ljsymtlf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3srxhrrwx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3oneupkfl.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3adbpbcol.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ochvxnuv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3debtbzps.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3hmqivvka.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3onuaoqbe.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ypizmsvi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3yrzvzgyd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hdwajxfi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3vwwtgrwj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3cwgnqcqq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lrutcpgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzzulsxq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3khjhfpvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3istdwjat.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3faximcpc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvvijaf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3dqrkoeeq.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bwosembe.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3whnsqvnz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3nypcwxov.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3vhxovrha.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3oxltyjof.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ghakvizq.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cnlcslxm.html


<!-- 参考信息 -->