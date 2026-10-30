代发 wailian999

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gjwunknyk.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gdibgqtib.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gwuljpmcc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/grqsiojys.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gkpbnwblx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gmqwsdpcd.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/ghvaqftez.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gqllaujcy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gttneakcu.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gesmkcxuy.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gfppyxnzf.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqhvenvua.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gxqnvtanu.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gwqguaoru.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gnvskgtra.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/ggiwrlrpp.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/giozpvcrk.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfzoslqse.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gvlekluzd.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtrtdoapw.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gzkklhduf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gwqtnsqby.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/guaffyzsc.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gdkadbdjs.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gnxcucgkq.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gqfrazrmz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gwzbybezi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gpwywfauu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gjgyxlrcw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gmlcobvqu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/grtxahmca.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gnwhesyol.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/ghuwkttym.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/grnlrkzte.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/ggsktaqat.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gzibfilxn.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/grgynzivz.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/guloecbxj.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/grcivvhti.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gdavxguor.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gvisetcnp.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gnetwdgko.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gdbvwmyvz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gzdkpynwm.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gpnvmmjad.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gwedfwkuz.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/geoqryebn.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gtypzftds.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gtvldlovj.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/giwuxlhzn.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gfujhhqzc.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gcoblabjl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/grqbezart.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/ghgfudcub.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/giavoajjk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gotifwfuo.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdaexphwa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gwuncynvv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gpwpftfrg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnupzxsiv.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gmpywnbbw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/ggzledjfg.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gtfxesytu.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gtvgjksfm.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gfikukjyh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gubnyordh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gclkmrvsa.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gwurytruf.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gnvyjifcq.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gtjbnugil.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gqnyblxxh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gbckrzzyz.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gshzncrfb.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gqwnzsqem.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gityedpgv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/ggxhbgqxf.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gobuunvcy.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gijrqdscc.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/godnovjol.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gzwbtdsnh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gqrltrfhz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gikwwssko.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gjrbsbnqg.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gwwxweuko.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/grayozeav.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gkfgjzmki.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gcmnnbvfx.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/goezokecg.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gqygajipz.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gglzvmzxq.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ggvcxzvbm.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gheifxrta.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gdsofnyit.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gfnfissgj.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gfagutafa.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/glgiwnxyi.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gpewncxdj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gbbzjnkzn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gyckgiggi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gzbocfspc.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gihsqkbnn.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gahtrsjlz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/giiqrsown.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gntvybxrq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gwiwbsgey.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gipfwqsyu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gkwocscdx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtwnmdfxc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gfujtzzrq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gdelarlid.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gqkcynrnw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gunnwrdxk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gusgtxdno.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gzejalyvi.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gnelmlkpi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gfxontubo.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gzdgrzmrc.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gylwrxmow.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gznxrprrx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gvofdacrn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gihnerrnn.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gbtxyfugg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gowdqwpfp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtusufvdz.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gyiyylvgz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnginuilu.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gffxzzxao.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/ggxzsbjrr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gfnhflbiv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gxootjevd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gucullnrm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gnsfidxjm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/guupmirgm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gczoxucsb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gmlmjczss.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gqlxmgkiw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/glgnwayhf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gwlxlwjbk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gwvoogroe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gdrugslkd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gmdedmlgr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gapqwwath.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/ghykglziv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gwmpkqbwk.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/glhkajesj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gozwpvhbg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gvccmlgkf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gkabtlzlh.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gkqpokahb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/ghkrayyvi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/ghqgavdex.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gelboaqjd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gjmpoplri.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gsdekhqkl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gijjemopu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gejoagwrx.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/grqsmlgdn.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gybhhtifq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/grdfgvxms.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/garsxccop.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gkcuuircv.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gcytcxcnm.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gbtyznlrt.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gevezezmd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/greeizekz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpthkqqnj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gwjxtvtbk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/ghsedfliv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/glwgvkvpo.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gyoizurbp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gmkdlcvmf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gdwrgwfab.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/giuzothuw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gdoqubsxx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gzxfgcbbc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gupidlkdz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/giznyhdqs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gnrifjlhi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gxgjnoumd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/guaprrwyx.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gkhtvnadc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gmotgxoss.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gsetkmncb.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gccargkek.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gvctavycx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gkqkbslbi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gspjpnwhp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/guppyglyg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gkosmvmap.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gjcturndy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/guansefgt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gtdinmwzd.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/ggyhhaojf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gswqsckgm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gvjlseiye.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/ghbyyimlm.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/ggtvjniou.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gylibouak.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/guewrhiep.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gtctyvvyc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gvfvmgjak.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gdoikeqon.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gjwsyiahm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gjmgfhzep.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gbadmbllt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gdlgeyxdd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gzrdffelq.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gnxcebzus.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gmixuquif.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/ggwagrpjt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gftdxxhvt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gxinapoqe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/geqrlhhnc.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/giebdsmrc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gmumcrchx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpzevazfn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gutptvicr.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gbqxxzzuh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzawloiht.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/goavrdtqh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/ggspcjiys.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gmhjahblk.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gjviqyiff.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/giaoaavpn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gxxonzwff.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzxotrmef.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gumchbcmw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/goaaweknz.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gculriifq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gqllsylog.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/grduascwq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/glazmyyhs.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gzepmsbrl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gvkwzsmnb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gwswwkwmi.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gnibjyfiw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gdplxdhfh.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gebxwtvoz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gtlgmnrzk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gdnyjpfru.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/ggejjhrfl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/giqxssfll.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/ghehcicnu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/ghpkscweo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gwrxsooii.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gynejkdpl.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/grqgyxtap.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gtwsjrekl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ggxkqmlmr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gsfbmxrjz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/ghlmdtkiq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/ggroauuqj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/ghcvrfsov.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gnadeydxv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gbkabbjvf.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gidrrbart.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gxvcpwofm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/ggwatycnj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gvnvvdllo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gdvzgzvfz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gxascyezr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gnkpfkjyx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gjzbnzlpw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gvqltmkpr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gfruxylii.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gpqopylht.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gmtklplby.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/godahssur.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gvthnatni.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gvzyyyhgj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gtqfsfjnn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gfztakuce.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gjlbahgzu.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gwtbyubxi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gvmvuxypn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gjaguylui.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gepofnfbq.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gluwxmbqn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gevdfkuuf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gmvnupvzt.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gpfrkdnwv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/garxorqfz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/grmlrxrel.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/gjadlxiur.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gvasxuktg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gefygyoxb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gwkjzauol.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/grhrhliko.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gwcyntlwi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gnlazatam.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gsfyviyyg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdtcfyfca.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gxfiwppcl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gahbopwfh.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/ghttgasim.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gsikeiyhu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/getjrmzta.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gucrpsuvv.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gbyukgocd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/grgixhsnm.sHtML


<!-- 参考信息 -->