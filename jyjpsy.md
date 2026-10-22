代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urxwfird.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wksgmttf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2egnfnmze.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntijfwas.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mxmunbum.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jrgfxxht.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vxxamlgg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2aslneodl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pvzhmtzw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihzmnbmr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mipuqwln.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmolkkxb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uatktuyd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mvjwwqpt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fnswvion.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cnaxlstu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2tehvfnph.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gckmidkg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqeftjfb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bbxmctjh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qlzxywqy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lptfekvu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mcwkquea.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2aytmupwr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2cgllrmbk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2yixkkdai.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yaoyfpve.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2wedpzsqp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lbsrkoeg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hjmedelf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dsvhmurj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ribhpyrt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2cvosvcni.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jzeskkxh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dnhtgisv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gurrynkv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ydgegnvw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkslqdra.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkjnmyek.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2knspvdzs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pxlyvqqv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2njkurnjp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2lzfvljxk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2oxvocvoi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ejrztwlf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mqxmsjkw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2cforwnkb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vojznrxw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqztivew.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2sqdoshlj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mktwxalu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2snhwfmrb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2htockekv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2kedxsqqw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hqhgovie.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kiboopqc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jtxrzydd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hriukemp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jjakydre.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yqjozbbe.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pxnuiqzy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lzudxlgi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2fvdyaicg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jpieqmqy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fjenbmbp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fikxfnrl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eywyvvon.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yysbbjhe.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xhzerhno.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqvegdho.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wsftjxrl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ygpuqywh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjjajfgk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kvbarfhj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2boyaekem.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbhrneor.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ottmgmdx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2waezcsob.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wnmaenqx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2uqjulcim.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vhtscizc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lddivcwn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lckuxndv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vitrveug.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ahnzvnos.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hdxsmwqj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gvjlasbg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mtdonisf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wtjbunxn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2edbrfuwh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2didbuavs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2guggnula.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qtbxklne.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2snshqmgg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mittlieo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2oqgowvup.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kebujmnu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vlasiabo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pfuobxfk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2njlvikoh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2cdmsiokk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jqjuitbq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ogrspzza.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2smsoiroo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2uvwbclrj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uuyelrlg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ekiyfjmz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ystehdof.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xugpgwsc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mmhfssrw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pgajsznq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jdvtlzsc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wuuyfqci.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2yllemryx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dsaimoit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kafqchqs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xwqqjuzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xylzwlfq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gswdnjtk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2sxbkddmn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lqduvhix.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2iltrhfft.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzqbiwnn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2palaokhm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2cipaaqvp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2tamjtfkb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsotskhg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2avadmkdw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2adojqbqr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iwrtqayk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bcxuzttu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dvlxjkvh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2scmzckid.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2goicjqkq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fiowvdba.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qlvhdign.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2unglwxea.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tqkakyle.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uovscsqr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mmcjbpsu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kvxyjlsg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bgctsmsc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2rsrqkdyc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2bpbstvoh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eupemwmd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2reaugtzg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hwffihzl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wpeywfzi.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyebhxbj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ezcfbsmf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewgwktem.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vmpybhzz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2jhpqjchk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2zuccaffj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2avuuzcbh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2uupgouob.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xazszpds.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dbbtaohw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yaypsdfr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pgdypjum.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2alvojjlu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2icacwyur.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcjojcda.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zuiodxqw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hrhfzdec.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tvvsornb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wpfbkjeo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vzydaacf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ensyzdzl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ckcgszbf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmxqjlkq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kssneaww.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2vazhwsgq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2zxdmvmce.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cqmuempm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wuonqrxi.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zejizbrj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ymxpmcbj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2bsuxdcsf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2jnkarmdu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2iceunvya.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pugmxwpy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2jtsasjfb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2yajgdsfx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2uomddzzl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qpxlvdii.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2mzfznugc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2hafgdgrg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2wynobjvm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2iwsheqcc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2fwgwpcqx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2gqcazifs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2taudnmoe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2pzvurzbk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2dbpmupfo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2fiqxtkbx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2aamvffjl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2jecteqmn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zoflfuxz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2xsxppzzd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2rcawvljg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2szpjznre.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2pteskxov.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tihhabjp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ebdkcyft.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2gnyvklto.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2gkebmcat.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aieozbnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzffgizf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rgxbbkgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lyjmloiu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rihcspoj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ayvsoyhx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nhwtfimc.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vhsswlyg.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fphjlhwi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2dhkclqjs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2qcrqmtlx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2proomzet.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mpeiiwgi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2wjpovxkk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gimgvzub.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2xuomzuyi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2unutnmim.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2sswjpzmd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tourgseq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ecphowvt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wgfhbtqw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cukldshk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2oyxazryv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2pkkecofh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2trhkdsln.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dwunmvbh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2jtfrgzpe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2gjlrafhr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ozucnllm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2dzjhlfjz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2xcqrvswg.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ocfeixoh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqhtlttf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ddkjnvjm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2aglprdzp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xkgalfnl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xpeddnfz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2queajsna.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yzjnglfw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2iwzrgmyw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2mevofsnu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bceolunc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wainausg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kvjkokoo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2imgwvmpg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2tpxkgwak.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xrtdafko.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qcuueysv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2amfeknmk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ttrafigu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ydoubmda.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2tvbdohem.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2yfublvsz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ngnilsbl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ldvkjuvx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2wiwceodd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2skuijkbz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2tnjthqno.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ezbagvye.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ygofzjwy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wdgkbtxw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2jriioxut.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ltfecxox.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2bibkvnzu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2joykiysq.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ctdqbbyv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2axeimfiq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xvvhxprq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2htsbvsbc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wkgbrlme.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2jvbbkdyu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kfnpttms.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qinawjdi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2xzqofqds.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2weyijusn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2mtniommj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snrfepne.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2xccgjqar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvmgqnnf.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pkdlppqf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2qcazbyfr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2hpztjshd.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2qqcnofot.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ztkwwnsn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zgybytrk.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2eduyxarq.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2rpozhugb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2vpzeuoul.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2obbwspoq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ojckkbnp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2soikhnmz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2mdjneafa.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2qjehwksn.html


<!-- 参考信息 -->