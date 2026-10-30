代发 wailian999

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gxpricdjv.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/ghtprnmwu.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gnccbrwvs.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gmgrckgno.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gsyyiddub.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gpoyirrmu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbxorodlj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/ggraycmry.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gflqjviuu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gtnpqwiad.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gnlbadkru.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gztmsioay.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/glgmhuwvb.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gdzokquuv.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gglhkjsko.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gzoadkpcf.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gmoxeluxg.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gqvjktccv.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/goswlhluf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gzuxmmyop.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gkdcwgswg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gnrijbwei.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/ghvbgvtkm.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/griqklnvg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gllvvkgxr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/goufvfmyo.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gztbjetad.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/guynovlbs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gbodcjfjg.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gjslkznla.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gdusjwtbw.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gefkdkytt.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gxfmjjiwg.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gnkwlacwj.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grtexoeyq.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gdmviadnw.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gyhycuwfr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gcnipwbyl.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gmisghsii.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gojuazfbf.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gbbxjxlks.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gxhzwwczg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gqtlokzyn.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gemwaywdr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gooylulpp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmfhcxqlc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gtfxyzlny.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/ghgakzghy.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/ggafgzadx.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/genzeuhkx.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gebplxure.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gtjmjlpjp.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gtwgfnjmd.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gomrjmefm.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gkwefszpo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gownkzmib.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gjhcmkajc.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/giwqnxrba.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gnumqwjgb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gtpvoclpp.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gdtyoautr.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gviwfgowh.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gfixxbzok.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gwpieyphi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gvpndbzwv.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gaxfbqmjh.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gczvmikbi.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gbaacqiqv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gjturkdzf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/ghdghjtfp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gfyaoyhdr.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gxwjcacdm.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gjyyvqazq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gwargmphb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gsynajsqy.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gjzopnekk.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gzitfoqfy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gxjcvdgrb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gtonhfzry.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gmnohogif.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gggidpdnx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/glxplzczx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/ggwopouvr.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gjcsjzsww.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/goqzpmgcy.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/glrmwvbjh.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/geycwajem.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gbmqkxerg.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/guvfhcory.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/glfxzwpek.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gekbuokdi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gfvoazhzj.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/grmjcuveu.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/goxdzfghc.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gazapaist.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gujsudhdm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxzmyvqxc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ghogqachp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gzaztkgco.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gdznsipgg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gkpkzcvsi.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gudbxysly.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gwkayhbxb.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gzgqhyvfk.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/grqiiapdr.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/grpljkcfm.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ghwxytmyr.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gbbgaovxf.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/geityznye.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/ghkfmsoru.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gapccsukq.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gvbszjfja.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gomfyjaph.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gtwraaicd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gouvgzsvz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gplrxezbr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gbtpbgzdu.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/glswmoueh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gdpubjepb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gvebtbmsc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gbkxoitql.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gibjpyfym.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gzctbjczg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gesimlveq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gaxzdckbw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gqhavwkfi.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gcokrejik.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/ggiysnqul.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/glyomkopr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gfoisvfgg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gvaxqcyxv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gdnpfsqpk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/ghrlqlvao.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gsjcypzph.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gmnkvebty.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gihxscqyq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gdvrclhzh.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gdewwcqcx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gespkmnyx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glfbvesll.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gbbddkiie.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggmhobjdi.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/guseaikbe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gxlyrjegp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gqjlbzmag.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gjsyumgug.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gkwyjufdy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gtnuydfdy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gbvplomsx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gppvfinrl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gyzpujrih.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gtcfhukbt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gmqatbkwj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gdtygelfp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gznkyrlpn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gybblhdgq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gbgatrats.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gitsuvxgt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/goajrmnuj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gcedkhfip.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gjnlhvuak.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gwmwkgbvg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gcuzhaxdg.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gidoaijih.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gtcspehbz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gojqrtexi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gsbubyhgf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gxbgixorj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gxqtgcfbv.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gahbifhpo.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gziuanmbk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/givqpeajq.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gkxjiglsm.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/girpezflu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/ghkewymga.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gppusohty.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gfigpcuud.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxlpgjlad.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gmuaffyxf.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gloucrcml.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gsothihts.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gonvvcsro.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/ggwzyxkxh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gergewapt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gfwfyckfk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gkalnldqv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gyqnrvabs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/glyiufqtu.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gsgibmcmv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gsdpthhqw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/grjjgrxbh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gzwpngniw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/ghqbydjaa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gignpccqv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gyyewjkup.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gdwvrldvg.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gybutzkki.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/giyssybaq.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gequvblqn.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gdnaipslb.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gqranetvk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gpgvnserg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gbwzyqgek.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gscrvurvd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gndgseqoo.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gzexmpkcx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gxmlytcor.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gddhmcxid.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gogyxajqi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gmzsgomvb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gltgqcwmk.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gwetvkvos.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/guhoutqqk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gdsbblmwe.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/ganxujlrp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gxoiusdwl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gtauitlna.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gdnfajein.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gedajpfpt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gdlntbkxv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/guqeevyuu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gumpiggoo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gthepxduo.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gxsqsrggy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gnjcpppnj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gpzrvizgx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gbviobdra.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gosxrdipi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gngzdxubr.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gfjvtpyff.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gbjvmzzqw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gkjiifprx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvmsyjaxc.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gomhueult.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjmothhyv.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gszxppjnq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/ggngqwcyt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/gsniszkgd.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gnlxegslz.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gegqswbtn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gkcpbugzk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gqjnnxxbi.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gxotnalub.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/ggnmglkyt.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/gcgbrxwjx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gxvrmyspc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gsexuxcjh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gcldrjicx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gfvilfxca.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gdcnkflhj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gbfnwzdzz.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gxicqjtpi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/geobybmza.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gxohzqtwy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/giofpcdht.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gbmqoodzj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/glsutimcj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gmxogoffo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gvaxfsgrw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gpxsgfszf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/genlygkbh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gcjdoafos.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gzgutndma.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/glsqdlear.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gqcjumjkw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/ghvtlkyfg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gyuwaacth.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gyixskqqi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gcxwekznm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gzeyulaie.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gjrncrzye.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gphnbxavj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/gilahijny.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gjmhckalj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gijlqcbnr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzcgvkpz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/ghcqrqjkh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gxdpvfuga.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gyuruleup.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/ggjxommin.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gymvqjsdq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gtqzitmem.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gfqhfuchh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gqgyzxaeg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gtkmpunvc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gbtgixatd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/geeammvcd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gnrwtvgbv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gdyghbfxo.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/giwgbjqno.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gbfzknzbv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gugqvclga.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/ggjtvybcz.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gqcrfygny.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gxdnrpjpi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/gpcbzbkgd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/grucbupnb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/gbikrokcc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gviwlogio.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gsvwhtpoe.sHtML


<!-- 参考信息 -->