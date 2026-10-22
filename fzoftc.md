代发 wailian999

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2maszcpan.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2svfrfjgh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2imuvbwms.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hueenvep.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zgancftp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuyaaich.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yuvdwxgw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xajbzbnw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oqjmtkzp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oobnhtgh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pztybnqg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2eeaxbtyf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2uzyxudkq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ulbkzabs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntnksrib.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hqhkfzdr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pxbvwrux.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2iwiomwuf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wiyxjpcj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qfrkygqo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ufpncsvw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2symsgndr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujsrtiek.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xuazllev.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpcvfxhk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugcvtgpa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2wwaudjcl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gljdlldf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2yymkwbfi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ppqixbhi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gookkptp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2znjjioba.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ihschsni.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xlgwroaa.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2esscreno.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zovwwbol.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gjwcjyig.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nfbiaaml.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fcoareev.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cxictrpw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfvcoeco.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjqarfqb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2fasnbmnw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrsmdbxd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2chjpjesg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kfxvkuih.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpdhjlxe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2gzuysdmv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qgwpcybe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2skqnhpon.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gatwvemc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrdsgmlq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2olhdnyzm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2srufmmen.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2dmekynwq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ilwodwak.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2payjcoek.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2btvtdcgm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dflaiqzi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2vswwunkw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jmqyhszj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zeolmlge.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ahqeaskf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hpyhngrp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2exzgqaqx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2loitxift.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dduapxee.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wtpiaiuv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iygnvpcs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyuxbtle.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhzzqkox.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2isdolfio.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wbveehdz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ovjngtry.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wrhodgus.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ashakkfp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iljydvqa.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkbhfqtd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uczkeicl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2abwwwucc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2geulquuc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vymwzkul.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2empkntpv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dvqxxsld.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rqkgerhh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lvmuzxze.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2izplscwi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kryprobn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cucswuvh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2amcbnigx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2thjbygix.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gbsgyaxk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fddelqgn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tzzdrxok.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2sgbuemmc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zfcrtgyp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ngnculyb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tndnqvur.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gscluyga.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zsgpbcqd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2mpkjnnsv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ydbaakmx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ftdeivpt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrosopkq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2yryiqbmn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qsnqpijp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qzwcpyig.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gtmyyiue.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2uwidqqtf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhjgqfad.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2fbbqodjw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2riyekegn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2dxydpkia.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pkptovsc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lkyttwxb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xjbnxdjq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ovhvtjkb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gyyfqezk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wanixcrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vptgsmbh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ibeiqjio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyqqxvzj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2sbdctgzt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2byysaoyp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2kursxggt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cxoawcde.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jnoxjcgh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrxzogmn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zeabdvtk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bzfsmbdy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtbxjwlu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2pmdsoifl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cspvpcpe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hixvpjjz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dhqhshng.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivlunsag.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2smmzhoyd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2lcmbdewv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2rjnbunrn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2toshvxip.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2owzozgrz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ibmatyuh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zniqirbo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2glimzwbd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2waokgksd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xkfeyeug.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2azkuhzuo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tdhjnahe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wmxrflgp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2psmiqeef.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ovyjvkaz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zxlsjapj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivzhlegk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qsoexpss.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gffakehr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2qyikdtpg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2yfmmycim.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2bwgzgsbj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2zjozfbkb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2daiygddb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jraytbst.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzrtildx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvkhfsel.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2chzbmpyq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qolphtxz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2aypelpyo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ipreaudu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tlbvkwvb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xkbnbmzu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2festjezi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vqmoevtw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2clarrkmq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2krhgmhyy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2aloxgikr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2dpuuftxz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2bufokdjq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2aetetlwu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2uzrezpmj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ndiimqqz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2efykzrtf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rnkypxmh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2dmjyfiqm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hhmgfent.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fookrpnp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ljggnnxp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2usedoznj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2olxzogwo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2kvhtympt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2zzufzfyc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2lpnwgxmw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2cpxzsqfj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2hccnrfgg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ueczlojd.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2najnioiq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2zktnkvhq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2eqnmgkfl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2etwfyjch.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2yzesupzq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2farihayy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndtbadbj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wbblewoo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2hzghhklg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ebseuuim.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2wkfdipvr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2thgpunfm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kclyvrcy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rqzyrtql.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wztykrzx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2kikyvzbv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2qqrxmqsy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2xskedksm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wuzqdxcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhuofaof.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2lvhlgaoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abuhmeew.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sglvtleh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2jcjemekk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nydqnxzv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tngqkwdv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2uasqktsv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2bbhwlyda.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2psxgmywl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2qgabhnvy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zmyzpxka.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2unrbyjzx.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yzwocvzr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mbtwdfsm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2smxkeorl.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2tgumygzt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ysnuvymy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xghzfinf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2qjqrvxjt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dbitrlcz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2miajomhh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yoplpgdi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bsnqyrwc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ndpdwctx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jeaajbem.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rzzfpfne.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2hcdcrgci.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ynfgviom.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2uvpdarvo.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gciqqesz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2lvngmtgo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zuqibgez.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gqqyavnn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2acenxgbc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2aycsxwhy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tceqgxto.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uxghghuc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jzmbbugx.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2iusoxzqm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqrvfrk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ciqdwavl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hivhnqhh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uunbfznv.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2qlbbflpr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2qkrhgfrl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jumjvwia.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2wfvyfvhj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2txqhhliq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2nbdikenx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2xwiohstw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zawolzao.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2onrutjra.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2uaqusjkk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2gedlieyk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2megkcwfh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2axofqivq.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2sezkgvjz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ttqxmqry.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2frpscgft.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2godmfnyo.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2hbzzavim.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2uoqguxkq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2tvgqiydt.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2mpzywncz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2aotimhat.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ugmmlxzi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2hnumhdpp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mfbcqcjv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zpuzteua.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qesfjjli.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2maczeprf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2qzsfuoua.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2gctsldxq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2dyktdwuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eramtsyu.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2zqxcvsja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hspvqapq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2htedrdmr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2mbbepuld.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vlhgnoaz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qrnjczmb.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ikkffneh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2nkmtnfjk.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2maewcros.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2bpksgibu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2bmyikyyq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bqngjoxy.html


<!-- 参考信息 -->