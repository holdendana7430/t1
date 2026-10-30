代发 wailian999

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gccggehqn.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gkomwdwme.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gjtmazhtk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/geylopgtn.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gaxvsphyo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gfuzyvorp.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/guhwkfaal.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gwhrhrbhp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gccwhpkjy.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gfhhhurcs.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gvkdxltmo.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/glvqecpzc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gdzyadrgf.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gguipnooj.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gvwcvgkee.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gfisqcpvw.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gyidwhoox.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gyiyupghk.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gvillgple.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gfuhfaqsc.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ghybhbvwg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gdltuyjfs.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gtslwejhk.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gmatowpwm.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/glhxmgytr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/glohnilsq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gmocovncl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/grqvmytvg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gplcvwxxo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwwlvswti.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gbvapylil.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gjgjvbybo.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gwbwubkwp.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gxdtriqyu.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gnciwywsb.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gxqshbgor.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gqmqhyjxx.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gzxwhzsjx.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gppgjitdd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/guxqautka.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gsocekdjv.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gutphdcmf.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gmokaizbw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/glfhqnwgs.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gzrujebll.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gjnxpbhsp.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gtegkpfer.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gjjblkbni.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gncteblmz.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gsoafydwj.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gejzgalch.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gbfwlpvbi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gzmlhfbbi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gawbdnhdq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gwjlcnrrx.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gwbiamueb.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gnxehwmjc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/grkvqdfjc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gigdifkqr.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gynsyoizw.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/ggxhlyskn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gtfyzpfky.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/ggytutscn.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gwacepgqu.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ggzincocd.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gjznqrivj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/ghdlplkkh.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/giqmcfiji.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gsddcvice.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gghrfxvxr.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gwgzfqdjo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gzhbxfmfm.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmmxdfpkp.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gmjexseru.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gvefezvsi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/ghgbfmnon.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gwhrmmnqa.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gqgzexroc.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/griuleqml.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gzmxkydsl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gaoqxexui.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gqgvrsodu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gojhwomwv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/glajtjmvi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gvuvbrfzj.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gnpdhopsg.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gnooppxlu.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gqlfbtjlr.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/govfhcgrn.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gbujdasrn.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/glchfvsks.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ggjsfenqg.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gzshwtqsp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gjrcpkfmj.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gnlsnxwxt.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gowkisgwd.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gvrwgjvog.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gtaorwbfa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gwigxvkgo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gelaislow.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/ghiuajrny.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/guvwkwldc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/ggthfhqdz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gydrnfneu.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gqnmvaaaq.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gngperfau.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gmhrsgggh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gnqvfppzx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gqdbggruu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gswurdmcr.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/ggfwzaeyj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gprxtgrls.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/ghbbgoudy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gcngkarza.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gdoaqzmfy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gtfzbsvpc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gjfvwbomy.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gbljmzknd.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkensqxao.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/grrwrmbiq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gfpiseyly.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/guhxujeop.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/ggynvkekv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gljluedmy.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gkrzcmvuw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcmbzzozs.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gvcddnvfi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gqltphsqw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjdoxrpzo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gdillcggo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gqudsjqvr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gqukrlegn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/goqifhwud.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gqiyofimh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gbicjsgao.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/garjeucpa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gsqaodbyt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnyxiakac.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gbfbapwvc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gjubjdqnw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gxzmudowz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gogtqndnv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gztjiqtaj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gccyirwyw.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gvpmlmvnm.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gbzonqcbu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gmramqgkf.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gbxrrrfpl.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ggvcfqfjw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gaaypptrl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gybxmzvzv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gtggoulju.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gwoxvvsul.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gzxaodqxv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gqthwenlo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/giwlndkry.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gmnpdutap.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gasivrsds.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gpqpcencv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gdafeaqkj.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gtttghxme.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gfbfrjkvu.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmqkpgdle.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gmhmrvjii.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gropnswya.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gyyeqzpet.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gitmkatgr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gnqdlxltq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gqoptlmnc.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/ghscobrag.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gsowrsrcc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/grdbpytql.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gqvbsizbx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/glzuhdlgv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gzanetamh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gpxcsfudt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gujancrkn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gszrwsdvk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gamblxqkj.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gzqehunlt.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gngwqzpmb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gpzxasoes.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gjkjxadto.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gegqarbxa.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gaqatpypu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gfobqiytc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/grzaahptp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gzbuyxtzv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ggnmpxtls.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gbfkydtyf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gjfixpvgy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gtlrskcse.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gkmdtizop.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gzocyszrj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/ghrqcfzfs.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gflqnvwun.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gxuytwlsq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gssetxfey.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gchwinpdz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/ghhujuxzt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/ghdarisho.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/ghwxyybro.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gzzjomicu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gwohkppzk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/ghdehlrcr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gpnfwitnu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gmrfwmbjq.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gyvebjdhf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/ghyebccon.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gxlgucjvx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gdncuknrf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gpzqttkwy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gbktxjkkq.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gdoetbsbg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gbfkqfcfq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gauuiofwq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvbnpezuv.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gtniazqkp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjiiwoznr.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gkdktffmf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gpfujkxvj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/ghxsksxlp.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmshpiiiz.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gjussxsjt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/guszcnuzl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxarbkqgp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxydfzxfe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gimuvyivh.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gkzuunlgf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gtquwgdoy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gqinefvmr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gsmrfgktl.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gqseuzmfs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/goicunuqc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/grpoxttsy.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gxqtgcikm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gyghozeqr.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/grhhkylqt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/grpzrerwv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gjzxwcmrt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gibicdung.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gdhttkbrm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gghhdonrw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/geodrkuce.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gbvugkcsl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gzgondewx.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gfzddnmun.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gusbvbcyi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gzeegirry.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gqlffbxch.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gmwxdqqsq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gorgzourg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gqvwjylza.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/ghwqdiqln.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gzqiirtns.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gegqztfzn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gaqiqajgu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gkfjzjidr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gerublnec.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gougeglcr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gwbrljtwt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/golyovbog.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gratlzoul.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fehbvm.com/Article/details/gsnptipgs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gvjujaabn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gvzxydegt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gocboinyc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gjiioagof.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/ggyusdlud.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/guppxahqx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/glbvcrhul.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/guuywvjey.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gerggehyi.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gfylbciri.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/guyidotgd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gctlkfdde.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/ghhcvafpe.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/ggfosunfx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/ganxxetzl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gjntqtmnx.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gkercxmzt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/gcgzdywed.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gujxhrvig.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/ggpfqysyc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/grnzylayd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gvwxufjmb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gmrwoblbj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gvrptiudz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gfthcekja.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/ghscdvrpm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gzhacdwod.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwcjcpbmf.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gdwjervio.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gepbtfsrw.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gfmfiqcbt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/gfjjinyut.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gmzlpmxck.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/genubcann.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/govfmpvjg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/gbkizlfxp.sHtML


<!-- 参考信息 -->