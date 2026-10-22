代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjyuciys.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyaxjpfu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiqaqpsr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lnjjftvn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jxduxbcd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qibxqblc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2etexlray.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vnorpxpk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2pthtqruo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ekfnrart.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbgzpfgk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsyvjgll.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2shfacjqx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2yceqpolk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2klluwohp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xiokprru.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dlklnwbj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2uysbsysr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ekbxdoza.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tplmvsxx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2feefthil.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsegwgxs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2lplqvdcl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xdmcyzmk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rxmpjjjh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2srnhbxbt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zwiuadfs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zqwkekrj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iisdrmtd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yzjkvdhy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xdoymnls.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2wmkujnad.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ezxrzbwu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nquwxvxr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xbktolqn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bkaspxjj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ernvykbb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnjyoxcp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2powbehqu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ddofmpkz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jwmrxpmy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wbtbmnar.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nxjbewiq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2iluvwwqa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2seyjqkdz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gnzxzlvh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vahgzbqa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2iggbdgiz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dojjtcjn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2puaxtwvo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qkholzis.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqmmwxlq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wslkqrrw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xtexptdo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bgbmanut.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qplytsjd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tpgjoijj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2khnogxoh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qwrrtgdt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2anbbqgqm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gqdemlen.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2igewhvqh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2buksxlwt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vezowbxt.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ewngeajk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zftajcha.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gogjbeav.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tccyphbp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hybtimhu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gbxqjgln.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oylhzjzi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aydemvwk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfgwrhwe.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aspgaxin.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mfuipyeh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gltnabnh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2voxbsrvg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rbsdqquq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jamgaypk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2bjxckjcl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hdgeiaax.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2irppskwx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dlumsory.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rsqnvjie.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ltblfcrj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2vifvnbsx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fuxhbnla.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qaosbgze.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2joqeoiiz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qmzpijlg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2sbdijbdp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ffjddntk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ukewzhsg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gxioqlzc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lkzgjzns.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2pimwhbwq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2hzcwrypg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kqjrctnr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2cxqvxizh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycladaed.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2tqnbfeji.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cpwiogcx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kyuellwp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2saylltbd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qrqntyfz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qgdxagiv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2jrljfbwj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2solrgqvm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nuhmockq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2avbdijtm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vuuyyraa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zqgocywy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rmeqifjv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dfovkzic.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gemxpvmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tirhcrcn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kffrldew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aicqcase.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tsonvlha.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pspoqcja.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2stcckaeg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bgzwwhes.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cwcrzyhr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ycbcfovy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2srodnhem.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gesexyzs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gjvzafau.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ehqdfroq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pfwvexwo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mslnfloi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxvdnitq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mckldkjo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwztwsve.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ijdaodqf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2vaaeyyzt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cwtjunpl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lfldwgpk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2maomipdr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cukafele.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fdojdfmc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2apizftar.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lcjrswtu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ktpwliup.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2nzpaojhl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nyzdrkkf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2cvwamudt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lzpkaicb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmbjdagd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cdjolqct.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgscuqzs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpcmbuvt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jofiulsu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2nywbyoqc.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ciyyblri.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2plkervmp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kfqkoyyi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xbxbfvpx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azbnttne.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mvoaigxo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2crhjdouj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2imluvnvg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2fzsnjatb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2getduuxz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ivjcksly.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2wmkxnjps.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dqyafxbc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lixgxumg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xyjcqkhs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2nxhuiqen.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2fqwtwntp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2uqjsgmdj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gwqnkmms.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2dsydmbsq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2yhzqjjmj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xziklybx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ssxvtygh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wdqtjmlv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2cdwthdag.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2gthxsyyd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wlxfbscg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mzelkjbg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2gjwnhvty.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2plipwbet.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2knsgaotv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2eriudmac.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2abddfzzp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2rkokoerd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2gaxxjnpf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2kluvumgc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2lnhtvggu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hsknvsdc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2qqfdnzpv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fzsrwefk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2kjyqwdce.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2yqyezgxg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkasvxab.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2vmsdqqyz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jngqrtgw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2yqveyrxq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ymdtcymu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2rgmynidu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gmfmxkqc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hcvtgbsw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hucmwogc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2dcubnhaz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2yptfqolq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2dhotosih.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tygqqnxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krtxfhlo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qfnkhfqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jutwcztk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2qarrrapf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2omzapodc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ulobauxw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2anfgfdmc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ewlschsr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2sgmbbnxn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2qfomtraw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2lzlxxezq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vgxvhlvg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ezmesypp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wifgcxwx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2uebdlvqc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ouytpqqy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ahtjfsfr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2srixkges.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ppqqwhzq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2itxcygny.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jmlzrjft.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2sogwzlmo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2jxixygce.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aduqnfkl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2cjvipntj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2muhubein.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2belttbal.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2cokztpxx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mahhcuaj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2qnehtnnr.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vjgnqezn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2xffsmhml.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qixvphqg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2uppsjnol.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2egkkblqw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vehoisdn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2eotsgeql.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2updbgjtr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ilgnmzuu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fwlqkdha.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2futiabcn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sptxvgsp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tmyspxfb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pcjrppqm.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2dbxftttj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipniwozn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zphgjjfx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2nnstzesr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2gidyvokh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2lqdeckrk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2mjdcvbgb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2pgdjzngw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2sfhmbghz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2shvwzxqj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2nmfacpur.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2gbizsdiy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pojijnzb.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2wuxirhyn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ontgddbh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2bfjulxxe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2hbaecrxv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2mrqrewmw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2cjmvfayz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ylkqzliv.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2iqhjvzpi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2fvfosgen.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2krfoppjc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2zveffomy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nefsxdqd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2twfldrkg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2olptovgj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2obfahbcu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2swqqzzvb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2rkzcstdq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uyhzodxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgxomgvd.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2qxhsrboj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykcamesk.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2jflpcqku.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2bixrtuwi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jouiewax.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gadrqnqc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cboflkdj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2khvmsndf.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2myfvpnel.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2qupbdvzl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2eiuuqueb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gjabzuag.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2nabksjgm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2icciozay.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2lzhhqsxb.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2mzluphxt.html


<!-- 参考信息 -->