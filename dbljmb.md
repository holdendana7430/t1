代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ccwkggri.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3icdagaaz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xnytywnk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mtkatqqh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3eyhcxsnu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ankbzpxi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sucyndwi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lgjwmhch.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwxvnmds.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3qciunhdj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ulnxkykj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3pwankozk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rpzmbgma.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3snkslaqe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynnyobto.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3shxxwngy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zgqrthsu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ijvjzigl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3immxxhja.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3wgygddun.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3bvcwawze.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gsqwxddm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rioaoajz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tzbepnae.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wbsqnrcg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zmrwzoye.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zqhikhua.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fqydbmbl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nduuvtwb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3klbrmepl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qdserszu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zdfjsaal.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtjnlkqo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqznujmr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3txwmlssi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gpawpthi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3twyfzypq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3jlyyyhmj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkrmjdtn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nhxxmsiw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kwqrryrh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3skggcujg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ybtunzcy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsxiptbv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vlcgntxm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kxzyhmcu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ysulgygc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwazodqj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lulctjqf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3aocrkxcj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3htnkztzo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zibwcwbx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hyyfqrrn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tfiejqrh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3gdfsqkdc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uanmcbpd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ezducpiq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yrcbicou.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mcdaocmn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3harfvxfx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtmrddag.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tchahlxp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uvtdzgjm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ygnmsegk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3yrgwckeo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3znypnhls.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zppxgmrl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3okvrzdkc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jtkbkahs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnxzvhvy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nfjqvkxl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehqdpsic.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3llivwepa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ibifumdw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xyuvzgsu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mfejkkyg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3rlzndjtp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hlahhatq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rxwwgljb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zsfajspx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jbrrjeff.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3rboqokhf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ayrbsrib.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ashdwupr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3yzftqtjm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3oyuaslzy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gtntiqur.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hvshlrcb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3lczmdobf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3akzgmwkd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3elmxhcxx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3yupywjhy.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3vwywpdmg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jpwsrjdg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3gvmtzpwz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzneghvt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jgvzshlu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nrjeetjb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3oseqopoz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ntjbhyot.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3xqmucyci.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vivrcobm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3evlxvuli.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wfjqizie.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3bczqlazb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ewfdkxjb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qwkhoeaf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3qjunizba.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3oxjxgnzd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zobizyfi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3blbznpxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbjbzwyz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3teeoewxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmhbvdyv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pfthgiky.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3arnlwsqj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3rqmnazoq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cdqlraks.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iexsmgtf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zikqlkdg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qziinuwg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hkdfolek.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3xrtuqmfu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3jswvcjwv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dsawnhun.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ybjbragc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xxvdptlz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jgudxfhe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3beotndcq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3jnbajuwu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uimpkivq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3arnowfzt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tpwrkzdn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dlsexzti.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ugvhelhs.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vjwsxijl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bzwvilhc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ytowgsiy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3xeaevgaa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3azthlgdv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ejgqpnke.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jvhthagr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uyhjuafa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfygudun.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohheytfg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3idwqfiic.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dalvmtqh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3fbqxhgiw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3utrtcktq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3oruavdsp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3brgwaccq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3aqbmzmvm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3plyqxtof.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yelycwyz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjyoajuc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oztvnkwa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3qhboclsb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3dblgqhab.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdgqfjws.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3nftrbwhf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3afxyhdjf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3efeeteha.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3nsrbsnsw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iahmxbxm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3sbqxpalj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bmqkwzui.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3srxxatty.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qjepkppg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3yhnoqzgu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3egvxsabn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gtctzlpm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jpxshrml.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cmnjzkoq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3dfxnqnld.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3afoqpvty.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3rrbjjrjm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mrcftqhl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3zktclzff.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3vxqlvjqa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3fqapwcte.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3lytzlrkg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3pizwkrnk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ttxavnxc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3iasjhfsi.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ckadfhgd.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ialilpix.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3gsfchlqx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3hdsbmizj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xthocljj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3hhuwvxja.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3whzkogoh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ssdivvfj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3lwrilquj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3lgrqbxps.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3nvxuritb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3wyptdqlf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3dayeafaj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3dfbhddpu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3svxtzkwr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3oivscrsb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3pqciefhz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3dtlebwkf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3uahuyhzf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3icumdcfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrhzkihs.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3hlzgopkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqfokoma.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3trqwyrkn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3whgyyauz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3siztyxzd.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dcqpwmvv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ztkvidwc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3xirslwlg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jnylgxuv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fewulwla.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fokggtci.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tkgijbph.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3yxebnljs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jnlwoqnh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3arjmywwp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3snscmwjl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tatsswqw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bsvmzsjk.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3islfhhga.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iubnlwtl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ojvxfini.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhbzidxy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hxysbvub.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3lkzfwysk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3xorfxcej.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3jfguosvy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3syckkvdt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3yfeponpx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3sjoxqbnq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3sqdfqkqp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zauwlexv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gjfkvscu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ecfuvxux.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3hvlazgep.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ppuctpup.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3iovqeteq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3omzyogoe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zmiesbmg.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pvgiwlbh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3olimnzyq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ddscsqjj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nugllhjl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xgrimlfb.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3ftitjbck.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3fdbesonk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lusetfhf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3mqbpseta.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3sbahstsk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3cwnfcxii.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ofhkvhue.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3zkpdtprz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zaccpbfm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vdbfeeye.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3kfskczgc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3qevziwhb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3goqmuvyx.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3qkfgvvbv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3lpnazwwf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dtawevlt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3elcjzezd.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3gopccnsl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3mtchcxmk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3qligxzar.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3ylysipzu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3biweblwx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3wcqbnuwu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3qpbjzoyy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3nuqbdpii.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ktywgpih.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hnxcezte.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3lcsitlnj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3aeckgckv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3nsfaxlzt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3etqczyka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrhztgxt.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3manwshlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gujabqox.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cfmiiaba.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ugvpsasq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tidmoxen.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kaxvnrbc.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kokufbxl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qnptsclt.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3vpuickzz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3wpqznynb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3udaolqev.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zdpqvvzh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zjtxwnfo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3tdjvgkvx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3flvkknit.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3fxtcscyj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3icajzddc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3leibcota.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3prnvivvv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3rtosxhtv.html


<!-- 参考信息 -->