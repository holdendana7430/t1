代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gbkghomf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zncxyjnw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gdexebgx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3afukbuzm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gxapdjgw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jaojdwlr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wecagqnc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tvzaqoxi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fhibkbbj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3otwenkqk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cimyenck.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lcleexng.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3palydgjp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3pxzvylyi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3uogbaxcw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hyjywakk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwnvcyrs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mennduur.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjgbqdpa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qhrdhezy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3acoxyhiw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hrhwnghq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jtnaulsh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3eefqkvsd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ehmvgjrb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eroljcte.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmmqggvq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uegdayne.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wvgnpclt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3txncwktw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xaskoeep.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ovucvdjq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cywldqah.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cnycabqr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gcorrupn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iroaxauz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kirrcoxh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojprstph.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rahaauiz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3oirpjgwf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rnkbyjvm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rnksikhj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zimmhiqj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kieopuvh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3octtkoni.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fljqnimr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3whqwmbzs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3inaxklhq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ongvshpa.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3dnazsebc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3rhcviukr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ddjpjzlf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tkjmhgua.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nfwjnpgb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjyfdqhp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdadlkqt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3pqagszei.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hbrtkcor.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mcphvoos.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ipahgxci.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jyabvxpo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ittfxgvl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3fdcyglbg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvwtbfbt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tciuszjg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wbbtawod.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pgzbihkk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fvazottz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3izuafwkq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ttnczwxn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qvyamdnz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jsktuuiv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yifekqqq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zbyicaao.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bmapibdk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vxljwasi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3onuwlxmv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ftkdbuyu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rsbrpzyj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbvfuwtk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zemunzcl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3aaucaldr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihqayivk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jubklcdb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gageclzk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjbudxga.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tdydssdu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ueemgbsi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhqbrnhv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esazljfo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3elovjoyt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qnxrloua.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ekkayprk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dpmzwqfk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jczgudvk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3svoqqlrt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tbkpaweb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dqlaeobp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ptrbzimf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ubwjrwpt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aenbwhdi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3hggoqhtw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3smmqgzbe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3hlumbblp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3wtjavorg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qeplvcsd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ynpeirdl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ranocnco.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rvzravhd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcfunvar.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hurjktbk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3opucvtuc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3duzgqwzl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vxragzrr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uxrofibg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsygkabb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nzfecxpe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3otebfwbr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3oydjzspd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3pldqspcf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nginvnwi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pddythut.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xokpkbjg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qcebbypf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ocpkdtns.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ykjwrvhy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3voerbwnm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3virrxnyh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rawofahs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zuhqhptb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jfqjbkyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgnjiczz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rrhtdteg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvlqovln.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zgovmllc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jbpzatxa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihzpmovb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ypcgbaax.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttohxnnn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecwgebmc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3urzrbqzr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljgzahwz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3appcfluj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3djjlvdfa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3rblipkdo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xyncwdwg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjpdkjmk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqhbruqo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqijjszp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3oqolbfev.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ymdqgmqp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pphjxfmg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kswkurxf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mapndapp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xtsydden.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qcvrenbp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wulfqqwe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3schgnfyl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zpnnfotl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3tkxxvdfn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lcwjnxmn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3lxwivhfh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dqtaentl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xateqimy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnxxewbg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjnwzlwq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vipumjuk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3imgqzdpl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zdlivooi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3diutigkz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3avawoiyo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mgqjfzou.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3oavhpvrm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rhvcubtt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gwuhyswq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbhmjcku.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3odskmpfk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3hkdggkev.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3atzbvszn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mnnkpewm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3dogiwkft.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dbfakjfz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lastdfbc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ehfenzll.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3kuixhovg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qktdlnjc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lbogancn.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xwbwzlws.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3zpbvvyid.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3pafqkhoa.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3egplpzxi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sfwqkubo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3krufarlm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ckgzdtvi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3icjzpuys.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3zwgqflep.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zlbfutyq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3hvvrchhl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3nyrfuxng.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rnsdiwdz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3wranfxdy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3npumfeid.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3godrebzp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ljboqtng.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3wbghivnn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ujhnqnka.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3cwsiukif.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3lzylyrbp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gofjiahh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3asrbaixd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3yrhbgamo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3sopwcakk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yfnugvmj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xwomohzh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ydrmslen.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3lpgooahs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3nvsjyawb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3izkmrsfo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jdqbauuv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bptukmce.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3vupbpbje.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3fgezwsga.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3jxkqsyrg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qdwvhhvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqvioydn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3dfshughw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvphvjlz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bqsdztoh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehnshgwj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bfycwehx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3giejvpbd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3cavjtejm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3elxfqzps.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ujdlzldr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3slswvufk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xhbwdrvv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lncgflwg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lgkyztjn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3jcjwldoo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3nugrpcfw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3altnjypb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3utvdeiyq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3dsawervy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3paxvlghg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jmeytcjo.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3joexpzth.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3bdrbtquh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3aobvtxfo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zxhwjomo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jnuqaree.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bjkbjrfu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3hzcprzwr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dqydrnkm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3uwpzlooe.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vejsegut.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fpdcngfj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ivlfzwcn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3duyesyxz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3maojupvq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3volrvnkr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yjlncaql.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kktkpudv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3plvgtbxz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3bqanhepf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3vmxmrmrz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ojqehsbf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vrpezdkd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zzrmedvw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3dsozyois.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cwonhzst.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ndrrnecx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3uiltggkj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3bhxuonoz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vfqehhpw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3bwcxumfq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zxxxvvkw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3qwgrlmoi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3thwjdant.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3cshmjqhr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3fhdnzvsa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3foymcijc.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3fvdesrak.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3okxmhcqi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3pdtwldpf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3spyimxsf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3bvwmfrgd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3dzcllecp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3hyobqenr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3xxebrgis.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3aqktbmvu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ywlwxvfw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3dayzssmy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3lmmsehjf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3njodwtfg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xnndarlk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3efmrznoj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3wqkifzvd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3qktzzcad.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3sdnzjbju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nelenzka.html


<!-- 参考信息 -->