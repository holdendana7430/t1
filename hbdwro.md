代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qgvjljyf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wbtkpeaf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yfyvvnrt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xmgvlbhq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mkihaiym.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cjiyljkl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gskhrijs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3nworixwb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vkuznryo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3prwkpold.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3sxzpuqjy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hmvgnjev.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yucyijat.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3owdvnppu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vulcdega.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ztiwwwqr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3owopexpq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ryvbqnov.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ohrrvdhe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rjblufiz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fhqgalhk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jjgaengk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nijctogd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddzxofwe.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvkhcipn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kqpsgdni.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3myumthhr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uaoqtobo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nmrjmvbj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tyetmcbu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xrxhcczp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwrdrucy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jbjjzwln.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlwmdvnd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gcvhpuom.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qqluwerg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tbebivah.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uwhhfqle.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xqsqxoad.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tedrdhrp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3asarskvk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pfkqekrv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zhciqctr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3dslvpkzc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3qficvsqa.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3aghvbtyx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3llrcgzrr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yyvytvad.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3drwigvva.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qfsuxhke.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3uflmzutq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lwzudmqg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3kobkjmou.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qxwelasg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbxogzlc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3sshnhwig.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ujimanja.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3njzrfpnv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ttziwjty.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3amktaegy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ritwdstt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nvomrfzz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3yfmhouiw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3jmerzogx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rbmjptqt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3braxgkpp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3znqfovaw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3opvucnhs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hkwcbluy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qctillmk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ojipmpas.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hqufelid.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3djrncrmk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xwcxuspm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nhsupszj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3flbgijxl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dluynbgj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jmxwpwhf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bwcchuak.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3apnoilzb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3kuwcnupp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3imrkwyng.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3njfenlis.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ezzevrev.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yqflyvzc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cprkimlk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3selnhaey.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cwhorkpb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3onxebkvs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jfyuyplj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qucicpgk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3eyaszvql.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fkyrsioz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xqmzcheb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ywkwvtmf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xypzldbo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3omudjcaj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tdfmjbgr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3zxqurdat.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fajlnnau.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3lwqqpdlb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3pckwaxen.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ueslhgon.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3dccverzp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3esvzslgd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3smfoahyg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xjighquu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3aucrtyek.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3muthszjp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tdvdeahf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3prprnkfq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ehznrquj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3llntslzq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cilosxmm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3dyytwyec.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3oiqtodfe.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3akbrqolu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kvdurzrp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hxtehfeq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3slliywwh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3boqaakyh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3spvjiopl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xpdlrmso.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3uvdjrrnc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jdhztmng.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3merkfmro.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kmvesivs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmhlbgho.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kbzajdsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcuvhxjk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ekrjjwvi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hhjvvvcc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3avigghap.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xteesyfr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xatparld.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3teepvqvg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3aopwrbrg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3uzvybnab.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vylpgoij.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zycigaep.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wqjvmvtw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbejkczf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xarbdfec.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3npjuvuxi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jxlwyaot.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3clswuert.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dexkcouh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpdglgyu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3thnhcanq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3edpttssj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xfzriowq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nsjtuahu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pnabzuuy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3owbjvmsh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3oocewuwx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qmqpaftp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rdgqqsxn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bpgycivq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hphyidla.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqzvotko.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqxweaon.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctojqaqu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3anrsxaxc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3fshncmgg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3wlsptlke.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hmnhzyzw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ezafaodm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3vqddxatu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3zepayyig.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mlvwgund.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sosmkstg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyjqiwww.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3rdgbptqx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3yqvbtstg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhzmzeak.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pvumarzl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3plkrnqjp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yxosyncf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fxedbgbt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3eazlavqz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mdkijjbq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hqmtpdfx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3vmhjkwzy.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3njabuyho.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3adnconhf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3uqejxnda.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3frjhcjcn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ggzsxeze.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ihpijncp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3fwwwlpmt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pndrhokp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3hxhqjqcr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vuyatyhm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kdusjxmw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3fqceubkz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3negrgehq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3jdfhvawe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3itabzhno.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3yupytmnw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rjjwople.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3fdhepjwp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3hotkgnpt.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3fnuzkkgf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3worwgbgx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3doypdfhz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3rfrduazc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3fphunqfh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilquiygb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ozjqmimu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3txgbcleb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3gvgajzcj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3kvhckdnx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fzngoocz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3zmrnvaxu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3erigdsvm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3oadaoroh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3cqaisynq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3htnehgxw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3tkkavqgg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3twcrffix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twfsemzu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3smttmacf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwmwiquu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3wjhpdtpw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3stvyyemy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qhnllhgu.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3yfjmauia.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gcgkhppe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ejrnbplz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltebmpsv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lrgcizlk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cwdtbujv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3axfiuihn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lugcaekw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wwzroezh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3hnqqiyxx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3biqqdrjk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lyhptypw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkzhoiyw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hcnihkqc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3funjlgqt.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3dqufgqyb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyknlwol.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3duifdpjq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ggydcqmv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3byjbqume.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3gfzehezi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3dfpjoyud.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rftjfdxc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3yolddsgn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vwfkmwlk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ylhbfrul.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3idfqbtec.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jiyshcab.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nilvxbqu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ncgfejry.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3kmlhcvch.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3fivyiska.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nrxeszbk.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yqlfjvyf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxkuswy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kjfqnfaf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3yuhjuzyj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dgrhvdic.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3cnkohjes.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3irnzivmn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kgvwelet.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3qrabijvr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3uwnkklqd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rgqfxxww.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3efmjksha.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ikuavqux.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3pmwrfgyd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sjnaxecb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3lcmqkukt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3itmnidld.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rmlgsmgn.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3mjuglnbk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3gecsijxs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3rmpbtfhj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3aifvwsfb.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3iexsjcwv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3bqifzuvf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3bgbqydcp.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3gfvmdugx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3zphlfnhx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3zrljtsrl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3aurijipi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3fnnxnrsy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zaqxhfhu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gqusbvee.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3mfjszzam.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3nwbulojn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3mxgnbpst.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3sqkxuqgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znbxwhgp.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ycuvzipq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwaisgmg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3eneahlpm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3riyvitpz.html


<!-- 参考信息 -->