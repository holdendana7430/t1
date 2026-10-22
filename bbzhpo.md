代发 wailian999

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dvgwdjnq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tevmtxhz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2egfjrazo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xnzehort.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2binipmii.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ylaxdhfr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dtlhoucv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cqzsaxjn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bmdyxotx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eyytwihk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2acfqrnda.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wijocoga.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ffrxzebn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2btsxelay.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bwfvmkin.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jhuchyfn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xvplxpnk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuviapch.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcbpumim.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2siugkxom.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2prqaawmi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zmukdvjz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fcooytvy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wcpcmjys.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tbbtdnhw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gbymyyog.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cgvjbhol.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kblsfoza.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkjxrpgy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jrzinigk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2asjxihng.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fjsfgvdo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2plylxwhu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wdoquowx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2vwgmajfd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zahhkucp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lyvrpurl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aatxkoaz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gphafmbw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2iwgpvyqa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dabrtsnw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gohzhxjn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hflidpkx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bkegmcne.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lplwqydv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kclrpwdh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzezgeeq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsvkztvq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2szftiueh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zgrgadts.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2drxmtkno.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2tvpkvvyi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lspkdazr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vyuljugj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2orxdrpch.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gfeltvry.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2iqnwinhn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2mutvskrk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pappoadr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dryfuubf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jfgixcbi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nhbbakng.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cnwdujvx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qlqoppst.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cwjzyxjj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2sevmhndt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nqxexebk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pztixqdk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zlmeylec.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2cwwafqgz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nzjjwomu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wnsledlc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrpbtehb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2panxaoxi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2augtnpyj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mxcruxqr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ukyaloui.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2typgzcug.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yzzyjgii.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jvqqfpko.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eluubwtj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvzmlkfw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dgagatzr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ptpkhexj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lwtpxtqm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xlyaeqvj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xaskhxxv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2iwxowqry.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2lwugerhu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ezecvzwy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xrlsplgl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xdzviwda.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nyiyngen.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bdeinjng.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rgbdheia.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lkvewgar.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xpsahmlz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xyobgqwb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2iwylkzmf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yjsusufy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2iplyxzrj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wojpqhdo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2lrjrwztw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2twohtpos.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2qdsjcjbz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nqvvupko.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2atzdoswb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcqupbdi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ggvjjhde.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nsqytykn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lkmqrmcc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2urbjiiom.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dezqrbhy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lwxbamwn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nnhfcizm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ppjerkjm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nxgevzld.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2elgcklvt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wukdidtg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2nrphhzpu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2dfkkcnww.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lauprrvu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zbcoewwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgmdrxvn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ckdkfhez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpnmcagz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2iuauqnnl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fcqfmunt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2djnqqkxy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcbqoyrw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrokbnio.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkntkamo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ikrwyusz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2mdznwmuu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2sosbrogn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hdngjclq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ngkrzvsr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzbrzuix.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dantrzhf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejwzmvrt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vfrtfrbr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pzekveux.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2rxfvmlkh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rlnsdjsg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tlwaawiu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zmgxexta.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dqeaocqv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ndwyfrbr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ascrtgbt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2licgbtks.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2eqhygxjn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jfxeohix.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nswtxomj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2yhfycmau.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2upfgaugk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqthuhqy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rdhhlwcb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cmvzztuh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hjwahhbm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bwrmkvef.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2biuytbkb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhgrimei.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2pwcqjrep.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qzdjhewq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2acqdcfgg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2czikemjm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvupgbvc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2cqlnpsxi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hflvqkih.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jxjdkmkh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cmkbzyew.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2gfgrhxiu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ibzhxebl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2htmvweyp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uudihugp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2owtovuph.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2pqrboakb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ujebilwn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2gplkovnv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vywvkvvj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2eotvegjg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2vwviecsq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xaqwvnrj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nvduztmm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ewzucovy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2guoujatt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vvchgado.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2bjegzgwr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pisygyod.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2cfvzakcp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2cljhrnqg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2kzhykmmb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2qkeaahut.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2iqktazfq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2rfnvweot.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2vngzspyg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2spevrogb.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2rppzcbdi.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2pgidjbqj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2swyhxoyy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lgsyvdhw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ledkuele.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2afvzdnbj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2niepfecv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hhcmixsm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2srgihlon.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2rxtdeslo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2thloienk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2batysimi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ukkyukbk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ounwpejw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2eluktvde.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2rsvrqked.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2asfuhler.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2rborajjt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yjnamrea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nckjtemn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mtcdvswf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkwxvryp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2apxbcwew.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bzqicduw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qvdqmpnq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zbzuregu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2bhjpekkn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2bfldzzdw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jmdghoaa.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2juemrzfs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qlgcgwdo.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2tlpistoe.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tsdfckcj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2znudqssl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2dzynmepe.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2iyrgxumb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ludrrnkj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewsvihql.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vgwgavfy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vecqeyta.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2jjtmlnzy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdrtnawm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vuiinsxj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2zymyduaz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2jobwbebq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2nhemwxki.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2webjxoxk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xpmyhjdp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2sovwlmgv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2onifcped.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2acwcafni.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bvmoovul.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lqpljpzu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ckyxyepl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2tpgsevqo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2cjvkcwgi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2binxmclx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2njzqfvaf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2knuxwvnb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2siogyuah.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2odjcvtwo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hfybqrle.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hibftvvw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2njzokkvo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2epahbqzn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2terxubvf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2dumxtknq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2hmtovnrc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bnyhcuib.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2kcsrjoej.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2dfvyhbhi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2gknreijs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zkfysopi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ztabgpuv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ecfhpbfc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2puycmiib.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ruhdvpwf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2gydjzrar.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vgbiulzs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ipmstsep.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2wukgqbam.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2pnbeqprc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2txbfxawk.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ywyqceyd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ardefkau.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eonfyoyw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2lykklcls.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2krmiuoro.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ifidkbbv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2lqtrwlux.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vvmesuqj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2umzfewke.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2filmlosi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rpefgyup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yeuzbasb.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ujkcecoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kixvcvwr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pbhvdyxi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2nhfkvdvo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ochghxdr.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2uztddipa.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dbbnbyje.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2zqfathml.html


<!-- 参考信息 -->