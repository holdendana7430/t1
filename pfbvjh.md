代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hfzznqlp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3umtsoqfu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tincogyg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pbbqjnop.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xogjouxl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vnelkcdm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wxbphvsc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3lgstyhnr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lyvlplnr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmqzkcit.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqkksjhw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yibfnwty.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dwnharzf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cbvpcufc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3grnwqrny.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vpzixtiv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3exajtheo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rdgdipbn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqngqnth.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkhtzqvc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmugbfrq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ktltrbxe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3qlvphisa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xdrvhupd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cgrzqdwg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xlhyeawb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cuqktsjm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qybigbhm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3awqniplm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xfyliajw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3heegiqlm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3adjeaxup.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vlcpnuri.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hybbquhl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kezypnul.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gtxfmpxa.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ityzpcbl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eddgmoxm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nynihchj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3bwxtdlvl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ruqgspjg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3sunmhtci.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ztudtyka.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jshykhmi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3sdzptjcf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3tsittodt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3afzcnrcd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mlmukree.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xerksigd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lxdfaqpg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3medhjaqg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3roswoxas.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ovzrmguu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hzodgfpg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yusexlms.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3rfigmtgi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uishhonb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3yrdwozxn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3iklwrpsx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kqeimuun.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3urfrsqae.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jlcupoho.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3sgjcvnpg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmnwnmkz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibjhxwcv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zxrlboot.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rxvbarbg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3avpvqxry.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qavlhmcu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpxydlik.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3clloiblg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3angdguzh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcvrurib.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mmuukerb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrbjnlky.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wuswihak.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kgjzzhvg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tggvmesk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ygkcphdu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mbajidlf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3gurtcqmp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3koslgtpa.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ooloxhlq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3doueuhjq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bdibjaak.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jhjtfsfb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qedydddo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3shhlljlq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3vaxvczxa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3oiycvndd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hjrjqips.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mzoifzms.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3puenvvrk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3onuyhbuh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3edwctgmm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xxmdgscr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mhhomvcv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kdceasbt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zsjvulhe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnzraajx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3aqoiwlyh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gtbwddly.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3zjhzsuog.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3sqpdrlit.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3svealmjf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tdszvjih.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3abvmbgub.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lyybmqht.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ubgoseuf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ddfbycvh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bkpyzhha.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3tuoyxdgw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rqowqron.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3bcywdize.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xrdkajpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpjlejaf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gnfdomqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aioteyll.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3owfqpaaw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3euobfkmf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qqaturxt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jfggurgb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rbivhted.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmzudkgo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lvvlutdi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rfacljkq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfjksimk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3mssojazd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3obgeyjja.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bhmexvew.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgswiqbc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwxibnuw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xekvcokz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xfarwjrg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3aicopmzq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngbtbodl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hsjujrnm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3umgcsnmx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3khercodm.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3khcbgrab.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kwwrivez.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wlqjrxrl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rgkintel.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3nnbxxtgr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dalnblku.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zgagqdrc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rktdzfgs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kdcvogwm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3sejvekhq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mwafcvnw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dhqzxwiu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3xsegbovm.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3nwckwpkg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssgbqndx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qvvnksox.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rwlztoyo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ukaezqng.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gwfmbmbg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ywjtqlvy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfbdjsst.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zevqyfib.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xbqdmgxg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3snwpepcu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3bqryxiba.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3mwitnpvx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3horuumuo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tazaykkf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ybwgumdf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3baiyulee.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3elcndfmw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3pjkndlyx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rwwxqruu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qtdbviie.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3odeeqvik.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kqyubjuc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bkzicnjx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fihrrlgm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3mpdiegdh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vgtjhdpl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3pzaaxzjc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gmvkqmct.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ghjvderd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3dwfazlip.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3tmwhcoic.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3gexoyxxh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vbgywrbh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3rqykdezm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3gtxraagm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hkteaxut.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3gxevulrc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3oksryori.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3oggxipfr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3viddjajy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ppbpvdcz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3mzzgsvsm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbbbtoji.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lgzgfiqh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3mmibaklf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3svnwklks.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3crsxzrzk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3bywhsrfg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3vvcnxjbv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3raaarzgn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xttgvqob.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3gowhnrlz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3fpowodqe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3kniorkpd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mvcndqaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rizsnvmi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3tckejigi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arqeglys.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3slyifyxl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3opwpylyq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3afihfndr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aznlxtmp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mjdvednf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3dqbsjlxa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyvhbffc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3szsmtqvx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3okijdnit.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3suanskaw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jgulsxpd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hzndkfki.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3yrojbhxv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3kuqzgwun.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gskrsdks.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhabvnys.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qyqyblek.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zmkzjxri.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3cjoszqpw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcwzrinq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3fluiofvk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wbmvcyvt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ztmwlxjs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3vxmezrmp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3wpxpmlyz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3owcqpoti.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3uzhwluld.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3eqqfikfg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3llibymhc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xozsjmyh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kogllfgs.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ridsdxrd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mfgbfpso.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xmzlyizy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kllrltxd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3drbvyejw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3yrkhqyhz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3trflxztq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3csbtlamf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dyuieuqw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wlvfyfkb.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3ktlytqwi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbpltftf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mkszlesd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3nyddscwf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3nkkuxbyo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rropbjov.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3tljxakqc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ywjohtop.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3rrphqewz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gdzhykuc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3mrvtmafy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3glgtphzg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lwscroca.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3snxrpgdk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3qjztvoai.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3wkqpdqyk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3gpmrupjg.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3espuggtn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3gwftiapj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3esjtyrgk.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3yzorvuqq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3rgkbuiqp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3xhnxetct.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3uxwsqxht.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lsbeltwh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jncxkgms.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3atnighkz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zfxayerc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3beqzafcw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3xsfzjovt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3atceglto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zesauugp.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3cbysodug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvmvrpet.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3gfkltfud.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3itlvnhio.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3njfaqhky.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3epxyjqtt.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rmvgrjtp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3xqufzqxn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3uxsbjykv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3afrwqapq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3oxfynpwv.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kftuswij.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3koqjepif.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jbgsmswk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3qseemhmd.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ijnmopcq.html


<!-- 参考信息 -->