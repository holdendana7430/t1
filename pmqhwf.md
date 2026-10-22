代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lvimglul.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fsczazyp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rgamfvee.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kiixjgip.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qmluysoz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2frpzppuu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fwazejrt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2twnwwpyc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lodgkhzd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zyzaxljg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtibmwjb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lbfirwhu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kjkabhjp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vcdpwxii.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jvxgorch.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2lkqupgut.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zyywvojm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2awfhyiza.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2syvgmnuv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2djciuycg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qxukdfxl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ylhuehli.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pdgdkikt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2yqvykuoy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xeqpdnzn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2jxcoihxv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nttrvrym.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulqlcpct.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2omlrecbj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2feoqmtog.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2yrmpkome.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2cghaakvg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xhmcselg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ynsnggxv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2lnqftmlx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2izeievcs.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2djciafsz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xwutmyag.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wsuumydc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2opnnmkza.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2nqhfkjpf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2irkztqdr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ozkqimck.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2outablni.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzigixfz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bosefdkt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlnbfvti.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qvouhkfv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ipbyzmln.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kkebawol.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdbjqgev.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2abvtpesx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2spaaanxg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkvytgat.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2htbefkgj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2dejoncqo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vtsphlts.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2fsiappgj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yrznvofo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ftseecli.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qmzwjloj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2duumuaht.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jftdmzdd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vydabnxd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2losjywzb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2aybukmmd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ngpptden.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xxrluufw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ggmpclax.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dvrqtumu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ecjdlzvx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbxissue.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rrxafmlc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtkddxws.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fllgleud.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nsvvnbjy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2emwxisxg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2clnctlik.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cylgjwqt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wwnerhou.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtdshkae.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgahuawy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqfntwer.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nyciygkm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2weghnstq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bkepeebp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mwlbzujo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fyfrvndl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2xeoqfszo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2slkvigxf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qmjvttcd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cghbglco.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zhnqpiay.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qzjlulqq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2swcnoyvp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uwzhvtuo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2aazetfua.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2shyxclfm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2cyywwvgm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2dncewzre.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2nmaxnzxy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmofekxp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2horpuriu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2kuwqbmcu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2tgoulmft.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qrmbadtb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2alqkrxuc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fthfmvcv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2njgnwjbs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2svmxoutz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2nsdzhgdb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dibxgmzx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ktdknoxu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aadhpirt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ehyhykux.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bjlkwkov.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2cyoogrkw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wcekljvs.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cbpoasqa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2unebmnyc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2pcnnwyhk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xhwtjjej.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dxptbsys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdegmdei.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2otwlxoxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkvtgwvd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2iwpomjed.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2oxxrdspn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcauwmaa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojinsrxo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wzvlfdvf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cohecspf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gxrxkdsz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2pdbtmlcu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzfxwuvh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dskpjnog.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2txrygcwl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxcilqrb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2epyvkynv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xcjuynim.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxkxbliy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dieghkgx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2lgpghaav.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2udibnofb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hbdeucji.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ffecpypd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mncnutll.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lzjpnkzl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fvxsjlql.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oorplvqc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mjstzsxt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2sqmuplgv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lawrrjqq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2sgqmuhke.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2oprorqjk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmnivyce.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkdphpwx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwtpnhde.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cruiejzu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2hijjbstj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2egxrmjfe.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qbyzgbfl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qarthtcg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ymregako.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2fpxlcini.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aaluhfst.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhfrehdl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2hilhishk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2jnidktyr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2cfmnivlt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2jcjebuux.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2qgnrfqro.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2etyqdxew.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xedfipyv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qvpmvhcg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ahksauia.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2iykkzcay.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ircetxrq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ppnuviou.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vcumhehs.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2faxvmzry.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ikxsdluq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dziqnxuf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nqwrlxas.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ftnhccrk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2imwqjpjp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2yoxlwdzs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2pztgkbaq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jclcgupi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2szlthuvd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2gccvksuv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ezsfitfb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2akhsbzzn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fodrvrka.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ipdmqxwq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2wfvxxyzw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2itilbseu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2unapahhq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2fpvgjsqr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2edbqgrcl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mbvwhnmm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2hfzjjgkd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2frrektgi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcqjrpgx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ziivuukm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2joorvfwu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qybowxcf.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2qbqcmmmj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2zfnxjppg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zqbtnhuo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zprpwiyn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jxwqpaag.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2dqgpdqkk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ikrccgtn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bivqsywi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hsfiwoug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndhnodua.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kuiualpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zahaibbr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ukvtlkef.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tagpxskk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gsqwufji.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xlzdickb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tiwfnigf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2xukmyhsz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2xycisvso.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2kgycgytc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kwdffrfc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qnjyekon.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nnnqppyd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2xolpkyxt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2cxglcfpb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2akncxixz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2wuwerird.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vkqicawg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pwsgohpl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tgcboict.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2gondxdtx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2mpjdxwie.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ydfxcegw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wvnnlaws.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2giqrgseo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wwcimqoa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2lxzqaqfd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2sxsjsrhz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jbpycbwf.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wcliydic.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2daajfxka.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fwpcmfbr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qudarjqv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2klyioiue.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uzxohpuf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2exdkinwt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2eeckpsvy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wijqrfdo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2aqkzoezp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gjqkkqjr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tyffrydm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2elbakyko.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pumsxjxq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2hxurqigz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnrtfejz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2byvgtqqj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2grnuazqb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2xwxxcxqy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2llzclktj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2bftzrtty.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ztygqywk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ctnojfdq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rqghuwjd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2gzzgoasy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2kxsdqwqv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2eiezmzmu.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2vintavbj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2cjychfmf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xxjwkbep.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2zydcalhg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2djlayiyb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2rezcjalw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2syivgnhq.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2frpzrywd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2fslvaxvo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fkrmnywq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2wxrktdso.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lzdtfqcn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2emvfohbj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ntyhvcdk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vamqhfkc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2mrwebhki.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2uxgnbrak.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zfarjtyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhdkcjiv.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2gityrwmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywxeuomm.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hobirqbk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2xbyslnnl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2piddhekw.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2minhhkef.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rjuvhxvh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wqrszfoo.html


<!-- 参考信息 -->