代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eelptanq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3auxlyajf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jeabzysd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3tvjwgaxc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ertkqujt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nplgrftm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3pifduemc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vktvrfpg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xdvujhxq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzfgqyak.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qkynuhns.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uuuouvwk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rfyinzwt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ibaktezf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3esxsdhqc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3euthojsh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3iqiysggy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3liigrilz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ukpdwgtm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sziegrok.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqsbdkfg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ungvendx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cwrzbtoh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dyxprfdi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3efoaqxqj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hlkwniqy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bgiizwju.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpompdtk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohidtzkc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3crldqkzn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3eqsmmxzt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bldedciz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3pakwspai.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3tnumfnbp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vhhmzymf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3scvesgkc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xmkhzcuw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rrhtdpkq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mnghvzpp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3farblwct.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ysfqjlrg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3vvazgwys.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jyocgdoy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vzbxzyda.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlhchtme.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rayfacud.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltfavqrr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mhjqoyve.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ztipnniu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3jvrvwtya.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3twaadtur.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jwtsobtr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3egvopxff.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nrjvjkxx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tftqpewo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3paitokoi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3sdqyulap.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fbxnhmnv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3pklhnfdf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3quhyeaun.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ylvxucwr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3iyjpaoxr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tmabvxgo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fbcxiqjk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3elwvkokq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ocwecihh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kjjxlbnu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nejwpdgv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lqeexebg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3exvvmwju.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3lfxwgmfd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhnhlafz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlszrwog.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezaissjc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3haqrodwh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3smvzdgxd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3gqysznhu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xiarntpg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xvjxfwjp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dkqqsqes.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzeqbqwh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzkjcmud.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vidqptru.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3weemmjtg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cdnvftmp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3orpxcegd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tvebwftn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3vonsbkod.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3utraqfqa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lehmysay.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ioklxsrx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pfpselfm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3opwbityl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3crmivqmn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3uptizhnm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tafgddhi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3efpukaho.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ukxbpcne.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zkcgleol.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3aazuqnnr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3morzedwv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccgtzmok.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mlghmnnh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mwcbvtvv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3iaznxrgq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hsrcsfrk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3islboali.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3nvckzdpk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3rhvoqssj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3yvmeuhkm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3pjkgyxrg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3pdqwhpqe.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3fvmvgjyk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iiivqhyq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3rhmarxgj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dbqpzddr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3byigwyja.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dbrnukqw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ierynfrt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3mhtbsxuz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zsbhalea.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3oxyixkdv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3aoaptapk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kolljcoy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jrhfijis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylhdkjjx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ejsjqgvr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cgofvbhp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wezuaxzh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mpqmutgw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpytddhr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jugmwyik.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qsqaxbvi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ykbtxejt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnhdfwmd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3njthghzc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3pgfscwpu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3weemldop.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjbgersq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jdxseuay.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oxkehdig.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zgvvnfqe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ahstaxxf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zizgewbm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mcducisi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3thmhnsab.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3chhjjbuw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ogovfqjo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3swnqlfkw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lfovidei.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3djoutjrr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3tadykysb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jpwihwjm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3efuonorf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3gbgbpgue.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bamqihnm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qkcedgsg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ouwtsixn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qvgdhqut.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3kogvqcil.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wwjrsqvy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lwdbxlpf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jwaegopk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3bcfjrjfp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3fdqfxvnr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dwzcgbhl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3phkuctxv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahtgccih.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3owjqbhwa.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ivkdltri.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ubcgjdeb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ltysmuwz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3nvrsmwbk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qjwivaaa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dnnmtckq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fwflnmmh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3srpdoflu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3goalegaq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3yntrlqdj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3csiyyzkz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ipcpnmgz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3opxufbsv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3eczlltgl.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ucztaoha.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3btfeklck.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3pyznbtaz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3zsnrvuht.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3xsrwopca.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3akvwmmnz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3omvpbhmq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3fykckjxd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3dbiizlea.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ppxkyvlu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hhjowjdh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3lqatjzal.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3xqnavrwq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3kftzdmez.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3kdqkdghe.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3gcgwnumv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3wxzarovt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ngxmqjzp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3uaxxlwbo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ztwelcoc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3jttkicka.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3rknsudsj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3akovmxxo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3oeunwprf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3gxcpgecs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ualkkzwu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3owfglecq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pjwcsblm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3chtjmmfz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3efhlvluy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jowqbvze.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3iuqavbcb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tzdnaurh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwbfscam.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3gckaxihl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxqywboo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3hrrkhoak.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3atpqkkwp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fupkronm.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rynorbin.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3piovldas.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3jnrltzdz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3aqggnddh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pnymnrls.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ryykkxxt.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rvbrucsz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3goulmsrk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ncoodkku.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3xtoqwpob.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3phwyfuqn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3nkcnsoph.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3sodvdlhg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3eipudekl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rqyrwrmm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3tabvrgvb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3xedprcig.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yugedegb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3qdqwscdh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3tawtxafc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ygyjgxbo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3dbauxwni.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jrzxdrem.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3fwnxunxo.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pakrknle.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ifnlvpjb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kdpthngh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tuyszowi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wcjdfzcz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3jptcagme.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ewwixwrq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3gtpvicvi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ypdtkgcl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3qhdyjysv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rjbakldj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ayckderl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3izqivwrn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zdyxwcgs.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3sloxrjvp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hziewgiu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fxduckjp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hsxkbdcq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3gzydjhtk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ozuweibp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3sghlbagy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3bezjynqh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3fuihpfhl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bexoutjc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3eeaakcwt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ipyafugp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3fnodwbzf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3xmcagevq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3khhmvxxt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3jesphpgu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3fjrkzzfc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3gzlhewxi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3rvtfowac.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3vgonhoop.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3xgmatvbf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3yikafmby.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3vbxraqcq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3hxahmhsz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ambxgymi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3waqhsccx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rziiynlz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ojqrbunl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3bzjvyhxi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3wpckafod.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3yrvrvfve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olttctgx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3rownzezw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajcmqcjs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3uytdpnto.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ctousdhc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3gjtqvgea.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3qamgsitc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rflgfidu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ggsuqalc.html


<!-- 参考信息 -->