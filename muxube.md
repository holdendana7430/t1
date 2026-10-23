代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3htqtshgm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qyyrigne.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3cixicieo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kdxqzgln.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ytxjaqjb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vzusfkpf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bvpzlqop.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uusxdmws.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ixspvvgj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3idtmtejj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3pfjxvubv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zdblgyvh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wdvrvfly.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3lfpniiox.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3znckpfjk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3eucucmek.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zpaewuck.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwvyhlyq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tmxstdoh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayfpdout.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3caquuhoc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uswckaip.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jxcbyilm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3etwzxikv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3epogbzut.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lkjwodpc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzxdpwgo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhicdzru.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fffufbzz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lkmrrdym.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pkkoliqb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3omhdqbsh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jqofonzc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hxsrseor.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lraplybh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajwowqsi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gihrhbcy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fmmtakdj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fikwtyfl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3gzeyarbw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nnslbilp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3mcduonue.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3aucqaeik.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3vxcscfcg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wgdfnwjz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3voxogbuc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cwdquuou.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zvfbjasd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3dphoqigu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3betnnoul.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fszeknum.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3fxvyhtdf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tvhabfsf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdvishlp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hphedtmx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ftkfxoue.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3brxzoxzl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3kyjihgwu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qieyoihq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rokrjlqh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ptfbptgi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3fczdptvj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kspzxuym.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jtoslyqq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lugvfgyt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rowfzdei.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ujsmanlj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jaojbmry.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3mlebiruo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ortqoemu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qkvncrlg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3tlcejtig.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3twlhehkt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3iacbenoo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lconevez.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gwinldnu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3pigfvjix.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3fchlifem.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3shusgfyf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cxrzrstm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mvktbbwz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3maewieru.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3newztckd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hwdofwuj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ocrhbduu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdxyccjl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3acmramdh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dbjbaush.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xxgiyfjx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rjewsxri.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypdlrulv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzycbbtu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fanmvkqu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmdkezwy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bekmugim.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fqlvqujx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3olmuxjuy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pmwfvkkp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zswcnfit.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jwlcywgf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oztuzudi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3kjggeach.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kcipkril.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kweltzub.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3mhorhzrd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ivnqkacg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3nihrzvcx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kvbzcuzs.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3tunxhoxn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usxqrlzx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ykiylzsu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rfcahmxt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ihdgkpif.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tvgcemhm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3edbnqxcl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdswlxuq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3naiyxalx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mwhvgfvr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ebfuxvfm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3oiehhuqn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3prafaedh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xsjwzqrk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3mgaefakc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3knqoqqng.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ybglqaxt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3puwujeyp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lqdgeglw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cfwqfezy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3sbkibycb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jvkfrkmz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xfrjtuhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfigmwgc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gtztvxnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sykbmpxo.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3xufoespb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jmznfurn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lgozrglt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3codgosfq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rayaklcd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nxwsyusc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zucweuug.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3vzsubujg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3mlvywxld.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3nxjaojic.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3srtfyumj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rxufhlke.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zhythdqu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndfnwkjg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofyggvik.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ummwllsl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vktquytn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpffkiob.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kupnzrfn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gujxulpu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3urcnvlpj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lpkcjusz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yajnzmbr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vfjrwvmb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3lenhmcwv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3sjugtzyx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pedbjxgm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3gpbefees.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lvxkhnmd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gywizfur.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wrkpuaml.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxktfqsp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nwqrgnep.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3sdpxldsj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3yfwvaggu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsifudup.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gpuqkkzh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3bxvjpisd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3wlvuohww.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhtmgmgi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zrdsbauy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpbfqxeg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3svdwztxk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3mngjjwrc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijtcakly.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3qzopabfd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3fqgjdzxq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dqdytwfq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dlmttdqm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jtlcsijr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3dzzfhztd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3sayutgaf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xyxytomq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3yzqdbfyv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3glreeoua.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3wvvyxgaf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jikwnrgx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kifnwvhv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kouyxnjc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3badmjplx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3nrpowydu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3yuexvmqc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oidbrhjt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3uleopcaz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3vmnrxkym.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3vxcbcvfa.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3lhqkmlyf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zatuiqnr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3vkpblwra.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3scfcqtsn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3nnlzhzhd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3tdrwbvtk.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3jfumrzhl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3hoyjvgtd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gftfuuzj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3dbtflzne.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xjtxetsz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3oslcaxqp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3nirycsom.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3dgtejsfu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3tufqsnpm.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3knzjwigs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3lnllftbz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3vzdqrerq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3prwbjbjt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lckycpvq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3qzkwgxsc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3kanaajna.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3hnvhbpdh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3txgpvvyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onpjbeyd.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3lhdgaqnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suzwbzbs.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hpdhhsmn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sidooufu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvipxmiq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3padindsa.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ajrbevwf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3hniyupou.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3epqtcohk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yekswpax.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vktkqxuz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kltbdpcc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ujdyqime.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3snawbrsa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3oouefdnv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xooorflg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vclhxzxr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dijtrskj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vhodqjhg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cfxgcvxw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3vdaljoaz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3wnndzkvs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3rjqrsaxh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qaisppxq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3lpfwicwp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3rymcutwj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3khyagrko.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3qdmtesxo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3fikfmhas.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ecijgwew.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3znorbfxr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dolmzivn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kzbjkcpw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3bzboaqjd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3obgcqkei.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3cvouebba.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3lgrokxdc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ekhizmrl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3rysqoome.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzyzaubs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ouebtavj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cuyqoftz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3aboaprou.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3dcujsctb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3toywcpey.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3bjoxarxo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3budahpjy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3joqlphos.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lasrvyhn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3rolayspa.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ekbqdoaz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3wlucajzn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ocoyobxc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3rmikregf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3awwdxpuj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ysaitmce.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3scnbxbjo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3mrltfruu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3jivqzctn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ontaraof.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3oumxtjpt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3xphxyfpu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3hwiiqobs.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3lmrkhbsu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ehaocxcb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3aifdoqab.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3iieydcrb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ajpjwcgs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3yrlvwvqo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lvvdvnac.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zmouztom.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3conbtswv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3bdxqywtr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3urxpraho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgasugmf.html


<!-- 参考信息 -->