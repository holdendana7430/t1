代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wwtiohyh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bmiggkhk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ifevljka.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hszaymab.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nmbshdxd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lwpnishx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2qriuspmk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kqcntxmy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfvrkqsp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmhyruzl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2agjtsrdr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2usshsepz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wkrcgrcg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tmeqmdmu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ngvtnlak.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xnsiuqzy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qeodluxx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dlmiulyv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qgfzyapg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2raibysyf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2euauntcy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2omixunkg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lempaswy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqafutjj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mwaohyoq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2texxkjaq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zymyoacr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmjywqsj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vlhxtwyk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pdmfyyyt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bccwtand.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2nntskhlf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2yogaxupt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rbtrpatz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2unkkeths.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2stfanohk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yopogbrq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2acxgqleh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ibnlzcbg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cntracqp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qqzpeock.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tbqqnccg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vbozpmzm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hityennl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lmadsxdl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2eluistbr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dpvsmneh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2babgyhaf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ctpivgyt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbcswnup.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fokyglov.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jgpkbbub.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2cnlqikth.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zfcfjthd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ehqqkzss.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2toysyrfi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vzbecqnr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nsphglfo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2melumnfx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngvefooc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2knhmconf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tpuzjdea.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wvlrtyon.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gjgwhavu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rpofzlvv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2yuhxrbid.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2iozjapeu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pvolanqy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rzctedkv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2iiruenbb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ocnamlmq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agcwdmca.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbtwiovx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkcyvrjo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tmifejxl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vkwcpmwq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xoctdpsw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsgjkicn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gzrgkksf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2izxebgeq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vycvlyfp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vdlbobci.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdhaarlo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bemyqqbt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kcnhuuzu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rilgovsu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vklduklp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2bdmtbqmz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2oqwxpjgc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qsmtxrzu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gquxenzy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ksjetoje.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2udluxyfs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hrvpfszt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2peghilmo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ibwpyxmt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ikvvlhnv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vcdvbkep.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jjafanje.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2didplpwi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2lqkddbxl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dscvoftf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2egpcyazx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xurguaxs.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pjdkmkum.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rrpalifd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xtvditdz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucsmdqns.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jvwgfqkq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ihaadsqn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2cdwirxyz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2fuhtdqbd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ksdrqtii.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yqzihlpf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nmpboxdq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2murgxphh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2unavfqks.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2phfhkpij.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2boygjntn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2lvjchljb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rqkuvmrx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qxeuougn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sufcxnxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrazsxrr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2elevnslk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxznjjqb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tqtfpdky.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hcyxpsic.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2iozbjgru.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2alozmxfn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ugkdjouu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ykaqspnj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zhduzglg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ciqtgqdw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyppdevp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2raylndru.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2lnecwffi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfnlomiw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecxpjyuz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnbuzdzx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2otlxpaqh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2urcxwzhc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2mrzhsvca.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2izjkhqqo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ugbzodip.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2qrvogfca.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kocfpahr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ovbdwuon.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tbamfqgi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2igoorqhk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2wzyjjugj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2letjqjzw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yrzkpexi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2japltnfl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fayiwvin.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xzndjhgm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2pysooivh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2trykoojw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlovotnm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wcmyrsre.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ndvrnblm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2zqjfjmvd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ewvvvqny.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2cdjheenr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ubboqjlt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lazxhaqh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2paauvatp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2sxnnhwop.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wdsswybh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zidedleg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cjlrwmoi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2kfswgvwx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2etdpgojg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qoarcqnq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ivzoapem.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zletfkez.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2isilfzkm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2pxfjapyv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xkwiijsi.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2upytzsyf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2iwpxihkw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2wruixohq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vcbqiahf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wwuswhjp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lxwifjwa.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2wggeqwcd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2smagjgys.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2owxvvinv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2orykqqwk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2undmyyuz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ubnrjcrx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2byedbsft.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2efaxbyhy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2aqjultfq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2njscrrcr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ydcarcbx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2luqmuvgw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2yhyjoyrl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2nraohksq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2uwovvbfz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2zaqyhcby.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2czxplyul.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2oogcudqv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vgnasddz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ujyfzrik.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ogvjoxuv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2sqawchsf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2cnwudorb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qgmxyqvb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2kndbgceh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zxcmhhvl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2juvzhbzb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2zxhhsqff.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2vjyioxjj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2voesbcpw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sqwvtxqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrnealrz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ravhfkdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yskkhvqk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zknglypm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqntrhkm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hxchjpoe.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qurbadxv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2derytdex.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2xmycrwqh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2clbehgxa.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sgckniqu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kqxqkypu.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ljjrakqy.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvwvsrkg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2zsicznuk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2cqwyzptt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2sxciwvfz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2mdkrmqfu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2flipkszn.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hzrymqjl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hhfgwcak.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2vjywqzpw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2vadchqwv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pjcgyhmj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qnrsfsne.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xqvzmhke.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2fqsdhazg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2mcmsvyep.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2vbxeqmee.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ytoorqii.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2hfquqbgi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwufzoeb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mqakbhqa.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jbxuvxht.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zxyrlkki.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ejfdowhz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2izcljaos.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kqrseyqs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xikbwrxw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2jmtcexmp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2lepwnuol.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hcggtdwp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2sgltvztd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nhqhltky.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jzmgbmpd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2anordokh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mhgvsicf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2tqwyehng.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2bzoirqih.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fjkkrieh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2rjyvyciy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2gpicwibj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yrfrpopo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nazyrsxe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2bgsklpzv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2laeytxsj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2asuwqzrd.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2bjiypgci.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2cpizeyij.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2oefgiypu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2nehpgcxn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ubasyldv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2bstiasjb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2gnuisjdb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2coeqsdde.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2fymyvpwe.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2swcxqdgo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2gpatcnrs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ofhyodqv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mgncalwp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2cmwxdniw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ahyesmel.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2kdwhwwxe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2yqwbbxzi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2tjfsflib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klbojyhr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2srcydofx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfdktcso.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2iodzlopf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2bmrrxmcl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2arsdapwz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2igbxelyk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2antytqup.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dfilhdyx.html


<!-- 参考信息 -->